---
title:  indexed_set
tags:
  - CP data structure
  - CP
  - CP indexed_set
---
<!--more-->
## Cú pháp các hàm
```cpp
#include <bits/stdc++.h>
using namespace std;

#include <ext/pb_ds/assoc_container.hpp>
using namespace __gnu_pbds;
typedef tree<int,null_type,less<int>,rb_tree_tag,tree_order_statistics_node_update> indexed_set;

#define debug(x) cerr << #x << " = " << x << endl;
#define int long long

main(){
//    freopen("input.txt", "r", stdin);
    ios_base::sync_with_stdio(0);cin.tie(0);
    indexed_set s;
    s.insert(1);
    s.insert(5);
    cout << *s.find_by_order(0) << endl; // 1
    cout << *s.find_by_order(1) << endl; // 5
    cout << *s.find_by_order(3) << endl; // 0
    cout << s.order_of_key(1) << endl; // 0
    cout << s.order_of_key(5) << endl; // 1
    cout << s.order_of_key(0) << endl; // 0
    cout << s.order_of_key(3) << endl; // 1
    cout << s.order_of_key(10) << endl; // 2
}
```

## Bài tập vận dụng

### cf.div3.744.b

Đề bài: Cho một mảng số nguyên. Hãy sắp xếp lại mảng. Được sử dụng thao tác sau không quá n lần: chọn 1 đoạn [l,r] của mảng, dịch sang trái k vị trí. Ví dụ 2, 5, 3 dịch sang trái 1 đơn vị sẽ là 5, 3, 2. Xuất ra các thao tác đã thực hiện để thu được mảng không giảm.

Showcode: O(nlogn)
```cpp
#include <bits/stdc++.h>
using namespace std;
#include <ext/pb_ds/assoc_container.hpp>
using namespace __gnu_pbds;
typedef tree<int,null_type,less<int>,rb_tree_tag,tree_order_statistics_node_update> indexed_set;
#define debug(x) cerr << #x << " = " << x << endl;
#define int long long

main(){
    freopen("input.txt", "r", stdin);
    ios_base::sync_with_stdio(0);cin.tie(0);
    int t;
    cin >> t;
    while(t--){
        int n;
        cin >> n;
        vector<pair<int,int>> res;
        indexed_set is;
        pair<int,int> a[n];
        for(int i = 0; i < n; i++){
            cin >> a[i].first;
            a[i].second = i;
        }
        sort(a, a + n);
        int b[n];
        for(int i = 0; i < n; i++){
            b[a[i].second] = i;
        }
        for(int i = 0; i < n; i++){;
            int u = is.order_of_key(b[i]);
            if(u < (int)is.size()) res.push_back(make_pair(u, i));
            is.insert(b[i]);
        }
        cout << res.size() << "\n";
        for(int i = 0; i < res.size(); i++){
            cout << res[i].first + 1 << " " << res[i].second + 1 << " " << res[i].second - res[i].first << "\n";
        }
    }
}
```


