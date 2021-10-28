---
title: 'Problem: Vupsen, Pupsen and 0'
tags:
  - cp
  - constructive algorithms
---
Cho mảng a gồm n `(2 <= n <= 1e5)` số nguyên `(0 < |a[i]| <= 1e4)`. Tìm mảng b có n phần tử sao cho `tổng của tất cả |b[i]| <= 1e9` và `tổng của tất cả a[i] * b[i]` bằng `0`.

<!--more-->

*Submit [tại đây](https://codeforces.com/contest/1582/problem/D)*

**Hướng dẫn**

  - Pending

**Code**

- Độ phưc tạp **O(n)**

```cpp
#include <bits/stdc++.h>
using namespace std;
#define debug(x) cerr << #x << " = " << x << endl;
using ll = long long;
const int N = 1e5;
ll a[N], b[N];
int n;
void solve(int l, int r){
    int sz = r - l + 1;
    if(sz % 2 == 0){
        for(int i = l; i <= r; i++){
            b[i] = a[r + l - i] *(i < l + sz / 2? 1: -1);
        }
        return ;
    }
    if(sz == 3){
        vector<pair<ll,int>> v(3);
        for(int i = l; i <= r; i++){
            v[i - l] = make_pair(a[i], i);
        }
        sort(v.begin(), v.end());
        if(v[0].first + v[1].first == 0){
            b[v[0].second] = v[2].first;
            b[v[1].second] = -v[2].first;
            b[v[2].second] = -(v[0].first - v[1].first);
        }
        else {
            b[v[0].second] = v[2].first;
            b[v[1].second] = v[2].first;
            b[v[2].second] = -(v[0].first + v[1].first);
        }
        return ;
    }
    solve(l, l + 2);
    solve(l + 3, r);
}
int main(){
    // freopen("input.txt", "r", stdin);
    ios_base::sync_with_stdio(0);cin.tie(0);
    int t;
    cin >> t;
    while(t--){
        cin >> n;
        for(int i = 0; i < n; i++){
            cin >> a[i];
        }
        solve(0, n - 1);
        ll check = 0;
        for(int i = 0; i < n; i++){
            cout << b[i] << " ";
//            check += a[i] * b[i];
        }
        cout << "\n";
//        debug(check)
    }
}
```
