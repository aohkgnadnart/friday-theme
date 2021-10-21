---
title:  'Problem: People are leaving'
tags:
  - cp
  - dsu
  - path-compression
---
Cho n người đang đứng ở vị trí từ 1 tới n. Bạn phải thực hiện các truy vấn thuộc 2 loại:

- `- x` Người ở vị trí x rời đi.
- `? x` Người gần nhất bên phải vị trí x.

<!--more-->

*Submit [tại đây](https://codeforces.com/edu/course/2/lesson/7/2/practice/contest/289391/problem/A)*

**Hướng dẫn**

- Bài này cần sử dụng dsu kết hợp nén đường dẫn(path-compression) để không bị TLE.

**Code**

- Độ phưc tạp **O(nlogn)**

```cpp
#include <bits/stdc++.h>
using namespace std;
const int MAX=1e6+1;
vector<int> link(MAX+1);
int find(int a){
	if(a != link[a]) return link[a] = find(link[a]);
	return a;
}
void unite(int y, int z){//a<b
	z=find(z);
	link[y]=z;
}
int main(){
	ios_base::sync_with_stdio(false); cin.tie(0); cout.tie(0);
	for(int i=1; i<=MAX; i++) link[i]=i;
	int n, m;
	cin >> n >> m;
	while(m--){
		char x;
		int y;
		cin >> x >> y;
		if(x=='?'){
			y=find(y);
			cout << (y==n+1? -1: y) << "\n";
		}
		else unite(y, y+1);
	}
}
```

