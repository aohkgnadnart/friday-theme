---
title: 'Problem: xúc xắc bò'
tags:
  - cp
  - brute force
---

Có 3 con xúc xắc cân đối, với số mặt lần lượt là s1, s2, s3. Xuất ra tổng giá trị của 3 con xúc xắc xuất hiện nhiều nhất.

**Code:** O(s1 * s2 * s3)

```cpp
#include <bits/stdc++.h>
using namespace std;
#define debug(x) cerr << #x << " = " << x << endl;
using ll = long long;

int main(){
    // freopen("input.txt", "r", stdin);
    ios_base::sync_with_stdio(0);cin.tie(0);
    int s1, s2, s3;
    cin >> s1 >> s2 >> s3;
    int n = s1 + s2 + s3;
    vector<int> cnt(n + 1, 0);
    for(int i = 1; i <= s1; i++){
        for(int j = 1; j <= s2; j++){
            for(int k = 1; k <= s3; k++){
                cnt[i + j + k]++;
            }
        }
    }
    int p = 0, val = 0;
    for(int i = 3; i <= n; i++){
        if(cnt[i] > val){
            p = i;
            val = cnt[i];
        }
    }
    cout << p;
}
```
