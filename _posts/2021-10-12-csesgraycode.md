---
title: 'Problem: Gray code'
tags:
  - cp
  - recursion
---

Mã màu xám là danh sách tất cả 2^n chuỗi bit có độ dài n, trong đó hai chuỗi liên tiếp bất kỳ khác nhau đúng một bit (tức là khoảng cách Hamming của chúng là một).

Nhiệm vụ của bạn là tạo mã Xám cho một độ dài nhất định n.

<!--more-->

*Nhận xét: Gặp những bài này, cố gắng nháp viết ra được cách đệ quy*

*Submit [tại đây](https://cses.fi/problemset/task/2205/)*

## Cách giải đúng

![image](https://user-images.githubusercontent.com/83690404/136924864-133193ea-f466-49e0-9f8e-c1960365a90c.png)

**Code 1**

```cpp
#include <bits/stdc++.h>
using namespace std;

int main(){
//    freopen("input.txt", "r", stdin);
    int n;
    cin >> n;
    vector<int> res;
    res.push_back(0);
    res.push_back(1);
    for(int i = 1; i < n; i++){
        int sz = res.size();
        int x = (1 << i);
        for(int j = sz - 1; j >=0; j--){
            res.push_back(res[j] + x);
        }
    }
    int m = (1 << n);
    for(int i = 0; i < m; i++){
        for(int j = 0; j < n; j++){
            cout << ((res[i] >> (n - 1 - j))&1);
        }
        cout << "\n";
    }
}
```
**Code 2:**

```cpp
#include <bits/stdc++.h>
#define ll long long
#define debug(x) cerr << #x << " = " << x << endl;
using namespace std;
vector<string> v(1, "");
void solve(int n){
	if(n == 0) return ;
	solve(n - 1);
	int k = v.size();
	for(int i = k - 1; i >= 0; i--) v.push_back(v[i] + "1");
	for(int i = 0; i < k; i++) v[i] += "0";
}
	
int main(){
	ios_base::sync_with_stdio(false); cin.tie(0); cout.tie(0);
	int n;
	cin >> n;
	solve(n);		
	for(auto val: v) cout << val << "\n";
}
```

## Cách giải sai

- Quy về bài toán đồ thị, 2 đỉnh i, j được nối với nhau nếu distanceHammil(i, j) = 1.
- Bây giờ tìm đường đi đi qua tất cả các đỉnh, tức là đường đi Hammilton.
- Bài toàn tìm đường đi Hammilton là bài toán NP-hard cho nên ta phải nghĩ cách khác để ko TLE
- Nhận thấy với giá trị n, đồ thị có 2^n đỉnh. mỗi đỉnh sẽ nối với đúng n đỉnh. Ta dfs tham lam luôn chọn dfs tới đỉnh nhỏ nhất có thể. (SAI với n > 5)



