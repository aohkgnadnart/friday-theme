[don-kien-nghinew.pdf](https://github.com/aohkgnadnart/aohkgnadnart.github.io/files/7653493/don-kien-nghinew.pdf)
---
title: Writing Content for Friday Theme
---

## Writing Content

1. `_pages/index.md` - this is the default home page.
2. `_includes/components/intro.md` - this chunk is reused between the top of the homepage and the top of the about page.
3. `_pages/about.md` reuses the intro and adds a bit more content about yourself.
4. `_posts` is the default Jekyll collection of blog posts. Each post has a list of tags. These lists are combined into a tag cloud on the post list page.
5. `_projects` is a directory of project pages. These are not organised into a collection. Each page can hold a description or documentation about a hobby or open-source project.

## HTML Content

Jekyll lets you mix HTML into Markdown in the content, so it is possible to add HTML content. You can use this to utilise Bootstrap 4's components. The [blog posts]({{ site.baseurl }}{% link list/posts.html %}) have some examples.
## Each page can hold a description or documentation about a hobby or open-source project.
```cpp
#pragma GCC optimize(3)
#include <bits/stdc++.h>
#define debug(x) cout<<#x<<":"<<x<<endl;
#define dl(x) printf("%lld\n",x);
#define di(x) printf("%d\n",x);
#define _CRT_SECURE_NO_WARNINGS
#define pb push_back
#define mp make_pair
#define all(x) (x).begin(),(x).end()
#define fi first
#define se second
#define SZ(x) ((int)(x).size())
using namespace std;
typedef long long ll;
typedef unsigned long long ull;
typedef pair<int, int> PII;
typedef vector<int> VI;
const int INF = 0x3f3f3f3f;
const int N = 2e5 + 10;
const ll mod = 1000000007;
const double eps = 1e-9;
const double PI = acos(-1);
template<typename T>inline void read(T &a) {
    char c = getchar(); T x = 0, f = 1; while (!isdigit(c)) {if (c == '-')f = -1; c = getchar();}
    while (isdigit(c)) {x = (x << 1) + (x << 3) + c - '0'; c = getchar();} a = f * x;
}
int gcd(int a, int b) {return (b > 0) ? gcd(b, a % b) : a;}
char str[N];
int n,m;
int sum[N];
map<int,VI> M;

int check(int l,int r){
    int x = sum[r] + sum[l - 1];
    return *lower_bound(all(M[x]),l);
}

int main() {
    int T;
    read(T);
    while(T--){
        M.clear();
        read(n),read(m);
        scanf("%s",str + 1);
        for(int i = 1;i <= n;i++){
            sum[i] = sum[i - 1] + (i%2?1:-1)*(str[i]=='+'?1:-1);
            M[sum[i] + sum[i - 1]].pb(i);
        }
        while(m--){
            int l,r;
            read(l),read(r);
            if(sum[r] - sum[l = 1] == 0) puts("0");
            else if((r - l + 1) & 1){
                puts("1");
                di(check(l,r));
            }
            else{
                puts("2");
                printf("%d %d\n",l,check(l + 1,r));
            }
        }
    }
    return 0;
}
```


https://user-images.githubusercontent.com/83690404/133911677-878f24f0-2bd3-4477-9fc9-0b679088c017.mp4

[![Untitled](https://user-images.githubusercontent.com/83690404/133911897-818cd986-febf-437d-a449-2a3b4f651c92.png)
](https://user-images.githubusercontent.com/83690404/133911677-878f24f0-2bd3-4477-9fc9-0b679088c017.mp4)
## HTML Content
## HTML Content
## HTML Content
## HTML Content
1. `_pages/index.md` - this is the default home page.
2. `_includes/components/intro.md` - this chunk is reused between the top of the homepage and the top of the about page.
3. `_pages/about.md` reuses the intro and adds a bit more content about yourself.
4. `_posts` is the default Jekyll collection of blog posts. Each post has a list of tags. These lists are combined into a tag cloud on the post list page.
5. `_projects` is a directory of project pages. These are not organised into a collection. Each page can hold a description or documentation about a hobby or open-source project.1. `_pages/index.md` - this is the default home page.
2. `_includes/components/intro.md` - this chunk is reused between the top of the homepage and the top of the about page.
3. `_pages/about.md` reuses the intro and adds a bit more content about yourself.
4. `_posts` is the default Jekyll collection of blog posts. Each post has a list of tags. These lists are combined into a tag cloud on the post list page.
5. `_projects` is a directory of project pages. These are not organised into a collection. Each page can hold a description or documentation about a hobby or open-source project.1. `_pages/index.md` - this is the default home page.
2. `_includes/components/intro.md` - this chunk is reused between the top of the homepage and the top of the about page.
3. `_pages/about.md` reuses the intro and adds a bit more content about yourself.
4. `_posts` is the default Jekyll collection of blog posts. Each post has a list of tags. These lists are combined into a tag cloud on the post list page.
5. `_projects` is a directory of project pages. These are not organised into a collection. Each page can hold a description or documentation about a hobby or open-source project.1. `_pages/index.md` - this is the default home page.
2. `_includes/components/intro.md` - this chunk is reused between the top of the homepage and the top of the about page.
3. `_pages/about.md` reuses the intro and adds a bit more content about yourself.
4. `_posts` is the default Jekyll collection of blog posts. Each post has a list of tags. These lists are combined into a tag cloud on the post list page.
5. `_projects` is a directory of project pages. These are not organised into a collection. Each page can hold a description or documentation about a hobby or open-source project.1. `_pages/index.md` - this is the default home page.
2. `_includes/components/intro.md` - this chunk is reused between the top of the homepage and the top of the about page.
3. `_pages/about.md` reuses the intro and adds a bit more content about yourself.
4. `_posts` is the default Jekyll collection of blog posts. Each post has a list of tags. These lists are combined into a tag cloud on the post list page.
5. `_projects` is a directory of project pages. These are not organised into a collection. Each page can hold a description or documentation about a hobby or open-source project.1. `_pages/index.md` - this is the default home page.
2. `_includes/components/intro.md` - this chunk is reused between the top of the homepage and the top of the about page.
3. `_pages/about.md` reuses the intro and adds a bit more content about yourself.
4. `_posts` is the default Jekyll collection of blog posts. Each post has a list of tags. These lists are combined into a tag cloud on the post list page.
5. `_projects` is a directory of project pages. These are not organised into a collection. Each page can hold a description or documentation about a hobby or open-source project.1. `_pages/index.md` - this is the default home page.
2. `_includes/components/intro.md` - this chunk is reused between the top of the homepage and the top of the about page.
3. `_pages/about.md` reuses the intro and adds a bit more content about yourself.
4. `_posts` is the default Jekyll collection of blog posts. Each post has a list of tags. These lists are combined into a tag cloud on the post list page.
5. `_projects` is a directory of project pages. These are not organised into a collection. Each page can hold a description or documentation about a hobby or open-source project.1. `_pages/index.md` - this is the default home page.
2. `_includes/components/intro.md` - this chunk is reused between the top of the homepage and the top of the about page.
3. `_pages/about.md` reuses the intro and adds a bit more content about yourself.
4. `_posts` is the default Jekyll collection of blog posts. Each post has a list of tags. These lists are combined into a tag cloud on the post list page.
5. `_projects` is a directory of project pages. These are not organised into a collection. Each page can hold a description or documentation about a hobby or open-source project.1. `_pages/index.md` - this is the default home page.
2. `_includes/components/intro.md` - this chunk is reused between the top of the homepage and the top of the about page.
3. `_pages/about.md` reuses the intro and adds a bit more content about yourself.
4. `_posts` is the default Jekyll collection of blog posts. Each post has a list of tags. These lists are combined into a tag cloud on the post list page.
5. `_projects` is a directory of project pages. These are not organised into a collection. Each page can hold a description or documentation about a hobby or open-source project.1. `_pages/index.md` - this is the default home page.
2. `_includes/components/intro.md` - this chunk is reused between the top of the homepage and the top of the about page.
3. `_pages/about.md` reuses the intro and adds a bit more content about yourself.
4. `_posts` is the default Jekyll collection of blog posts. Each post has a list of tags. These lists are combined into a tag cloud on the post list page.
5. `_projects` is a directory of project pages. These are not organised into a collection. Each page can hold a description or documentation about a hobby or open-source project.1. `_pages/index.md` - this is the default home page.
2. `_includes/components/intro.md` - this chunk is reused between the top of the homepage and the top of the about page.
3. `_pages/about.md` reuses the intro and adds a bit more content about yourself.
4. `_posts` is the default Jekyll collection of blog posts. Each post has a list of tags. These lists are combined into a tag cloud on the post list page.
5. `_projects` is a directory of project pages. These are not organised into a collection. Each page can hold a description or documentation about a hobby or open-source project.1. `_pages/index.md` - this is the default home page.
2. `_includes/components/intro.md` - this chunk is reused between the top of the homepage and the top of the about page.
3. `_pages/about.md` reuses the intro and adds a bit more content about yourself.
4. `_posts` is the default Jekyll collection of blog posts. Each post has a list of tags. These lists are combined into a tag cloud on the post list page.
5. `_projects` is a directory of project pages. These are not organised into a collection. Each page can hold a description or documentation about a hobby or open-source project.1. `_pages/index.md` - this is the default home page.
2. `_includes/components/intro.md` - this chunk is reused between the top of the homepage and the top of the about page.
3. `_pages/about.md` reuses the intro and adds a bit more content about yourself.
4. `_posts` is the default Jekyll collection of blog posts. Each post has a list of tags. These lists are combined into a tag cloud on the post list page.
5. `_projects` is a directory of project pages. These are not organised into a collection. Each page can hold a description or documentation about a hobby or open-source project.1. `_pages/index.md` - this is the default home page.
2. `_includes/components/intro.md` - this chunk is reused between the top of the homepage and the top of the about page.
3. `_pages/about.md` reuses the intro and adds a bit more content about yourself.
4. `_posts` is the default Jekyll collection of blog posts. Each post has a list of tags. These lists are combined into a tag cloud on the post list page.
5. `_projects` is a directory of project pages. These are not organised into a collection. Each page can hold a description or documentation about a hobby or open-source project.1. `_pages/index.md` - this is the default home page.
2. `_includes/components/intro.md` - this chunk is reused between the top of the homepage and the top of the about page.
3. `_pages/about.md` reuses the intro and adds a bit more content about yourself.
4. `_posts` is the default Jekyll collection of blog posts. Each post has a list of tags. These lists are combined into a tag cloud on the post list page.
5. `_projects` is a directory of project pages. These are not organised into a collection. Each page can hold a description or documentation about a hobby or open-source project.1. `_pages/index.md` - this is the default home page.
2. `_includes/components/intro.md` - this chunk is reused between the top of the homepage and the top of the about page.
3. `_pages/about.md` reuses the intro and adds a bit more content about yourself.
4. `_posts` is the default Jekyll collection of blog posts. Each post has a list of tags. These lists are combined into a tag cloud on the post list page.
5. `_projects` is a directory of project pages. These are not organised into a collection. Each page can hold a description or documentation about a hobby or open-source project.1. `_pages/index.md` - this is the default home page.
2. `_includes/components/intro.md` - this chunk is reused between the top of the homepage and the top of the about page.
3. `_pages/about.md` reuses the intro and adds a bit more content about yourself.
4. `_posts` is the default Jekyll collection of blog posts. Each post has a list of tags. These lists are combined into a tag cloud on the post list page.
5. `_projects` is a directory of project pages. These are not organised into a collection. Each page can hold a description or documentation about a hobby or open-source project.1. `_pages/index.md` - this is the default home page.
2. `_includes/components/intro.md` - this chunk is reused between the top of the homepage and the top of the about page.
3. `_pages/about.md` reuses the intro and adds a bit more content about yourself.
4. `_posts` is the default Jekyll collection of blog posts. Each post has a list of tags. These lists are combined into a tag cloud on the post list page.
5. `_projects` is a directory of project pages. These are not organised into a collection. Each page can hold a description or documentation about a hobby or open-source project.1. `_pages/index.md` - this is the default home page.
2. `_includes/components/intro.md` - this chunk is reused between the top of the homepage and the top of the about page.
3. `_pages/about.md` reuses the intro and adds a bit more content about yourself.
4. `_posts` is the default Jekyll collection of blog posts. Each post has a list of tags. These lists are combined into a tag cloud on the post list page.
5. `_projects` is a directory of project pages. These are not organised into a collection. Each page can hold a description or documentation about a hobby or open-source project.1. `_pages/index.md` - this is the default home page.
2. `_includes/components/intro.md` - this chunk is reused between the top of the homepage and the top of the about page.
3. `_pages/about.md` reuses the intro and adds a bit more content about yourself.
4. `_posts` is the default Jekyll collection of blog posts. Each post has a list of tags. These lists are combined into a tag cloud on the post list page.
5. `_projects` is a directory of project pages. These are not organised into a collection. Each page can hold a description or documentation about a hobby or open-source project.1. `_pages/index.md` - this is the default home page.
2. `_includes/components/intro.md` - this chunk is reused between the top of the homepage and the top of the about page.
3. `_pages/about.md` reuses the intro and adds a bit more content about yourself.
4. `_posts` is the default Jekyll collection of blog posts. Each post has a list of tags. These lists are combined into a tag cloud on the post list page.
5. `_projects` is a directory of project pages. These are not organised into a collection. Each page can hold a description or documentation about a hobby or open-source project.1. `_pages/index.md` - this is the default home page.
2. `_includes/components/intro.md` - this chunk is reused between the top of the homepage and the top of the about page.
3. `_pages/about.md` reuses the intro and adds a bit more content about yourself.
4. `_posts` is the default Jekyll collection of blog posts. Each post has a list of tags. These lists are combined into a tag cloud on the post list page.
5. `_projects` is a directory of project pages. These are not organised into a collection. Each page can hold a description or documentation about a hobby or open-source project.1. `_pages/index.md` - this is the default home page.
2. `_includes/components/intro.md` - this chunk is reused between the top of the homepage and the top of the about page.
3. `_pages/about.md` reuses the intro and adds a bit more content about yourself.
4. `_posts` is the default Jekyll collection of blog posts. Each post has a list of tags. These lists are combined into a tag cloud on the post list page.
5. `_projects` is a directory of project pages. These are not organised into a collection. Each page can hold a description or documentation about a hobby or open-source project.1. `_pages/index.md` - this is the default home page.
2. `_includes/components/intro.md` - this chunk is reused between the top of the homepage and the top of the about page.
3. `_pages/about.md` reuses the intro and adds a bit more content about yourself.
4. `_posts` is the default Jekyll collection of blog posts. Each post has a list of tags. These lists are combined into a tag cloud on the post list page.
5. `_projects` is a directory of project pages. These are not organised into a collection. Each page can hold a description or documentation about a hobby or open-source project.1. `_pages/index.md` - this is the default home page.
2. `_includes/components/intro.md` - this chunk is reused between the top of the homepage and the top of the about page.
3. `_pages/about.md` reuses the intro and adds a bit more content about yourself.
4. `_posts` is the default Jekyll collection of blog posts. Each post has a list of tags. These lists are combined into a tag cloud on the post list page.
5. `_projects` is a directory of project pages. These are not organised into a collection. Each page can hold a description or documentation about a hobby or open-source project.1. `_pages/index.md` - this is the default home page.
2. `_includes/components/intro.md` - this chunk is reused between the top of the homepage and the top of the about page.
3. `_pages/about.md` reuses the intro and adds a bit more content about yourself.
4. `_posts` is the default Jekyll collection of blog posts. Each post has a list of tags. These lists are combined into a tag cloud on the post list page.
5. `_projects` is a directory of project pages. These are not organised into a collection. Each page can hold a description or documentation about a hobby or open-source project.1. `_pages/index.md` - this is the default home page.
2. `_includes/components/intro.md` - this chunk is reused between the top of the homepage and the top of the about page.
3. `_pages/about.md` reuses the intro and adds a bit more content about yourself.
4. `_posts` is the default Jekyll collection of blog posts. Each post has a list of tags. These lists are combined into a tag cloud on the post list page.
5. `_projects` is a directory of project pages. These are not organised into a collection. Each page can hold a description or documentation about a hobby or open-source project.1. `_pages/index.md` - this is the default home page.
2. `_includes/components/intro.md` - this chunk is reused between the top of the homepage and the top of the about page.
3. `_pages/about.md` reuses the intro and adds a bit more content about yourself.
4. `_posts` is the default Jekyll collection of blog posts. Each post has a list of tags. These lists are combined into a tag cloud on the post list page.
5. `_projects` is a directory of project pages. These are not organised into a collection. Each page can hold a description or documentation about a hobby or open-source project.1. `_pages/index.md` - this is the default home page.
2. `_includes/components/intro.md` - this chunk is reused between the top of the homepage and the top of the about page.
3. `_pages/about.md` reuses the intro and adds a bit more content about yourself.
4. `_posts` is the default Jekyll collection of blog posts. Each post has a list of tags. These lists are combined into a tag cloud on the post list page.
5. `_projects` is a directory of project pages. These are not organised into a collection. Each page can hold a description or documentation about a hobby or open-source project.1. `_pages/index.md` - this is the default home page.
2. `_includes/components/intro.md` - this chunk is reused between the top of the homepage and the top of the about page.
3. `_pages/about.md` reuses the intro and adds a bit more content about yourself.
4. `_posts` is the default Jekyll collection of blog posts. Each post has a list of tags. These lists are combined into a tag cloud on the post list page.
5. `_projects` is a directory of project pages. These are not organised into a collection. Each page can hold a description or documentation about a hobby or open-source project.1. `_pages/index.md` - this is the default home page.
2. `_includes/components/intro.md` - this chunk is reused between the top of the homepage and the top of the about page.
3. `_pages/about.md` reuses the intro and adds a bit more content about yourself.
4. `_posts` is the default Jekyll collection of blog posts. Each post has a list of tags. These lists are combined into a tag cloud on the post list page.
5. `_projects` is a directory of project pages. These are not organised into a collection. Each page can hold a description or documentation about a hobby or open-source project.1. `_pages/index.md` - this is the default home page.
2. `_includes/components/intro.md` - this chunk is reused between the top of the homepage and the top of the about page.
3. `_pages/about.md` reuses the intro and adds a bit more content about yourself.
4. `_posts` is the default Jekyll collection of blog posts. Each post has a list of tags. These lists are combined into a tag cloud on the post list page.
5. `_projects` is a directory of project pages. These are not organised into a collection. Each page can hold a description or documentation about a hobby or open-source project.1. `_pages/index.md` - this is the default home page.
2. `_includes/components/intro.md` - this chunk is reused between the top of the homepage and the top of the about page.
3. `_pages/about.md` reuses the intro and adds a bit more content about yourself.
4. `_posts` is the default Jekyll collection of blog posts. Each post has a list of tags. These lists are combined into a tag cloud on the post list page.
5. `_projects` is a directory of project pages. These are not organised into a collection. Each page can hold a description or documentation about a hobby or open-source project.1. `_pages/index.md` - this is the default home page.
2. `_includes/components/intro.md` - this chunk is reused between the top of the homepage and the top of the about page.
3. `_pages/about.md` reuses the intro and adds a bit more content about yourself.
4. `_posts` is the default Jekyll collection of blog posts. Each post has a list of tags. These lists are combined into a tag cloud on the post list page.
5. `_projects` is a directory of project pages. These are not organised into a collection. Each page can hold a description or documentation about a hobby or open-source project.1. `_pages/index.md` - this is the default home page.
2. `_includes/components/intro.md` - this chunk is reused between the top of the homepage and the top of the about page.
3. `_pages/about.md` reuses the intro and adds a bit more content about yourself.
4. `_posts` is the default Jekyll collection of blog posts. Each post has a list of tags. These lists are combined into a tag cloud on the post list page.
5. `_projects` is a directory of project pages. These are not organised into a collection. Each page can hold a description or documentation about a hobby or open-source project.1. `_pages/index.md` - this is the default home page.
2. `_includes/components/intro.md` - this chunk is reused between the top of the homepage and the top of the about page.
3. `_pages/about.md` reuses the intro and adds a bit more content about yourself.
4. `_posts` is the default Jekyll collection of blog posts. Each post has a list of tags. These lists are combined into a tag cloud on the post list page.
5. `_projects` is a directory of project pages. These are not organised into a collection. Each page can hold a description or documentation about a hobby or open-source project.1. `_pages/index.md` - this is the default home page.
2. `_includes/components/intro.md` - this chunk is reused between the top of the homepage and the top of the about page.
3. `_pages/about.md` reuses the intro and adds a bit more content about yourself.
4. `_posts` is the default Jekyll collection of blog posts. Each post has a list of tags. These lists are combined into a tag cloud on the post list page.
5. `_projects` is a directory of project pages. These are not organised into a collection. Each page can hold a description or documentation about a hobby or open-source project.1. `_pages/index.md` - this is the default home page.
2. `_includes/components/intro.md` - this chunk is reused between the top of the homepage and the top of the about page.
3. `_pages/about.md` reuses the intro and adds a bit more content about yourself.
4. `_posts` is the default Jekyll collection of blog posts. Each post has a list of tags. These lists are combined into a tag cloud on the post list page.
5. `_projects` is a directory of project pages. These are not organised into a collection. Each page can hold a description or documentation about a hobby or open-source project.1. `_pages/index.md` - this is the default home page.
2. `_includes/components/intro.md` - this chunk is reused between the top of the homepage and the top of the about page.
3. `_pages/about.md` reuses the intro and adds a bit more content about yourself.
4. `_posts` is the default Jekyll collection of blog posts. Each post has a list of tags. These lists are combined into a tag cloud on the post list page.
5. `_projects` is a directory of project pages. These are not organised into a collection. Each page can hold a description or documentation about a hobby or open-source project.1. `_pages/index.md` - this is the default home page.
2. `_includes/components/intro.md` - this chunk is reused between the top of the homepage and the top of the about page.
3. `_pages/about.md` reuses the intro and adds a bit more content about yourself.
4. `_posts` is the default Jekyll collection of blog posts. Each post has a list of tags. These lists are combined into a tag cloud on the post list page.
5. `_projects` is a directory of project pages. These are not organised into a collection. Each page can hold a description or documentation about a hobby or open-source project.1. `_pages/index.md` - this is the default home page.
2. `_includes/components/intro.md` - this chunk is reused between the top of the homepage and the top of the about page.
3. `_pages/about.md` reuses the intro and adds a bit more content about yourself.
4. `_posts` is the default Jekyll collection of blog posts. Each post has a list of tags. These lists are combined into a tag cloud on the post list page.
5. `_projects` is a directory of project pages. These are not organised into a collection. Each page can hold a description or documentation about a hobby or open-source project.1. `_pages/index.md` - this is the default home page.
2. `_includes/components/intro.md` - this chunk is reused between the top of the homepage and the top of the about page.
3. `_pages/about.md` reuses the intro and adds a bit more content about yourself.
4. `_posts` is the default Jekyll collection of blog posts. Each post has a list of tags. These lists are combined into a tag cloud on the post list page.
5. `_projects` is a directory of project pages. These are not organised into a collection. Each page can hold a description or documentation about a hobby or open-source project.1. `_pages/index.md` - this is the default home page.
2. `_includes/components/intro.md` - this chunk is reused between the top of the homepage and the top of the about page.
3. `_pages/about.md` reuses the intro and adds a bit more content about yourself.
4. `_posts` is the default Jekyll collection of blog posts. Each post has a list of tags. These lists are combined into a tag cloud on the post list page.
5. `_projects` is a directory of project pages. These are not organised into a collection. Each page can hold a description or documentation about a hobby or open-source project.1. `_pages/index.md` - this is the default home page.
2. `_includes/components/intro.md` - this chunk is reused between the top of the homepage and the top of the about page.
3. `_pages/about.md` reuses the intro and adds a bit more content about yourself.
4. `_posts` is the default Jekyll collection of blog posts. Each post has a list of tags. These lists are combined into a tag cloud on the post list page.
5. `_projects` is a directory of project pages. These are not organised into a collection. Each page can hold a description or documentation about a hobby or open-source project.1. `_pages/index.md` - this is the default home page.
2. `_includes/components/intro.md` - this chunk is reused between the top of the homepage and the top of the about page.
3. `_pages/about.md` reuses the intro and adds a bit more content about yourself.
4. `_posts` is the default Jekyll collection of blog posts. Each post has a list of tags. These lists are combined into a tag cloud on the post list page.
5. `_projects` is a directory of project pages. These are not organised into a collection. Each page can hold a description or documentation about a hobby or open-source project.1. `_pages/index.md` - this is the default home page.
2. `_includes/components/intro.md` - this chunk is reused between the top of the homepage and the top of the about page.
3. `_pages/about.md` reuses the intro and adds a bit more content about yourself.
4. `_posts` is the default Jekyll collection of blog posts. Each post has a list of tags. These lists are combined into a tag cloud on the post list page.
5. `_projects` is a directory of project pages. These are not organised into a collection. Each page can hold a description or documentation about a hobby or open-source project.1. `_pages/index.md` - this is the default home page.
2. `_includes/components/intro.md` - this chunk is reused between the top of the homepage and the top of the about page.
3. `_pages/about.md` reuses the intro and adds a bit more content about yourself.
4. `_posts` is the default Jekyll collection of blog posts. Each post has a list of tags. These lists are combined into a tag cloud on the post list page.
5. `_projects` is a directory of project pages. These are not organised into a collection. Each page can hold a description or documentation about a hobby or open-source project.1. `_pages/index.md` - this is the default home page.
2. `_includes/components/intro.md` - this chunk is reused between the top of the homepage and the top of the about page.
3. `_pages/about.md` reuses the intro and adds a bit more content about yourself.
4. `_posts` is the default Jekyll collection of blog posts. Each post has a list of tags. These lists are combined into a tag cloud on the post list page.
5. `_projects` is a directory of project pages. These are not organised into a collection. Each page can hold a description or documentation about a hobby or open-source project.1. `_pages/index.md` - this is the default home page.
2. `_includes/components/intro.md` - this chunk is reused between the top of the homepage and the top of the about page.
3. `_pages/about.md` reuses the intro and adds a bit more content about yourself.
4. `_posts` is the default Jekyll collection of blog posts. Each post has a list of tags. These lists are combined into a tag cloud on the post list page.
5. `_projects` is a directory of project pages. These are not organised into a collection. Each page can hold a description or documentation about a hobby or open-source project.1. `_pages/index.md` - this is the default home page.
2. `_includes/components/intro.md` - this chunk is reused between the top of the homepage and the top of the about page.
3. `_pages/about.md` reuses the intro and adds a bit more content about yourself.
4. `_posts` is the default Jekyll collection of blog posts. Each post has a list of tags. These lists are combined into a tag cloud on the post list page.
5. `_projects` is a directory of project pages. These are not organised into a collection. Each page can hold a description or documentation about a hobby or open-source project.1. `_pages/index.md` - this is the default home page.
2. `_includes/components/intro.md` - this chunk is reused between the top of the homepage and the top of the about page.
3. `_pages/about.md` reuses the intro and adds a bit more content about yourself.
4. `_posts` is the default Jekyll collection of blog posts. Each post has a list of tags. These lists are combined into a tag cloud on the post list page.
5. `_projects` is a directory of project pages. These are not organised into a collection. Each page can hold a description or documentation about a hobby or open-source project.1. `_pages/index.md` - this is the default home page.
2. `_includes/components/intro.md` - this chunk is reused between the top of the homepage and the top of the about page.
3. `_pages/about.md` reuses the intro and adds a bit more content about yourself.
4. `_posts` is the default Jekyll collection of blog posts. Each post has a list of tags. These lists are combined into a tag cloud on the post list page.
5. `_projects` is a directory of project pages. These are not organised into a collection. Each page can hold a description or documentation about a hobby or open-source project.1. `_pages/index.md` - this is the default home page.
2. `_includes/components/intro.md` - this chunk is reused between the top of the homepage and the top of the about page.
3. `_pages/about.md` reuses the intro and adds a bit more content about yourself.
4. `_posts` is the default Jekyll collection of blog posts. Each post has a list of tags. These lists are combined into a tag cloud on the post list page.
5. `_projects` is a directory of project pages. These are not organised into a collection. Each page can hold a description or documentation about a hobby or open-source project.1. `_pages/index.md` - this is the default home page.
2. `_includes/components/intro.md` - this chunk is reused between the top of the homepage and the top of the about page.
3. `_pages/about.md` reuses the intro and adds a bit more content about yourself.
4. `_posts` is the default Jekyll collection of blog posts. Each post has a list of tags. These lists are combined into a tag cloud on the post list page.
5. `_projects` is a directory of project pages. These are not organised into a collection. Each page can hold a description or documentation about a hobby or open-source project.1. `_pages/index.md` - this is the default home page.
2. `_includes/components/intro.md` - this chunk is reused between the top of the homepage and the top of the about page.
3. `_pages/about.md` reuses the intro and adds a bit more content about yourself.
4. `_posts` is the default Jekyll collection of blog posts. Each post has a list of tags. These lists are combined into a tag cloud on the post list page.
5. `_projects` is a directory of project pages. These are not organised into a collection. Each page can hold a description or documentation about a hobby or open-source project.1. `_pages/index.md` - this is the default home page.
2. `_includes/components/intro.md` - this chunk is reused between the top of the homepage and the top of the about page.
3. `_pages/about.md` reuses the intro and adds a bit more content about yourself.
4. `_posts` is the default Jekyll collection of blog posts. Each post has a list of tags. These lists are combined into a tag cloud on the post list page.
5. `_projects` is a directory of project pages. These are not organised into a collection. Each page can hold a description or documentation about a hobby or open-source project.1. `_pages/index.md` - this is the default home page.
2. `_includes/components/intro.md` - this chunk is reused between the top of the homepage and the top of the about page.
3. `_pages/about.md` reuses the intro and adds a bit more content about yourself.
4. `_posts` is the default Jekyll collection of blog posts. Each post has a list of tags. These lists are combined into a tag cloud on the post list page.
5. `_projects` is a directory of project pages. These are not organised into a collection. Each page can hold a description or documentation about a hobby or open-source project.1. `_pages/index.md` - this is the default home page.
2. `_includes/components/intro.md` - this chunk is reused between the top of the homepage and the top of the about page.
3. `_pages/about.md` reuses the intro and adds a bit more content about yourself.
4. `_posts` is the default Jekyll collection of blog posts. Each post has a list of tags. These lists are combined into a tag cloud on the post list page.
5. `_projects` is a directory of project pages. These are not organised into a collection. Each page can hold a description or documentation about a hobby or open-source project.1. `_pages/index.md` - this is the default home page.
2. `_includes/components/intro.md` - this chunk is reused between the top of the homepage and the top of the about page.
3. `_pages/about.md` reuses the intro and adds a bit more content about yourself.
4. `_posts` is the default Jekyll collection of blog posts. Each post has a list of tags. These lists are combined into a tag cloud on the post list page.
5. `_projects` is a directory of project pages. These are not organised into a collection. Each page can hold a description or documentation about a hobby or open-source project.1. `_pages/index.md` - this is the default home page.
2. `_includes/components/intro.md` - this chunk is reused between the top of the homepage and the top of the about page.
3. `_pages/about.md` reuses the intro and adds a bit more content about yourself.
4. `_posts` is the default Jekyll collection of blog posts. Each post has a list of tags. These lists are combined into a tag cloud on the post list page.
5. `_projects` is a directory of project pages. These are not organised into a collection. Each page can hold a description or documentation about a hobby or open-source project.1. `_pages/index.md` - this is the default home page.
2. `_includes/components/intro.md` - this chunk is reused between the top of the homepage and the top of the about page.
3. `_pages/about.md` reuses the intro and adds a bit more content about yourself.
4. `_posts` is the default Jekyll collection of blog posts. Each post has a list of tags. These lists are combined into a tag cloud on the post list page.
5. `_projects` is a directory of project pages. These are not organised into a collection. Each page can hold a description or documentation about a hobby or open-source project.1. `_pages/index.md` - this is the default home page.
2. `_includes/components/intro.md` - this chunk is reused between the top of the homepage and the top of the about page.
3. `_pages/about.md` reuses the intro and adds a bit more content about yourself.
4. `_posts` is the default Jekyll collection of blog posts. Each post has a list of tags. These lists are combined into a tag cloud on the post list page.
5. `_projects` is a directory of project pages. These are not organised into a collection. Each page can hold a description or documentation about a hobby or open-source project.1. `_pages/index.md` - this is the default home page.
2. `_includes/components/intro.md` - this chunk is reused between the top of the homepage and the top of the about page.
3. `_pages/about.md` reuses the intro and adds a bit more content about yourself.
4. `_posts` is the default Jekyll collection of blog posts. Each post has a list of tags. These lists are combined into a tag cloud on the post list page.
5. `_projects` is a directory of project pages. These are not organised into a collection. Each page can hold a description or documentation about a hobby or open-source project.1. `_pages/index.md` - this is the default home page.
2. `_includes/components/intro.md` - this chunk is reused between the top of the homepage and the top of the about page.
3. `_pages/about.md` reuses the intro and adds a bit more content about yourself.
4. `_posts` is the default Jekyll collection of blog posts. Each post has a list of tags. These lists are combined into a tag cloud on the post list page.
5. `_projects` is a directory of project pages. These are not organised into a collection. Each page can hold a description or documentation about a hobby or open-source project.1. `_pages/index.md` - this is the default home page.
2. `_includes/components/intro.md` - this chunk is reused between the top of the homepage and the top of the about page.
3. `_pages/about.md` reuses the intro and adds a bit more content about yourself.
4. `_posts` is the default Jekyll collection of blog posts. Each post has a list of tags. These lists are combined into a tag cloud on the post list page.
5. `_projects` is a directory of project pages. These are not organised into a collection. Each page can hold a description or documentation about a hobby or open-source project.1. `_pages/index.md` - this is the default home page.
2. `_includes/components/intro.md` - this chunk is reused between the top of the homepage and the top of the about page.
3. `_pages/about.md` reuses the intro and adds a bit more content about yourself.
4. `_posts` is the default Jekyll collection of blog posts. Each post has a list of tags. These lists are combined into a tag cloud on the post list page.
5. `_projects` is a directory of project pages. These are not organised into a collection. Each page can hold a description or documentation about a hobby or open-source project.1. `_pages/index.md` - this is the default home page.
2. `_includes/components/intro.md` - this chunk is reused between the top of the homepage and the top of the about page.
3. `_pages/about.md` reuses the intro and adds a bit more content about yourself.
4. `_posts` is the default Jekyll collection of blog posts. Each post has a list of tags. These lists are combined into a tag cloud on the post list page.
5. `_projects` is a directory of project pages. These are not organised into a collection. Each page can hold a description or documentation about a hobby or open-source project.1. `_pages/index.md` - this is the default home page.
2. `_includes/components/intro.md` - this chunk is reused between the top of the homepage and the top of the about page.
3. `_pages/about.md` reuses the intro and adds a bit more content about yourself.
4. `_posts` is the default Jekyll collection of blog posts. Each post has a list of tags. These lists are combined into a tag cloud on the post list page.
5. `_projects` is a directory of project pages. These are not organised into a collection. Each page can hold a description or documentation about a hobby or open-source project.1. `_pages/index.md` - this is the default home page.
2. `_includes/components/intro.md` - this chunk is reused between the top of the homepage and the top of the about page.
3. `_pages/about.md` reuses the intro and adds a bit more content about yourself.
4. `_posts` is the default Jekyll collection of blog posts. Each post has a list of tags. These lists are combined into a tag cloud on the post list page.
5. `_projects` is a directory of project pages. These are not organised into a collection. Each page can hold a description or documentation about a hobby or open-source project.1. `_pages/index.md` - this is the default home page.
2. `_includes/components/intro.md` - this chunk is reused between the top of the homepage and the top of the about page.
3. `_pages/about.md` reuses the intro and adds a bit more content about yourself.
4. `_posts` is the default Jekyll collection of blog posts. Each post has a list of tags. These lists are combined into a tag cloud on the post list page.
5. `_projects` is a directory of project pages. These are not organised into a collection. Each page can hold a description or documentation about a hobby or open-source project.1. `_pages/index.md` - this is the default home page.
2. `_includes/components/intro.md` - this chunk is reused between the top of the homepage and the top of the about page.
3. `_pages/about.md` reuses the intro and adds a bit more content about yourself.
4. `_posts` is the default Jekyll collection of blog posts. Each post has a list of tags. These lists are combined into a tag cloud on the post list page.
5. `_projects` is a directory of project pages. These are not organised into a collection. Each page can hold a description or documentation about a hobby or open-source project.1. `_pages/index.md` - this is the default home page.
2. `_includes/components/intro.md` - this chunk is reused between the top of the homepage and the top of the about page.
3. `_pages/about.md` reuses the intro and adds a bit more content about yourself.
4. `_posts` is the default Jekyll collection of blog posts. Each post has a list of tags. These lists are combined into a tag cloud on the post list page.
5. `_projects` is a directory of project pages. These are not organised into a collection. Each page can hold a description or documentation about a hobby or open-source project.1. `_pages/index.md` - this is the default home page.
2. `_includes/components/intro.md` - this chunk is reused between the top of the homepage and the top of the about page.
3. `_pages/about.md` reuses the intro and adds a bit more content about yourself.
4. `_posts` is the default Jekyll collection of blog posts. Each post has a list of tags. These lists are combined into a tag cloud on the post list page.
5. `_projects` is a directory of project pages. These are not organised into a collection. Each page can hold a description or documentation about a hobby or open-source project.1. `_pages/index.md` - this is the default home page.
2. `_includes/components/intro.md` - this chunk is reused between the top of the homepage and the top of the about page.
3. `_pages/about.md` reuses the intro and adds a bit more content about yourself.
4. `_posts` is the default Jekyll collection of blog posts. Each post has a list of tags. These lists are combined into a tag cloud on the post list page.
5. `_projects` is a directory of project pages. These are not organised into a collection. Each page can hold a description or documentation about a hobby or open-source project.1. `_pages/index.md` - this is the default home page.
2. `_includes/components/intro.md` - this chunk is reused between the top of the homepage and the top of the about page.
3. `_pages/about.md` reuses the intro and adds a bit more content about yourself.
4. `_posts` is the default Jekyll collection of blog posts. Each post has a list of tags. These lists are combined into a tag cloud on the post list page.
5. `_projects` is a directory of project pages. These are not organised into a collection. Each page can hold a description or documentation about a hobby or open-source project.1. `_pages/index.md` - this is the default home page.
2. `_includes/components/intro.md` - this chunk is reused between the top of the homepage and the top of the about page.
3. `_pages/about.md` reuses the intro and adds a bit more content about yourself.
4. `_posts` is the default Jekyll collection of blog posts. Each post has a list of tags. These lists are combined into a tag cloud on the post list page.
5. `_projects` is a directory of project pages. These are not organised into a collection. Each page can hold a description or documentation about a hobby or open-source project.1. `_pages/index.md` - this is the default home page.
2. `_includes/components/intro.md` - this chunk is reused between the top of the homepage and the top of the about page.
3. `_pages/about.md` reuses the intro and adds a bit more content about yourself.
4. `_posts` is the default Jekyll collection of blog posts. Each post has a list of tags. These lists are combined into a tag cloud on the post list page.
5. `_projects` is a directory of project pages. These are not organised into a collection. Each page can hold a description or documentation about a hobby or open-source project.1. `_pages/index.md` - this is the default home page.
2. `_includes/components/intro.md` - this chunk is reused between the top of the homepage and the top of the about page.
3. `_pages/about.md` reuses the intro and adds a bit more content about yourself.
4. `_posts` is the default Jekyll collection of blog posts. Each post has a list of tags. These lists are combined into a tag cloud on the post list page.
5. `_projects` is a directory of project pages. These are not organised into a collection. Each page can hold a description or documentation about a hobby or open-source project.1. `_pages/index.md` - this is the default home page.
2. `_includes/components/intro.md` - this chunk is reused between the top of the homepage and the top of the about page.
3. `_pages/about.md` reuses the intro and adds a bit more content about yourself.
4. `_posts` is the default Jekyll collection of blog posts. Each post has a list of tags. These lists are combined into a tag cloud on the post list page.
5. `_projects` is a directory of project pages. These are not organised into a collection. Each page can hold a description or documentation about a hobby or open-source project.1. `_pages/index.md` - this is the default home page.
2. `_includes/components/intro.md` - this chunk is reused between the top of the homepage and the top of the about page.
3. `_pages/about.md` reuses the intro and adds a bit more content about yourself.
4. `_posts` is the default Jekyll collection of blog posts. Each post has a list of tags. These lists are combined into a tag cloud on the post list page.
5. `_projects` is a directory of project pages. These are not organised into a collection. Each page can hold a description or documentation about a hobby or open-source project.1. `_pages/index.md` - this is the default home page.
2. `_includes/components/intro.md` - this chunk is reused between the top of the homepage and the top of the about page.
3. `_pages/about.md` reuses the intro and adds a bit more content about yourself.
4. `_posts` is the default Jekyll collection of blog posts. Each post has a list of tags. These lists are combined into a tag cloud on the post list page.
5. `_projects` is a directory of project pages. These are not organised into a collection. Each page can hold a description or documentation about a hobby or open-source project.1. `_pages/index.md` - this is the default home page.
2. `_includes/components/intro.md` - this chunk is reused between the top of the homepage and the top of the about page.
3. `_pages/about.md` reuses the intro and adds a bit more content about yourself.
4. `_posts` is the default Jekyll collection of blog posts. Each post has a list of tags. These lists are combined into a tag cloud on the post list page.
5. `_projects` is a directory of project pages. These are not organised into a collection. Each page can hold a description or documentation about a hobby or open-source project.1. `_pages/index.md` - this is the default home page.
2. `_includes/components/intro.md` - this chunk is reused between the top of the homepage and the top of the about page.
3. `_pages/about.md` reuses the intro and adds a bit more content about yourself.
4. `_posts` is the default Jekyll collection of blog posts. Each post has a list of tags. These lists are combined into a tag cloud on the post list page.
5. `_projects` is a directory of project pages. These are not organised into a collection. Each page can hold a description or documentation about a hobby or open-source project.1. `_pages/index.md` - this is the default home page.
2. `_includes/components/intro.md` - this chunk is reused between the top of the homepage and the top of the about page.
3. `_pages/about.md` reuses the intro and adds a bit more content about yourself.
4. `_posts` is the default Jekyll collection of blog posts. Each post has a list of tags. These lists are combined into a tag cloud on the post list page.
5. `_projects` is a directory of project pages. These are not organised into a collection. Each page can hold a description or documentation about a hobby or open-source project.1. `_pages/index.md` - this is the default home page.
2. `_includes/components/intro.md` - this chunk is reused between the top of the homepage and the top of the about page.
3. `_pages/about.md` reuses the intro and adds a bit more content about yourself.
4. `_posts` is the default Jekyll collection of blog posts. Each post has a list of tags. These lists are combined into a tag cloud on the post list page.
5. `_projects` is a directory of project pages. These are not organised into a collection. Each page can hold a description or documentation about a hobby or open-source project.1. `_pages/index.md` - this is the default home page.
2. `_includes/components/intro.md` - this chunk is reused between the top of the homepage and the top of the about page.
3. `_pages/about.md` reuses the intro and adds a bit more content about yourself.
4. `_posts` is the default Jekyll collection of blog posts. Each post has a list of tags. These lists are combined into a tag cloud on the post list page.
5. `_projects` is a directory of project pages. These are not organised into a collection. Each page can hold a description or documentation about a hobby or open-source project.1. `_pages/index.md` - this is the default home page.
2. `_includes/components/intro.md` - this chunk is reused between the top of the homepage and the top of the about page.
3. `_pages/about.md` reuses the intro and adds a bit more content about yourself.
4. `_posts` is the default Jekyll collection of blog posts. Each post has a list of tags. These lists are combined into a tag cloud on the post list page.
5. `_projects` is a directory of project pages. These are not organised into a collection. Each page can hold a description or documentation about a hobby or open-source project.1. `_pages/index.md` - this is the default home page.
2. `_includes/components/intro.md` - this chunk is reused between the top of the homepage and the top of the about page.
3. `_pages/about.md` reuses the intro and adds a bit more content about yourself.
4. `_posts` is the default Jekyll collection of blog posts. Each post has a list of tags. These lists are combined into a tag cloud on the post list page.
5. `_projects` is a directory of project pages. These are not organised into a collection. Each page can hold a description or documentation about a hobby or open-source project.1. `_pages/index.md` - this is the default home page.
2. `_includes/components/intro.md` - this chunk is reused between the top of the homepage and the top of the about page.
3. `_pages/about.md` reuses the intro and adds a bit more content about yourself.
4. `_posts` is the default Jekyll collection of blog posts. Each post has a list of tags. These lists are combined into a tag cloud on the post list page.
5. `_projects` is a directory of project pages. These are not organised into a collection. Each page can hold a description or documentation about a hobby or open-source project.1. `_pages/index.md` - this is the default home page.
2. `_includes/components/intro.md` - this chunk is reused between the top of the homepage and the top of the about page.
3. `_pages/about.md` reuses the intro and adds a bit more content about yourself.
4. `_posts` is the default Jekyll collection of blog posts. Each post has a list of tags. These lists are combined into a tag cloud on the post list page.
5. `_projects` is a directory of project pages. These are not organised into a collection. Each page can hold a description or documentation about a hobby or open-source project.1. `_pages/index.md` - this is the default home page.
2. `_includes/components/intro.md` - this chunk is reused between the top of the homepage and the top of the about page.
3. `_pages/about.md` reuses the intro and adds a bit more content about yourself.
4. `_posts` is the default Jekyll collection of blog posts. Each post has a list of tags. These lists are combined into a tag cloud on the post list page.
5. `_projects` is a directory of project pages. These are not organised into a collection. Each page can hold a description or documentation about a hobby or open-source project.1. `_pages/index.md` - this is the default home page.
2. `_includes/components/intro.md` - this chunk is reused between the top of the homepage and the top of the about page.
3. `_pages/about.md` reuses the intro and adds a bit more content about yourself.
4. `_posts` is the default Jekyll collection of blog posts. Each post has a list of tags. These lists are combined into a tag cloud on the post list page.
5. `_projects` is a directory of project pages. These are not organised into a collection. Each page can hold a description or documentation about a hobby or open-source project.1. `_pages/index.md` - this is the default home page.
2. `_includes/components/intro.md` - this chunk is reused between the top of the homepage and the top of the about page.
3. `_pages/about.md` reuses the intro and adds a bit more content about yourself.
4. `_posts` is the default Jekyll collection of blog posts. Each post has a list of tags. These lists are combined into a tag cloud on the post list page.
5. `_projects` is a directory of project pages. These are not organised into a collection. Each page can hold a description or documentation about a hobby or open-source project.1. `_pages/index.md` - this is the default home page.
2. `_includes/components/intro.md` - this chunk is reused between the top of the homepage and the top of the about page.
3. `_pages/about.md` reuses the intro and adds a bit more content about yourself.
4. `_posts` is the default Jekyll collection of blog posts. Each post has a list of tags. These lists are combined into a tag cloud on the post list page.
5. `_projects` is a directory of project pages. These are not organised into a collection. Each page can hold a description or documentation about a hobby or open-source project.1. `_pages/index.md` - this is the default home page.
2. `_includes/components/intro.md` - this chunk is reused between the top of the homepage and the top of the about page.
3. `_pages/about.md` reuses the intro and adds a bit more content about yourself.
4. `_posts` is the default Jekyll collection of blog posts. Each post has a list of tags. These lists are combined into a tag cloud on the post list page.
5. `_projects` is a directory of project pages. These are not organised into a collection. Each page can hold a description or documentation about a hobby or open-source project.1. `_pages/index.md` - this is the default home page.
2. `_includes/components/intro.md` - this chunk is reused between the top of the homepage and the top of the about page.
3. `_pages/about.md` reuses the intro and adds a bit more content about yourself.
4. `_posts` is the default Jekyll collection of blog posts. Each post has a list of tags. These lists are combined into a tag cloud on the post list page.
5. `_projects` is a directory of project pages. These are not organised into a collection. Each page can hold a description or documentation about a hobby or open-source project.1. `_pages/index.md` - this is the default home page.
2. `_includes/components/intro.md` - this chunk is reused between the top of the homepage and the top of the about page.
3. `_pages/about.md` reuses the intro and adds a bit more content about yourself.
4. `_posts` is the default Jekyll collection of blog posts. Each post has a list of tags. These lists are combined into a tag cloud on the post list page.
5. `_projects` is a directory of project pages. These are not organised into a collection. Each page can hold a description or documentation about a hobby or open-source project.1. `_pages/index.md` - this is the default home page.
2. `_includes/components/intro.md` - this chunk is reused between the top of the homepage and the top of the about page.
3. `_pages/about.md` reuses the intro and adds a bit more content about yourself.
4. `_posts` is the default Jekyll collection of blog posts. Each post has a list of tags. These lists are combined into a tag cloud on the post list page.
5. `_projects` is a directory of project pages. These are not organised into a collection. Each page can hold a description or documentation about a hobby or open-source project.1. `_pages/index.md` - this is the default home page.
2. `_includes/components/intro.md` - this chunk is reused between the top of the homepage and the top of the about page.
3. `_pages/about.md` reuses the intro and adds a bit more content about yourself.
4. `_posts` is the default Jekyll collection of blog posts. Each post has a list of tags. These lists are combined into a tag cloud on the post list page.
5. `_projects` is a directory of project pages. These are not organised into a collection. Each page can hold a description or documentation about a hobby or open-source project.1. `_pages/index.md` - this is the default home page.
2. `_includes/components/intro.md` - this chunk is reused between the top of the homepage and the top of the about page.
3. `_pages/about.md` reuses the intro and adds a bit more content about yourself.
4. `_posts` is the default Jekyll collection of blog posts. Each post has a list of tags. These lists are combined into a tag cloud on the post list page.
5. `_projects` is a directory of project pages. These are not organised into a collection. Each page can hold a description or documentation about a hobby or open-source project.1. `_pages/index.md` - this is the default home page.
2. `_includes/components/intro.md` - this chunk is reused between the top of the homepage and the top of the about page.
3. `_pages/about.md` reuses the intro and adds a bit more content about yourself.
4. `_posts` is the default Jekyll collection of blog posts. Each post has a list of tags. These lists are combined into a tag cloud on the post list page.
5. `_projects` is a directory of project pages. These are not organised into a collection. Each page can hold a description or documentation about a hobby or open-source project.1. `_pages/index.md` - this is the default home page.
2. `_includes/components/intro.md` - this chunk is reused between the top of the homepage and the top of the about page.
3. `_pages/about.md` reuses the intro and adds a bit more content about yourself.
4. `_posts` is the default Jekyll collection of blog posts. Each post has a list of tags. These lists are combined into a tag cloud on the post list page.
5. `_projects` is a directory of project pages. These are not organised into a collection. Each page can hold a description or documentation about a hobby or open-source project.1. `_pages/index.md` - this is the default home page.
2. `_includes/components/intro.md` - this chunk is reused between the top of the homepage and the top of the about page.
3. `_pages/about.md` reuses the intro and adds a bit more content about yourself.
4. `_posts` is the default Jekyll collection of blog posts. Each post has a list of tags. These lists are combined into a tag cloud on the post list page.
5. `_projects` is a directory of project pages. These are not organised into a collection. Each page can hold a description or documentation about a hobby or open-source project.1. `_pages/index.md` - this is the default home page.
2. `_includes/components/intro.md` - this chunk is reused between the top of the homepage and the top of the about page.
3. `_pages/about.md` reuses the intro and adds a bit more content about yourself.
4. `_posts` is the default Jekyll collection of blog posts. Each post has a list of tags. These lists are combined into a tag cloud on the post list page.
5. `_projects` is a directory of project pages. These are not organised into a collection. Each page can hold a description or documentation about a hobby or open-source project.1. `_pages/index.md` - this is the default home page.
2. `_includes/components/intro.md` - this chunk is reused between the top of the homepage and the top of the about page.
3. `_pages/about.md` reuses the intro and adds a bit more content about yourself.
4. `_posts` is the default Jekyll collection of blog posts. Each post has a list of tags. These lists are combined into a tag cloud on the post list page.
5. `_projects` is a directory of project pages. These are not organised into a collection. Each page can hold a description or documentation about a hobby or open-source project.1. `_pages/index.md` - this is the default home page.
2. `_includes/components/intro.md` - this chunk is reused between the top of the homepage and the top of the about page.
3. `_pages/about.md` reuses the intro and adds a bit more content about yourself.
4. `_posts` is the default Jekyll collection of blog posts. Each post has a list of tags. These lists are combined into a tag cloud on the post list page.
5. `_projects` is a directory of project pages. These are not organised into a collection. Each page can hold a description or documentation about a hobby or open-source project.1. `_pages/index.md` - this is the default home page.
2. `_includes/components/intro.md` - this chunk is reused between the top of the homepage and the top of the about page.
3. `_pages/about.md` reuses the intro and adds a bit more content about yourself.
4. `_posts` is the default Jekyll collection of blog posts. Each post has a list of tags. These lists are combined into a tag cloud on the post list page.
5. `_projects` is a directory of project pages. These are not organised into a collection. Each page can hold a description or documentation about a hobby or open-source project.1. `_pages/index.md` - this is the default home page.
2. `_includes/components/intro.md` - this chunk is reused between the top of the homepage and the top of the about page.
3. `_pages/about.md` reuses the intro and adds a bit more content about yourself.
4. `_posts` is the default Jekyll collection of blog posts. Each post has a list of tags. These lists are combined into a tag cloud on the post list page.
5. `_projects` is a directory of project pages. These are not organised into a collection. Each page can hold a description or documentation about a hobby or open-source project.1. `_pages/index.md` - this is the default home page.
2. `_includes/components/intro.md` - this chunk is reused between the top of the homepage and the top of the about page.
3. `_pages/about.md` reuses the intro and adds a bit more content about yourself.
4. `_posts` is the default Jekyll collection of blog posts. Each post has a list of tags. These lists are combined into a tag cloud on the post list page.
5. `_projects` is a directory of project pages. These are not organised into a collection. Each page can hold a description or documentation about a hobby or open-source project.1. `_pages/index.md` - this is the default home page.
2. `_includes/components/intro.md` - this chunk is reused between the top of the homepage and the top of the about page.
3. `_pages/about.md` reuses the intro and adds a bit more content about yourself.
4. `_posts` is the default Jekyll collection of blog posts. Each post has a list of tags. These lists are combined into a tag cloud on the post list page.
5. `_projects` is a directory of project pages. These are not organised into a collection. Each page can hold a description or documentation about a hobby or open-source project.1. `_pages/index.md` - this is the default home page.
2. `_includes/components/intro.md` - this chunk is reused between the top of the homepage and the top of the about page.
3. `_pages/about.md` reuses the intro and adds a bit more content about yourself.
4. `_posts` is the default Jekyll collection of blog posts. Each post has a list of tags. These lists are combined into a tag cloud on the post list page.
5. `_projects` is a directory of project pages. These are not organised into a collection. Each page can hold a description or documentation about a hobby or open-source project.1. `_pages/index.md` - this is the default home page.
2. `_includes/components/intro.md` - this chunk is reused between the top of the homepage and the top of the about page.
3. `_pages/about.md` reuses the intro and adds a bit more content about yourself.
4. `_posts` is the default Jekyll collection of blog posts. Each post has a list of tags. These lists are combined into a tag cloud on the post list page.
5. `_projects` is a directory of project pages. These are not organised into a collection. Each page can hold a description or documentation about a hobby or open-source project.1. `_pages/index.md` - this is the default home page.
2. `_includes/components/intro.md` - this chunk is reused between the top of the homepage and the top of the about page.
3. `_pages/about.md` reuses the intro and adds a bit more content about yourself.
4. `_posts` is the default Jekyll collection of blog posts. Each post has a list of tags. These lists are combined into a tag cloud on the post list page.
5. `_projects` is a directory of project pages. These are not organised into a collection. Each page can hold a description or documentation about a hobby or open-source project.1. `_pages/index.md` - this is the default home page.
2. `_includes/components/intro.md` - this chunk is reused between the top of the homepage and the top of the about page.
3. `_pages/about.md` reuses the intro and adds a bit more content about yourself.
4. `_posts` is the default Jekyll collection of blog posts. Each post has a list of tags. These lists are combined into a tag cloud on the post list page.
5. `_projects` is a directory of project pages. These are not organised into a collection. Each page can hold a description or documentation about a hobby or open-source project.1. `_pages/index.md` - this is the default home page.
2. `_includes/components/intro.md` - this chunk is reused between the top of the homepage and the top of the about page.
3. `_pages/about.md` reuses the intro and adds a bit more content about yourself.
4. `_posts` is the default Jekyll collection of blog posts. Each post has a list of tags. These lists are combined into a tag cloud on the post list page.
5. `_projects` is a directory of project pages. These are not organised into a collection. Each page can hold a description or documentation about a hobby or open-source project.1. `_pages/index.md` - this is the default home page.
2. `_includes/components/intro.md` - this chunk is reused between the top of the homepage and the top of the about page.
3. `_pages/about.md` reuses the intro and adds a bit more content about yourself.
4. `_posts` is the default Jekyll collection of blog posts. Each post has a list of tags. These lists are combined into a tag cloud on the post list page.
5. `_projects` is a directory of project pages. These are not organised into a collection. Each page can hold a description or documentation about a hobby or open-source project.1. `_pages/index.md` - this is the default home page.
2. `_includes/components/intro.md` - this chunk is reused between the top of the homepage and the top of the about page.
3. `_pages/about.md` reuses the intro and adds a bit more content about yourself.
4. `_posts` is the default Jekyll collection of blog posts. Each post has a list of tags. These lists are combined into a tag cloud on the post list page.
5. `_projects` is a directory of project pages. These are not organised into a collection. Each page can hold a description or documentation about a hobby or open-source project.1. `_pages/index.md` - this is the default home page.
2. `_includes/components/intro.md` - this chunk is reused between the top of the homepage and the top of the about page.
3. `_pages/about.md` reuses the intro and adds a bit more content about yourself.
4. `_posts` is the default Jekyll collection of blog posts. Each post has a list of tags. These lists are combined into a tag cloud on the post list page.
5. `_projects` is a directory of project pages. These are not organised into a collection. Each page can hold a description or documentation about a hobby or open-source project.1. `_pages/index.md` - this is the default home page.
2. `_includes/components/intro.md` - this chunk is reused between the top of the homepage and the top of the about page.
3. `_pages/about.md` reuses the intro and adds a bit more content about yourself.
4. `_posts` is the default Jekyll collection of blog posts. Each post has a list of tags. These lists are combined into a tag cloud on the post list page.
5. `_projects` is a directory of project pages. These are not organised into a collection. Each page can hold a description or documentation about a hobby or open-source project.1. `_pages/index.md` - this is the default home page.
2. `_includes/components/intro.md` - this chunk is reused between the top of the homepage and the top of the about page.
3. `_pages/about.md` reuses the intro and adds a bit more content about yourself.
4. `_posts` is the default Jekyll collection of blog posts. Each post has a list of tags. These lists are combined into a tag cloud on the post list page.
5. `_projects` is a directory of project pages. These are not organised into a collection. Each page can hold a description or documentation about a hobby or open-source project.1. `_pages/index.md` - this is the default home page.
2. `_includes/components/intro.md` - this chunk is reused between the top of the homepage and the top of the about page.
3. `_pages/about.md` reuses the intro and adds a bit more content about yourself.
4. `_posts` is the default Jekyll collection of blog posts. Each post has a list of tags. These lists are combined into a tag cloud on the post list page.
5. `_projects` is a directory of project pages. These are not organised into a collection. Each page can hold a description or documentation about a hobby or open-source project.1. `_pages/index.md` - this is the default home page.
2. `_includes/components/intro.md` - this chunk is reused between the top of the homepage and the top of the about page.
3. `_pages/about.md` reuses the intro and adds a bit more content about yourself.
4. `_posts` is the default Jekyll collection of blog posts. Each post has a list of tags. These lists are combined into a tag cloud on the post list page.
5. `_projects` is a directory of project pages. These are not organised into a collection. Each page can hold a description or documentation about a hobby or open-source project.1. `_pages/index.md` - this is the default home page.
2. `_includes/components/intro.md` - this chunk is reused between the top of the homepage and the top of the about page.
3. `_pages/about.md` reuses the intro and adds a bit more content about yourself.
4. `_posts` is the default Jekyll collection of blog posts. Each post has a list of tags. These lists are combined into a tag cloud on the post list page.
5. `_projects` is a directory of project pages. These are not organised into a collection. Each page can hold a description or documentation about a hobby or open-source project.1. `_pages/index.md` - this is the default home page.
2. `_includes/components/intro.md` - this chunk is reused between the top of the homepage and the top of the about page.
3. `_pages/about.md` reuses the intro and adds a bit more content about yourself.
4. `_posts` is the default Jekyll collection of blog posts. Each post has a list of tags. These lists are combined into a tag cloud on the post list page.
5. `_projects` is a directory of project pages. These are not organised into a collection. Each page can hold a description or documentation about a hobby or open-source project.1. `_pages/index.md` - this is the default home page.
2. `_includes/components/intro.md` - this chunk is reused between the top of the homepage and the top of the about page.
3. `_pages/about.md` reuses the intro and adds a bit more content about yourself.
4. `_posts` is the default Jekyll collection of blog posts. Each post has a list of tags. These lists are combined into a tag cloud on the post list page.
5. `_projects` is a directory of project pages. These are not organised into a collection. Each page can hold a description or documentation about a hobby or open-source project.1. `_pages/index.md` - this is the default home page.
2. `_includes/components/intro.md` - this chunk is reused between the top of the homepage and the top of the about page.
3. `_pages/about.md` reuses the intro and adds a bit more content about yourself.
4. `_posts` is the default Jekyll collection of blog posts. Each post has a list of tags. These lists are combined into a tag cloud on the post list page.
5. `_projects` is a directory of project pages. These are not organised into a collection. Each page can hold a description or documentation about a hobby or open-source project.1. `_pages/index.md` - this is the default home page.
2. `_includes/components/intro.md` - this chunk is reused between the top of the homepage and the top of the about page.
3. `_pages/about.md` reuses the intro and adds a bit more content about yourself.
4. `_posts` is the default Jekyll collection of blog posts. Each post has a list of tags. These lists are combined into a tag cloud on the post list page.
5. `_projects` is a directory of project pages. These are not organised into a collection. Each page can hold a description or documentation about a hobby or open-source project.1. `_pages/index.md` - this is the default home page.
2. `_includes/components/intro.md` - this chunk is reused between the top of the homepage and the top of the about page.
3. `_pages/about.md` reuses the intro and adds a bit more content about yourself.
4. `_posts` is the default Jekyll collection of blog posts. Each post has a list of tags. These lists are combined into a tag cloud on the post list page.
5. `_projects` is a directory of project pages. These are not organised into a collection. Each page can hold a description or documentation about a hobby or open-source project.1. `_pages/index.md` - this is the default home page.
2. `_includes/components/intro.md` - this chunk is reused between the top of the homepage and the top of the about page.
3. `_pages/about.md` reuses the intro and adds a bit more content about yourself.
4. `_posts` is the default Jekyll collection of blog posts. Each post has a list of tags. These lists are combined into a tag cloud on the post list page.
5. `_projects` is a directory of project pages. These are not organised into a collection. Each page can hold a description or documentation about a hobby or open-source project.1. `_pages/index.md` - this is the default home page.
2. `_includes/components/intro.md` - this chunk is reused between the top of the homepage and the top of the about page.
3. `_pages/about.md` reuses the intro and adds a bit more content about yourself.
4. `_posts` is the default Jekyll collection of blog posts. Each post has a list of tags. These lists are combined into a tag cloud on the post list page.
5. `_projects` is a directory of project pages. These are not organised into a collection. Each page can hold a description or documentation about a hobby or open-source project.1. `_pages/index.md` - this is the default home page.
2. `_includes/components/intro.md` - this chunk is reused between the top of the homepage and the top of the about page.
3. `_pages/about.md` reuses the intro and adds a bit more content about yourself.
4. `_posts` is the default Jekyll collection of blog posts. Each post has a list of tags. These lists are combined into a tag cloud on the post list page.
5. `_projects` is a directory of project pages. These are not organised into a collection. Each page can hold a description or documentation about a hobby or open-source project.1. `_pages/index.md` - this is the default home page.
2. `_includes/components/intro.md` - this chunk is reused between the top of the homepage and the top of the about page.
3. `_pages/about.md` reuses the intro and adds a bit more content about yourself.
4. `_posts` is the default Jekyll collection of blog posts. Each post has a list of tags. These lists are combined into a tag cloud on the post list page.
5. `_projects` is a directory of project pages. These are not organised into a collection. Each page can hold a description or documentation about a hobby or open-source project.1. `_pages/index.md` - this is the default home page.
2. `_includes/components/intro.md` - this chunk is reused between the top of the homepage and the top of the about page.
3. `_pages/about.md` reuses the intro and adds a bit more content about yourself.
4. `_posts` is the default Jekyll collection of blog posts. Each post has a list of tags. These lists are combined into a tag cloud on the post list page.
5. `_projects` is a directory of project pages. These are not organised into a collection. Each page can hold a description or documentation about a hobby or open-source project.1. `_pages/index.md` - this is the default home page.
2. `_includes/components/intro.md` - this chunk is reused between the top of the homepage and the top of the about page.
3. `_pages/about.md` reuses the intro and adds a bit more content about yourself.
4. `_posts` is the default Jekyll collection of blog posts. Each post has a list of tags. These lists are combined into a tag cloud on the post list page.
5. `_projects` is a directory of project pages. These are not organised into a collection. Each page can hold a description or documentation about a hobby or open-source project.1. `_pages/index.md` - this is the default home page.
2. `_includes/components/intro.md` - this chunk is reused between the top of the homepage and the top of the about page.
3. `_pages/about.md` reuses the intro and adds a bit more content about yourself.
4. `_posts` is the default Jekyll collection of blog posts. Each post has a list of tags. These lists are combined into a tag cloud on the post list page.
5. `_projects` is a directory of project pages. These are not organised into a collection. Each page can hold a description or documentation about a hobby or open-source project.1. `_pages/index.md` - this is the default home page.
2. `_includes/components/intro.md` - this chunk is reused between the top of the homepage and the top of the about page.
3. `_pages/about.md` reuses the intro and adds a bit more content about yourself.
4. `_posts` is the default Jekyll collection of blog posts. Each post has a list of tags. These lists are combined into a tag cloud on the post list page.
5. `_projects` is a directory of project pages. These are not organised into a collection. Each page can hold a description or documentation about a hobby or open-source project.1. `_pages/index.md` - this is the default home page.
2. `_includes/components/intro.md` - this chunk is reused between the top of the homepage and the top of the about page.
3. `_pages/about.md` reuses the intro and adds a bit more content about yourself.
4. `_posts` is the default Jekyll collection of blog posts. Each post has a list of tags. These lists are combined into a tag cloud on the post list page.
5. `_projects` is a directory of project pages. These are not organised into a collection. Each page can hold a description or documentation about a hobby or open-source project.1. `_pages/index.md` - this is the default home page.
2. `_includes/components/intro.md` - this chunk is reused between the top of the homepage and the top of the about page.
3. `_pages/about.md` reuses the intro and adds a bit more content about yourself.
4. `_posts` is the default Jekyll collection of blog posts. Each post has a list of tags. These lists are combined into a tag cloud on the post list page.
5. `_projects` is a directory of project pages. These are not organised into a collection. Each page can hold a description or documentation about a hobby or open-source project.1. `_pages/index.md` - this is the default home page.
2. `_includes/components/intro.md` - this chunk is reused between the top of the homepage and the top of the about page.
3. `_pages/about.md` reuses the intro and adds a bit more content about yourself.
4. `_posts` is the default Jekyll collection of blog posts. Each post has a list of tags. These lists are combined into a tag cloud on the post list page.
5. `_projects` is a directory of project pages. These are not organised into a collection. Each page can hold a description or documentation about a hobby or open-source project.1. `_pages/index.md` - this is the default home page.
2. `_includes/components/intro.md` - this chunk is reused between the top of the homepage and the top of the about page.
3. `_pages/about.md` reuses the intro and adds a bit more content about yourself.
4. `_posts` is the default Jekyll collection of blog posts. Each post has a list of tags. These lists are combined into a tag cloud on the post list page.
5. `_projects` is a directory of project pages. These are not organised into a collection. Each page can hold a description or documentation about a hobby or open-source project.1. `_pages/index.md` - this is the default home page.
2. `_includes/components/intro.md` - this chunk is reused between the top of the homepage and the top of the about page.
3. `_pages/about.md` reuses the intro and adds a bit more content about yourself.
4. `_posts` is the default Jekyll collection of blog posts. Each post has a list of tags. These lists are combined into a tag cloud on the post list page.
5. `_projects` is a directory of project pages. These are not organised into a collection. Each page can hold a description or documentation about a hobby or open-source project.1. `_pages/index.md` - this is the default home page.
2. `_includes/components/intro.md` - this chunk is reused between the top of the homepage and the top of the about page.
3. `_pages/about.md` reuses the intro and adds a bit more content about yourself.
4. `_posts` is the default Jekyll collection of blog posts. Each post has a list of tags. These lists are combined into a tag cloud on the post list page.
5. `_projects` is a directory of project pages. These are not organised into a collection. Each page can hold a description or documentation about a hobby or open-source project.1. `_pages/index.md` - this is the default home page.
2. `_includes/components/intro.md` - this chunk is reused between the top of the homepage and the top of the about page.
3. `_pages/about.md` reuses the intro and adds a bit more content about yourself.
4. `_posts` is the default Jekyll collection of blog posts. Each post has a list of tags. These lists are combined into a tag cloud on the post list page.
5. `_projects` is a directory of project pages. These are not organised into a collection. Each page can hold a description or documentation about a hobby or open-source project.1. `_pages/index.md` - this is the default home page.
2. `_includes/components/intro.md` - this chunk is reused between the top of the homepage and the top of the about page.
3. `_pages/about.md` reuses the intro and adds a bit more content about yourself.
4. `_posts` is the default Jekyll collection of blog posts. Each post has a list of tags. These lists are combined into a tag cloud on the post list page.
5. `_projects` is a directory of project pages. These are not organised into a collection. Each page can hold a description or documentation about a hobby or open-source project.1. `_pages/index.md` - this is the default home page.
2. `_includes/components/intro.md` - this chunk is reused between the top of the homepage and the top of the about page.
3. `_pages/about.md` reuses the intro and adds a bit more content about yourself.
4. `_posts` is the default Jekyll collection of blog posts. Each post has a list of tags. These lists are combined into a tag cloud on the post list page.
5. `_projects` is a directory of project pages. These are not organised into a collection. Each page can hold a description or documentation about a hobby or open-source project.1. `_pages/index.md` - this is the default home page.
2. `_includes/components/intro.md` - this chunk is reused between the top of the homepage and the top of the about page.
3. `_pages/about.md` reuses the intro and adds a bit more content about yourself.
4. `_posts` is the default Jekyll collection of blog posts. Each post has a list of tags. These lists are combined into a tag cloud on the post list page.
5. `_projects` is a directory of project pages. These are not organised into a collection. Each page can hold a description or documentation about a hobby or open-source project.1. `_pages/index.md` - this is the default home page.
2. `_includes/components/intro.md` - this chunk is reused between the top of the homepage and the top of the about page.
3. `_pages/about.md` reuses the intro and adds a bit more content about yourself.
4. `_posts` is the default Jekyll collection of blog posts. Each post has a list of tags. These lists are combined into a tag cloud on the post list page.
5. `_projects` is a directory of project pages. These are not organised into a collection. Each page can hold a description or documentation about a hobby or open-source project.1. `_pages/index.md` - this is the default home page.
2. `_includes/components/intro.md` - this chunk is reused between the top of the homepage and the top of the about page.
3. `_pages/about.md` reuses the intro and adds a bit more content about yourself.
4. `_posts` is the default Jekyll collection of blog posts. Each post has a list of tags. These lists are combined into a tag cloud on the post list page.
5. `_projects` is a directory of project pages. These are not organised into a collection. Each page can hold a description or documentation about a hobby or open-source project.1. `_pages/index.md` - this is the default home page.
2. `_includes/components/intro.md` - this chunk is reused between the top of the homepage and the top of the about page.
3. `_pages/about.md` reuses the intro and adds a bit more content about yourself.
4. `_posts` is the default Jekyll collection of blog posts. Each post has a list of tags. These lists are combined into a tag cloud on the post list page.
5. `_projects` is a directory of project pages. These are not organised into a collection. Each page can hold a description or documentation about a hobby or open-source project.1. `_pages/index.md` - this is the default home page.
2. `_includes/components/intro.md` - this chunk is reused between the top of the homepage and the top of the about page.
3. `_pages/about.md` reuses the intro and adds a bit more content about yourself.
4. `_posts` is the default Jekyll collection of blog posts. Each post has a list of tags. These lists are combined into a tag cloud on the post list page.
5. `_projects` is a directory of project pages. These are not organised into a collection. Each page can hold a description or documentation about a hobby or open-source project.1. `_pages/index.md` - this is the default home page.
2. `_includes/components/intro.md` - this chunk is reused between the top of the homepage and the top of the about page.
3. `_pages/about.md` reuses the intro and adds a bit more content about yourself.
4. `_posts` is the default Jekyll collection of blog posts. Each post has a list of tags. These lists are combined into a tag cloud on the post list page.
5. `_projects` is a directory of project pages. These are not organised into a collection. Each page can hold a description or documentation about a hobby or open-source project.1. `_pages/index.md` - this is the default home page.
2. `_includes/components/intro.md` - this chunk is reused between the top of the homepage and the top of the about page.
3. `_pages/about.md` reuses the intro and adds a bit more content about yourself.
4. `_posts` is the default Jekyll collection of blog posts. Each post has a list of tags. These lists are combined into a tag cloud on the post list page.
5. `_projects` is a directory of project pages. These are not organised into a collection. Each page can hold a description or documentation about a hobby or open-source project.1. `_pages/index.md` - this is the default home page.
2. `_includes/components/intro.md` - this chunk is reused between the top of the homepage and the top of the about page.
3. `_pages/about.md` reuses the intro and adds a bit more content about yourself.
4. `_posts` is the default Jekyll collection of blog posts. Each post has a list of tags. These lists are combined into a tag cloud on the post list page.
5. `_projects` is a directory of project pages. These are not organised into a collection. Each page can hold a description or documentation about a hobby or open-source project.1. `_pages/index.md` - this is the default home page.
2. `_includes/components/intro.md` - this chunk is reused between the top of the homepage and the top of the about page.
3. `_pages/about.md` reuses the intro and adds a bit more content about yourself.
4. `_posts` is the default Jekyll collection of blog posts. Each post has a list of tags. These lists are combined into a tag cloud on the post list page.
5. `_projects` is a directory of project pages. These are not organised into a collection. Each page can hold a description or documentation about a hobby or open-source project.1. `_pages/index.md` - this is the default home page.
2. `_includes/components/intro.md` - this chunk is reused between the top of the homepage and the top of the about page.
3. `_pages/about.md` reuses the intro and adds a bit more content about yourself.
4. `_posts` is the default Jekyll collection of blog posts. Each post has a list of tags. These lists are combined into a tag cloud on the post list page.
5. `_projects` is a directory of project pages. These are not organised into a collection. Each page can hold a description or documentation about a hobby or open-source project.1. `_pages/index.md` - this is the default home page.
2. `_includes/components/intro.md` - this chunk is reused between the top of the homepage and the top of the about page.
3. `_pages/about.md` reuses the intro and adds a bit more content about yourself.
4. `_posts` is the default Jekyll collection of blog posts. Each post has a list of tags. These lists are combined into a tag cloud on the post list page.
5. `_projects` is a directory of project pages. These are not organised into a collection. Each page can hold a description or documentation about a hobby or open-source project.1. `_pages/index.md` - this is the default home page.
2. `_includes/components/intro.md` - this chunk is reused between the top of the homepage and the top of the about page.
3. `_pages/about.md` reuses the intro and adds a bit more content about yourself.
4. `_posts` is the default Jekyll collection of blog posts. Each post has a list of tags. These lists are combined into a tag cloud on the post list page.
5. `_projects` is a directory of project pages. These are not organised into a collection. Each page can hold a description or documentation about a hobby or open-source project.1. `_pages/index.md` - this is the default home page.
2. `_includes/components/intro.md` - this chunk is reused between the top of the homepage and the top of the about page.
3. `_pages/about.md` reuses the intro and adds a bit more content about yourself.
4. `_posts` is the default Jekyll collection of blog posts. Each post has a list of tags. These lists are combined into a tag cloud on the post list page.
5. `_projects` is a directory of project pages. These are not organised into a collection. Each page can hold a description or documentation about a hobby or open-source project.1. `_pages/index.md` - this is the default home page.
2. `_includes/components/intro.md` - this chunk is reused between the top of the homepage and the top of the about page.
3. `_pages/about.md` reuses the intro and adds a bit more content about yourself.
4. `_posts` is the default Jekyll collection of blog posts. Each post has a list of tags. These lists are combined into a tag cloud on the post list page.
5. `_projects` is a directory of project pages. These are not organised into a collection. Each page can hold a description or documentation about a hobby or open-source project.1. `_pages/index.md` - this is the default home page.
2. `_includes/components/intro.md` - this chunk is reused between the top of the homepage and the top of the about page.
3. `_pages/about.md` reuses the intro and adds a bit more content about yourself.
4. `_posts` is the default Jekyll collection of blog posts. Each post has a list of tags. These lists are combined into a tag cloud on the post list page.
5. `_projects` is a directory of project pages. These are not organised into a collection. Each page can hold a description or documentation about a hobby or open-source project.1. `_pages/index.md` - this is the default home page.
2. `_includes/components/intro.md` - this chunk is reused between the top of the homepage and the top of the about page.
3. `_pages/about.md` reuses the intro and adds a bit more content about yourself.
4. `_posts` is the default Jekyll collection of blog posts. Each post has a list of tags. These lists are combined into a tag cloud on the post list page.
5. `_projects` is a directory of project pages. These are not organised into a collection. Each page can hold a description or documentation about a hobby or open-source project.1. `_pages/index.md` - this is the default home page.
2. `_includes/components/intro.md` - this chunk is reused between the top of the homepage and the top of the about page.
3. `_pages/about.md` reuses the intro and adds a bit more content about yourself.
4. `_posts` is the default Jekyll collection of blog posts. Each post has a list of tags. These lists are combined into a tag cloud on the post list page.
5. `_projects` is a directory of project pages. These are not organised into a collection. Each page can hold a description or documentation about a hobby or open-source project.1. `_pages/index.md` - this is the default home page.
2. `_includes/components/intro.md` - this chunk is reused between the top of the homepage and the top of the about page.
3. `_pages/about.md` reuses the intro and adds a bit more content about yourself.
4. `_posts` is the default Jekyll collection of blog posts. Each post has a list of tags. These lists are combined into a tag cloud on the post list page.
5. `_projects` is a directory of project pages. These are not organised into a collection. Each page can hold a description or documentation about a hobby or open-source project.1. `_pages/index.md` - this is the default home page.
2. `_includes/components/intro.md` - this chunk is reused between the top of the homepage and the top of the about page.
3. `_pages/about.md` reuses the intro and adds a bit more content about yourself.
4. `_posts` is the default Jekyll collection of blog posts. Each post has a list of tags. These lists are combined into a tag cloud on the post list page.
5. `_projects` is a directory of project pages. These are not organised into a collection. Each page can hold a description or documentation about a hobby or open-source project.1. `_pages/index.md` - this is the default home page.
2. `_includes/components/intro.md` - this chunk is reused between the top of the homepage and the top of the about page.
3. `_pages/about.md` reuses the intro and adds a bit more content about yourself.
4. `_posts` is the default Jekyll collection of blog posts. Each post has a list of tags. These lists are combined into a tag cloud on the post list page.
5. `_projects` is a directory of project pages. These are not organised into a collection. Each page can hold a description or documentation about a hobby or open-source project.1. `_pages/index.md` - this is the default home page.
2. `_includes/components/intro.md` - this chunk is reused between the top of the homepage and the top of the about page.
3. `_pages/about.md` reuses the intro and adds a bit more content about yourself.
4. `_posts` is the default Jekyll collection of blog posts. Each post has a list of tags. These lists are combined into a tag cloud on the post list page.
5. `_projects` is a directory of project pages. These are not organised into a collection. Each page can hold a description or documentation about a hobby or open-source project.1. `_pages/index.md` - this is the default home page.
2. `_includes/components/intro.md` - this chunk is reused between the top of the homepage and the top of the about page.
3. `_pages/about.md` reuses the intro and adds a bit more content about yourself.
4. `_posts` is the default Jekyll collection of blog posts. Each post has a list of tags. These lists are combined into a tag cloud on the post list page.
5. `_projects` is a directory of project pages. These are not organised into a collection. Each page can hold a description or documentation about a hobby or open-source project.1. `_pages/index.md` - this is the default home page.
2. `_includes/components/intro.md` - this chunk is reused between the top of the homepage and the top of the about page.
3. `_pages/about.md` reuses the intro and adds a bit more content about yourself.
4. `_posts` is the default Jekyll collection of blog posts. Each post has a list of tags. These lists are combined into a tag cloud on the post list page.
5. `_projects` is a directory of project pages. These are not organised into a collection. Each page can hold a description or documentation about a hobby or open-source project.1. `_pages/index.md` - this is the default home page.
2. `_includes/components/intro.md` - this chunk is reused between the top of the homepage and the top of the about page.
3. `_pages/about.md` reuses the intro and adds a bit more content about yourself.
4. `_posts` is the default Jekyll collection of blog posts. Each post has a list of tags. These lists are combined into a tag cloud on the post list page.
5. `_projects` is a directory of project pages. These are not organised into a collection. Each page can hold a description or documentation about a hobby or open-source project.1. `_pages/index.md` - this is the default home page.
2. `_includes/components/intro.md` - this chunk is reused between the top of the homepage and the top of the about page.
3. `_pages/about.md` reuses the intro and adds a bit more content about yourself.
4. `_posts` is the default Jekyll collection of blog posts. Each post has a list of tags. These lists are combined into a tag cloud on the post list page.
5. `_projects` is a directory of project pages. These are not organised into a collection. Each page can hold a description or documentation about a hobby or open-source project.1. `_pages/index.md` - this is the default home page.
2. `_includes/components/intro.md` - this chunk is reused between the top of the homepage and the top of the about page.
3. `_pages/about.md` reuses the intro and adds a bit more content about yourself.
4. `_posts` is the default Jekyll collection of blog posts. Each post has a list of tags. These lists are combined into a tag cloud on the post list page.
5. `_projects` is a directory of project pages. These are not organised into a collection. Each page can hold a description or documentation about a hobby or open-source project.1. `_pages/index.md` - this is the default home page.
2. `_includes/components/intro.md` - this chunk is reused between the top of the homepage and the top of the about page.
3. `_pages/about.md` reuses the intro and adds a bit more content about yourself.
4. `_posts` is the default Jekyll collection of blog posts. Each post has a list of tags. These lists are combined into a tag cloud on the post list page.
5. `_projects` is a directory of project pages. These are not organised into a collection. Each page can hold a description or documentation about a hobby or open-source project.1. `_pages/index.md` - this is the default home page.
2. `_includes/components/intro.md` - this chunk is reused between the top of the homepage and the top of the about page.
3. `_pages/about.md` reuses the intro and adds a bit more content about yourself.
4. `_posts` is the default Jekyll collection of blog posts. Each post has a list of tags. These lists are combined into a tag cloud on the post list page.
5. `_projects` is a directory of project pages. These are not organised into a collection. Each page can hold a description or documentation about a hobby or open-source project.1. `_pages/index.md` - this is the default home page.
2. `_includes/components/intro.md` - this chunk is reused between the top of the homepage and the top of the about page.
3. `_pages/about.md` reuses the intro and adds a bit more content about yourself.
4. `_posts` is the default Jekyll collection of blog posts. Each post has a list of tags. These lists are combined into a tag cloud on the post list page.
5. `_projects` is a directory of project pages. These are not organised into a collection. Each page can hold a description or documentation about a hobby or open-source project.1. `_pages/index.md` - this is the default home page.
2. `_includes/components/intro.md` - this chunk is reused between the top of the homepage and the top of the about page.
3. `_pages/about.md` reuses the intro and adds a bit more content about yourself.
4. `_posts` is the default Jekyll collection of blog posts. Each post has a list of tags. These lists are combined into a tag cloud on the post list page.
5. `_projects` is a directory of project pages. These are not organised into a collection. Each page can hold a description or documentation about a hobby or open-source project.1. `_pages/index.md` - this is the default home page.
2. `_includes/components/intro.md` - this chunk is reused between the top of the homepage and the top of the about page.
3. `_pages/about.md` reuses the intro and adds a bit more content about yourself.
4. `_posts` is the default Jekyll collection of blog posts. Each post has a list of tags. These lists are combined into a tag cloud on the post list page.
5. `_projects` is a directory of project pages. These are not organised into a collection. Each page can hold a description or documentation about a hobby or open-source project.1. `_pages/index.md` - this is the default home page.
2. `_includes/components/intro.md` - this chunk is reused between the top of the homepage and the top of the about page.
3. `_pages/about.md` reuses the intro and adds a bit more content about yourself.
4. `_posts` is the default Jekyll collection of blog posts. Each post has a list of tags. These lists are combined into a tag cloud on the post list page.
5. `_projects` is a directory of project pages. These are not organised into a collection. Each page can hold a description or documentation about a hobby or open-source project.1. `_pages/index.md` - this is the default home page.
2. `_includes/components/intro.md` - this chunk is reused between the top of the homepage and the top of the about page.
3. `_pages/about.md` reuses the intro and adds a bit more content about yourself.
4. `_posts` is the default Jekyll collection of blog posts. Each post has a list of tags. These lists are combined into a tag cloud on the post list page.
5. `_projects` is a directory of project pages. These are not organised into a collection. Each page can hold a description or documentation about a hobby or open-source project.1. `_pages/index.md` - this is the default home page.
2. `_includes/components/intro.md` - this chunk is reused between the top of the homepage and the top of the about page.
3. `_pages/about.md` reuses the intro and adds a bit more content about yourself.
4. `_posts` is the default Jekyll collection of blog posts. Each post has a list of tags. These lists are combined into a tag cloud on the post list page.
5. `_projects` is a directory of project pages. These are not organised into a collection. Each page can hold a description or documentation about a hobby or open-source project.1. `_pages/index.md` - this is the default home page.
2. `_includes/components/intro.md` - this chunk is reused between the top of the homepage and the top of the about page.
3. `_pages/about.md` reuses the intro and adds a bit more content about yourself.
4. `_posts` is the default Jekyll collection of blog posts. Each post has a list of tags. These lists are combined into a tag cloud on the post list page.
5. `_projects` is a directory of project pages. These are not organised into a collection. Each page can hold a description or documentation about a hobby or open-source project.1. `_pages/index.md` - this is the default home page.
2. `_includes/components/intro.md` - this chunk is reused between the top of the homepage and the top of the about page.
3. `_pages/about.md` reuses the intro and adds a bit more content about yourself.
4. `_posts` is the default Jekyll collection of blog posts. Each post has a list of tags. These lists are combined into a tag cloud on the post list page.
5. `_projects` is a directory of project pages. These are not organised into a collection. Each page can hold a description or documentation about a hobby or open-source project.1. `_pages/index.md` - this is the default home page.
2. `_includes/components/intro.md` - this chunk is reused between the top of the homepage and the top of the about page.
3. `_pages/about.md` reuses the intro and adds a bit more content about yourself.
4. `_posts` is the default Jekyll collection of blog posts. Each post has a list of tags. These lists are combined into a tag cloud on the post list page.
5. `_projects` is a directory of project pages. These are not organised into a collection. Each page can hold a description or documentation about a hobby or open-source project.1. `_pages/index.md` - this is the default home page.
2. `_includes/components/intro.md` - this chunk is reused between the top of the homepage and the top of the about page.
3. `_pages/about.md` reuses the intro and adds a bit more content about yourself.
4. `_posts` is the default Jekyll collection of blog posts. Each post has a list of tags. These lists are combined into a tag cloud on the post list page.
5. `_projects` is a directory of project pages. These are not organised into a collection. Each page can hold a description or documentation about a hobby or open-source project.1. `_pages/index.md` - this is the default home page.
2. `_includes/components/intro.md` - this chunk is reused between the top of the homepage and the top of the about page.
3. `_pages/about.md` reuses the intro and adds a bit more content about yourself.
4. `_posts` is the default Jekyll collection of blog posts. Each post has a list of tags. These lists are combined into a tag cloud on the post list page.
5. `_projects` is a directory of project pages. These are not organised into a collection. Each page can hold a description or documentation about a hobby or open-source project.1. `_pages/index.md` - this is the default home page.
2. `_includes/components/intro.md` - this chunk is reused between the top of the homepage and the top of the about page.
3. `_pages/about.md` reuses the intro and adds a bit more content about yourself.
4. `_posts` is the default Jekyll collection of blog posts. Each post has a list of tags. These lists are combined into a tag cloud on the post list page.
5. `_projects` is a directory of project pages. These are not organised into a collection. Each page can hold a description or documentation about a hobby or open-source project.1. `_pages/index.md` - this is the default home page.
2. `_includes/components/intro.md` - this chunk is reused between the top of the homepage and the top of the about page.
3. `_pages/about.md` reuses the intro and adds a bit more content about yourself.
4. `_posts` is the default Jekyll collection of blog posts. Each post has a list of tags. These lists are combined into a tag cloud on the post list page.
5. `_projects` is a directory of project pages. These are not organised into a collection. Each page can hold a description or documentation about a hobby or open-source project.1. `_pages/index.md` - this is the default home page.
2. `_includes/components/intro.md` - this chunk is reused between the top of the homepage and the top of the about page.
3. `_pages/about.md` reuses the intro and adds a bit more content about yourself.
4. `_posts` is the default Jekyll collection of blog posts. Each post has a list of tags. These lists are combined into a tag cloud on the post list page.
5. `_projects` is a directory of project pages. These are not organised into a collection. Each page can hold a description or documentation about a hobby or open-source project.1. `_pages/index.md` - this is the default home page.
2. `_includes/components/intro.md` - this chunk is reused between the top of the homepage and the top of the about page.
3. `_pages/about.md` reuses the intro and adds a bit more content about yourself.
4. `_posts` is the default Jekyll collection of blog posts. Each post has a list of tags. These lists are combined into a tag cloud on the post list page.
5. `_projects` is a directory of project pages. These are not organised into a collection. Each page can hold a description or documentation about a hobby or open-source project.1. `_pages/index.md` - this is the default home page.
2. `_includes/components/intro.md` - this chunk is reused between the top of the homepage and the top of the about page.
3. `_pages/about.md` reuses the intro and adds a bit more content about yourself.
4. `_posts` is the default Jekyll collection of blog posts. Each post has a list of tags. These lists are combined into a tag cloud on the post list page.
5. `_projects` is a directory of project pages. These are not organised into a collection. Each page can hold a description or documentation about a hobby or open-source project.1. `_pages/index.md` - this is the default home page.
2. `_includes/components/intro.md` - this chunk is reused between the top of the homepage and the top of the about page.
3. `_pages/about.md` reuses the intro and adds a bit more content about yourself.
4. `_posts` is the default Jekyll collection of blog posts. Each post has a list of tags. These lists are combined into a tag cloud on the post list page.
5. `_projects` is a directory of project pages. These are not organised into a collection. Each page can hold a description or documentation about a hobby or open-source project.1. `_pages/index.md` - this is the default home page.
2. `_includes/components/intro.md` - this chunk is reused between the top of the homepage and the top of the about page.
3. `_pages/about.md` reuses the intro and adds a bit more content about yourself.
4. `_posts` is the default Jekyll collection of blog posts. Each post has a list of tags. These lists are combined into a tag cloud on the post list page.
5. `_projects` is a directory of project pages. These are not organised into a collection. Each page can hold a description or documentation about a hobby or open-source project.1. `_pages/index.md` - this is the default home page.
2. `_includes/components/intro.md` - this chunk is reused between the top of the homepage and the top of the about page.
3. `_pages/about.md` reuses the intro and adds a bit more content about yourself.
4. `_posts` is the default Jekyll collection of blog posts. Each post has a list of tags. These lists are combined into a tag cloud on the post list page.
5. `_projects` is a directory of project pages. These are not organised into a collection. Each page can hold a description or documentation about a hobby or open-source project.1. `_pages/index.md` - this is the default home page.
2. `_includes/components/intro.md` - this chunk is reused between the top of the homepage and the top of the about page.
3. `_pages/about.md` reuses the intro and adds a bit more content about yourself.
4. `_posts` is the default Jekyll collection of blog posts. Each post has a list of tags. These lists are combined into a tag cloud on the post list page.
5. `_projects` is a directory of project pages. These are not organised into a collection. Each page can hold a description or documentation about a hobby or open-source project.1. `_pages/index.md` - this is the default home page.
2. `_includes/components/intro.md` - this chunk is reused between the top of the homepage and the top of the about page.
3. `_pages/about.md` reuses the intro and adds a bit more content about yourself.
4. `_posts` is the default Jekyll collection of blog posts. Each post has a list of tags. These lists are combined into a tag cloud on the post list page.
5. `_projects` is a directory of project pages. These are not organised into a collection. Each page can hold a description or documentation about a hobby or open-source project.1. `_pages/index.md` - this is the default home page.
2. `_includes/components/intro.md` - this chunk is reused between the top of the homepage and the top of the about page.
3. `_pages/about.md` reuses the intro and adds a bit more content about yourself.
4. `_posts` is the default Jekyll collection of blog posts. Each post has a list of tags. These lists are combined into a tag cloud on the post list page.
5. `_projects` is a directory of project pages. These are not organised into a collection. Each page can hold a description or documentation about a hobby or open-source project.1. `_pages/index.md` - this is the default home page.
2. `_includes/components/intro.md` - this chunk is reused between the top of the homepage and the top of the about page.
3. `_pages/about.md` reuses the intro and adds a bit more content about yourself.
4. `_posts` is the default Jekyll collection of blog posts. Each post has a list of tags. These lists are combined into a tag cloud on the post list page.
5. `_projects` is a directory of project pages. These are not organised into a collection. Each page can hold a description or documentation about a hobby or open-source project.1. `_pages/index.md` - this is the default home page.
2. `_includes/components/intro.md` - this chunk is reused between the top of the homepage and the top of the about page.
3. `_pages/about.md` reuses the intro and adds a bit more content about yourself.
4. `_posts` is the default Jekyll collection of blog posts. Each post has a list of tags. These lists are combined into a tag cloud on the post list page.
5. `_projects` is a directory of project pages. These are not organised into a collection. Each page can hold a description or documentation about a hobby or open-source project.1. `_pages/index.md` - this is the default home page.
2. `_includes/components/intro.md` - this chunk is reused between the top of the homepage and the top of the about page.
3. `_pages/about.md` reuses the intro and adds a bit more content about yourself.
4. `_posts` is the default Jekyll collection of blog posts. Each post has a list of tags. These lists are combined into a tag cloud on the post list page.
5. `_projects` is a directory of project pages. These are not organised into a collection. Each page can hold a description or documentation about a hobby or open-source project.1. `_pages/index.md` - this is the default home page.
2. `_includes/components/intro.md` - this chunk is reused between the top of the homepage and the top of the about page.
3. `_pages/about.md` reuses the intro and adds a bit more content about yourself.
4. `_posts` is the default Jekyll collection of blog posts. Each post has a list of tags. These lists are combined into a tag cloud on the post list page.
5. `_projects` is a directory of project pages. These are not organised into a collection. Each page can hold a description or documentation about a hobby or open-source project.1. `_pages/index.md` - this is the default home page.
2. `_includes/components/intro.md` - this chunk is reused between the top of the homepage and the top of the about page.
3. `_pages/about.md` reuses the intro and adds a bit more content about yourself.
4. `_posts` is the default Jekyll collection of blog posts. Each post has a list of tags. These lists are combined into a tag cloud on the post list page.
5. `_projects` is a directory of project pages. These are not organised into a collection. Each page can hold a description or documentation about a hobby or open-source project.1. `_pages/index.md` - this is the default home page.
2. `_includes/components/intro.md` - this chunk is reused between the top of the homepage and the top of the about page.
3. `_pages/about.md` reuses the intro and adds a bit more content about yourself.
4. `_posts` is the default Jekyll collection of blog posts. Each post has a list of tags. These lists are combined into a tag cloud on the post list page.
5. `_projects` is a directory of project pages. These are not organised into a collection. Each page can hold a description or documentation about a hobby or open-source project.1. `_pages/index.md` - this is the default home page.
2. `_includes/components/intro.md` - this chunk is reused between the top of the homepage and the top of the about page.
3. `_pages/about.md` reuses the intro and adds a bit more content about yourself.
4. `_posts` is the default Jekyll collection of blog posts. Each post has a list of tags. These lists are combined into a tag cloud on the post list page.
5. `_projects` is a directory of project pages. These are not organised into a collection. Each page can hold a description or documentation about a hobby or open-source project.1. `_pages/index.md` - this is the default home page.
2. `_includes/components/intro.md` - this chunk is reused between the top of the homepage and the top of the about page.
3. `_pages/about.md` reuses the intro and adds a bit more content about yourself.
4. `_posts` is the default Jekyll collection of blog posts. Each post has a list of tags. These lists are combined into a tag cloud on the post list page.
5. `_projects` is a directory of project pages. These are not organised into a collection. Each page can hold a description or documentation about a hobby or open-source project.1. `_pages/index.md` - this is the default home page.
2. `_includes/components/intro.md` - this chunk is reused between the top of the homepage and the top of the about page.
3. `_pages/about.md` reuses the intro and adds a bit more content about yourself.
4. `_posts` is the default Jekyll collection of blog posts. Each post has a list of tags. These lists are combined into a tag cloud on the post list page.
5. `_projects` is a directory of project pages. These are not organised into a collection. Each page can hold a description or documentation about a hobby or open-source project.1. `_pages/index.md` - this is the default home page.
2. `_includes/components/intro.md` - this chunk is reused between the top of the homepage and the top of the about page.
3. `_pages/about.md` reuses the intro and adds a bit more content about yourself.
4. `_posts` is the default Jekyll collection of blog posts. Each post has a list of tags. These lists are combined into a tag cloud on the post list page.
5. `_projects` is a directory of project pages. These are not organised into a collection. Each page can hold a description or documentation about a hobby or open-source project.1. `_pages/index.md` - this is the default home page.
2. `_includes/components/intro.md` - this chunk is reused between the top of the homepage and the top of the about page.
3. `_pages/about.md` reuses the intro and adds a bit more content about yourself.
4. `_posts` is the default Jekyll collection of blog posts. Each post has a list of tags. These lists are combined into a tag cloud on the post list page.
5. `_projects` is a directory of project pages. These are not organised into a collection. Each page can hold a description or documentation about a hobby or open-source project.1. `_pages/index.md` - this is the default home page.
2. `_includes/components/intro.md` - this chunk is reused between the top of the homepage and the top of the about page.
3. `_pages/about.md` reuses the intro and adds a bit more content about yourself.
4. `_posts` is the default Jekyll collection of blog posts. Each post has a list of tags. These lists are combined into a tag cloud on the post list page.
5. `_projects` is a directory of project pages. These are not organised into a collection. Each page can hold a description or documentation about a hobby or open-source project.1. `_pages/index.md` - this is the default home page.
2. `_includes/components/intro.md` - this chunk is reused between the top of the homepage and the top of the about page.
3. `_pages/about.md` reuses the intro and adds a bit more content about yourself.
4. `_posts` is the default Jekyll collection of blog posts. Each post has a list of tags. These lists are combined into a tag cloud on the post list page.
5. `_projects` is a directory of project pages. These are not organised into a collection. Each page can hold a description or documentation about a hobby or open-source project.1. `_pages/index.md` - this is the default home page.
2. `_includes/components/intro.md` - this chunk is reused between the top of the homepage and the top of the about page.
3. `_pages/about.md` reuses the intro and adds a bit more content about yourself.
4. `_posts` is the default Jekyll collection of blog posts. Each post has a list of tags. These lists are combined into a tag cloud on the post list page.
5. `_projects` is a directory of project pages. These are not organised into a collection. Each page can hold a description or documentation about a hobby or open-source project.1. `_pages/index.md` - this is the default home page.
2. `_includes/components/intro.md` - this chunk is reused between the top of the homepage and the top of the about page.
3. `_pages/about.md` reuses the intro and adds a bit more content about yourself.
4. `_posts` is the default Jekyll collection of blog posts. Each post has a list of tags. These lists are combined into a tag cloud on the post list page.
5. `_projects` is a directory of project pages. These are not organised into a collection. Each page can hold a description or documentation about a hobby or open-source project.1. `_pages/index.md` - this is the default home page.
2. `_includes/components/intro.md` - this chunk is reused between the top of the homepage and the top of the about page.
3. `_pages/about.md` reuses the intro and adds a bit more content about yourself.
4. `_posts` is the default Jekyll collection of blog posts. Each post has a list of tags. These lists are combined into a tag cloud on the post list page.
5. `_projects` is a directory of project pages. These are not organised into a collection. Each page can hold a description or documentation about a hobby or open-source project.1. `_pages/index.md` - this is the default home page.
2. `_includes/components/intro.md` - this chunk is reused between the top of the homepage and the top of the about page.
3. `_pages/about.md` reuses the intro and adds a bit more content about yourself.
4. `_posts` is the default Jekyll collection of blog posts. Each post has a list of tags. These lists are combined into a tag cloud on the post list page.
5. `_projects` is a directory of project pages. These are not organised into a collection. Each page can hold a description or documentation about a hobby or open-source project.1. `_pages/index.md` - this is the default home page.
2. `_includes/components/intro.md` - this chunk is reused between the top of the homepage and the top of the about page.
3. `_pages/about.md` reuses the intro and adds a bit more content about yourself.
4. `_posts` is the default Jekyll collection of blog posts. Each post has a list of tags. These lists are combined into a tag cloud on the post list page.
5. `_projects` is a directory of project pages. These are not organised into a collection. Each page can hold a description or documentation about a hobby or open-source project.1. `_pages/index.md` - this is the default home page.
2. `_includes/components/intro.md` - this chunk is reused between the top of the homepage and the top of the about page.
3. `_pages/about.md` reuses the intro and adds a bit more content about yourself.
4. `_posts` is the default Jekyll collection of blog posts. Each post has a list of tags. These lists are combined into a tag cloud on the post list page.
5. `_projects` is a directory of project pages. These are not organised into a collection. Each page can hold a description or documentation about a hobby or open-source project.1. `_pages/index.md` - this is the default home page.
2. `_includes/components/intro.md` - this chunk is reused between the top of the homepage and the top of the about page.
3. `_pages/about.md` reuses the intro and adds a bit more content about yourself.
4. `_posts` is the default Jekyll collection of blog posts. Each post has a list of tags. These lists are combined into a tag cloud on the post list page.
5. `_projects` is a directory of project pages. These are not organised into a collection. Each page can hold a description or documentation about a hobby or open-source project.1. `_pages/index.md` - this is the default home page.
2. `_includes/components/intro.md` - this chunk is reused between the top of the homepage and the top of the about page.
3. `_pages/about.md` reuses the intro and adds a bit more content about yourself.
4. `_posts` is the default Jekyll collection of blog posts. Each post has a list of tags. These lists are combined into a tag cloud on the post list page.
5. `_projects` is a directory of project pages. These are not organised into a collection. Each page can hold a description or documentation about a hobby or open-source project.1. `_pages/index.md` - this is the default home page.
2. `_includes/components/intro.md` - this chunk is reused between the top of the homepage and the top of the about page.
3. `_pages/about.md` reuses the intro and adds a bit more content about yourself.
4. `_posts` is the default Jekyll collection of blog posts. Each post has a list of tags. These lists are combined into a tag cloud on the post list page.
5. `_projects` is a directory of project pages. These are not organised into a collection. Each page can hold a description or documentation about a hobby or open-source project.1. `_pages/index.md` - this is the default home page.
2. `_includes/components/intro.md` - this chunk is reused between the top of the homepage and the top of the about page.
3. `_pages/about.md` reuses the intro and adds a bit more content about yourself.
4. `_posts` is the default Jekyll collection of blog posts. Each post has a list of tags. These lists are combined into a tag cloud on the post list page.
5. `_projects` is a directory of project pages. These are not organised into a collection. Each page can hold a description or documentation about a hobby or open-source project.1. `_pages/index.md` - this is the default home page.
2. `_includes/components/intro.md` - this chunk is reused between the top of the homepage and the top of the about page.
3. `_pages/about.md` reuses the intro and adds a bit more content about yourself.
4. `_posts` is the default Jekyll collection of blog posts. Each post has a list of tags. These lists are combined into a tag cloud on the post list page.
5. `_projects` is a directory of project pages. These are not organised into a collection. Each page can hold a description or documentation about a hobby or open-source project.1. `_pages/index.md` - this is the default home page.
2. `_includes/components/intro.md` - this chunk is reused between the top of the homepage and the top of the about page.
3. `_pages/about.md` reuses the intro and adds a bit more content about yourself.
4. `_posts` is the default Jekyll collection of blog posts. Each post has a list of tags. These lists are combined into a tag cloud on the post list page.
5. `_projects` is a directory of project pages. These are not organised into a collection. Each page can hold a description or documentation about a hobby or open-source project.1. `_pages/index.md` - this is the default home page.
2. `_includes/components/intro.md` - this chunk is reused between the top of the homepage and the top of the about page.
3. `_pages/about.md` reuses the intro and adds a bit more content about yourself.
4. `_posts` is the default Jekyll collection of blog posts. Each post has a list of tags. These lists are combined into a tag cloud on the post list page.
5. `_projects` is a directory of project pages. These are not organised into a collection. Each page can hold a description or documentation about a hobby or open-source project.1. `_pages/index.md` - this is the default home page.
2. `_includes/components/intro.md` - this chunk is reused between the top of the homepage and the top of the about page.
3. `_pages/about.md` reuses the intro and adds a bit more content about yourself.
4. `_posts` is the default Jekyll collection of blog posts. Each post has a list of tags. These lists are combined into a tag cloud on the post list page.
5. `_projects` is a directory of project pages. These are not organised into a collection. Each page can hold a description or documentation about a hobby or open-source project.1. `_pages/index.md` - this is the default home page.
2. `_includes/components/intro.md` - this chunk is reused between the top of the homepage and the top of the about page.
3. `_pages/about.md` reuses the intro and adds a bit more content about yourself.
4. `_posts` is the default Jekyll collection of blog posts. Each post has a list of tags. These lists are combined into a tag cloud on the post list page.
5. `_projects` is a directory of project pages. These are not organised into a collection. Each page can hold a description or documentation about a hobby or open-source project.1. `_pages/index.md` - this is the default home page.
2. `_includes/components/intro.md` - this chunk is reused between the top of the homepage and the top of the about page.
3. `_pages/about.md` reuses the intro and adds a bit more content about yourself.
4. `_posts` is the default Jekyll collection of blog posts. Each post has a list of tags. These lists are combined into a tag cloud on the post list page.
5. `_projects` is a directory of project pages. These are not organised into a collection. Each page can hold a description or documentation about a hobby or open-source project.1. `_pages/index.md` - this is the default home page.
2. `_includes/components/intro.md` - this chunk is reused between the top of the homepage and the top of the about page.
3. `_pages/about.md` reuses the intro and adds a bit more content about yourself.
4. `_posts` is the default Jekyll collection of blog posts. Each post has a list of tags. These lists are combined into a tag cloud on the post list page.
5. `_projects` is a directory of project pages. These are not organised into a collection. Each page can hold a description or documentation about a hobby or open-source project.1. `_pages/index.md` - this is the default home page.
2. `_includes/components/intro.md` - this chunk is reused between the top of the homepage and the top of the about page.
3. `_pages/about.md` reuses the intro and adds a bit more content about yourself.
4. `_posts` is the default Jekyll collection of blog posts. Each post has a list of tags. These lists are combined into a tag cloud on the post list page.
5. `_projects` is a directory of project pages. These are not organised into a collection. Each page can hold a description or documentation about a hobby or open-source project.1. `_pages/index.md` - this is the default home page.
2. `_includes/components/intro.md` - this chunk is reused between the top of the homepage and the top of the about page.
3. `_pages/about.md` reuses the intro and adds a bit more content about yourself.
4. `_posts` is the default Jekyll collection of blog posts. Each post has a list of tags. These lists are combined into a tag cloud on the post list page.
5. `_projects` is a directory of project pages. These are not organised into a collection. Each page can hold a description or documentation about a hobby or open-source project.1. `_pages/index.md` - this is the default home page.
2. `_includes/components/intro.md` - this chunk is reused between the top of the homepage and the top of the about page.
3. `_pages/about.md` reuses the intro and adds a bit more content about yourself.
4. `_posts` is the default Jekyll collection of blog posts. Each post has a list of tags. These lists are combined into a tag cloud on the post list page.
5. `_projects` is a directory of project pages. These are not organised into a collection. Each page can hold a description or documentation about a hobby or open-source project.1. `_pages/index.md` - this is the default home page.
2. `_includes/components/intro.md` - this chunk is reused between the top of the homepage and the top of the about page.
3. `_pages/about.md` reuses the intro and adds a bit more content about yourself.
4. `_posts` is the default Jekyll collection of blog posts. Each post has a list of tags. These lists are combined into a tag cloud on the post list page.
5. `_projects` is a directory of project pages. These are not organised into a collection. Each page can hold a description or documentation about a hobby or open-source project.1. `_pages/index.md` - this is the default home page.
2. `_includes/components/intro.md` - this chunk is reused between the top of the homepage and the top of the about page.
3. `_pages/about.md` reuses the intro and adds a bit more content about yourself.
4. `_posts` is the default Jekyll collection of blog posts. Each post has a list of tags. These lists are combined into a tag cloud on the post list page.
5. `_projects` is a directory of project pages. These are not organised into a collection. Each page can hold a description or documentation about a hobby or open-source project.1. `_pages/index.md` - this is the default home page.
2. `_includes/components/intro.md` - this chunk is reused between the top of the homepage and the top of the about page.
3. `_pages/about.md` reuses the intro and adds a bit more content about yourself.
4. `_posts` is the default Jekyll collection of blog posts. Each post has a list of tags. These lists are combined into a tag cloud on the post list page.
5. `_projects` is a directory of project pages. These are not organised into a collection. Each page can hold a description or documentation about a hobby or open-source project.1. `_pages/index.md` - this is the default home page.
2. `_includes/components/intro.md` - this chunk is reused between the top of the homepage and the top of the about page.
3. `_pages/about.md` reuses the intro and adds a bit more content about yourself.
4. `_posts` is the default Jekyll collection of blog posts. Each post has a list of tags. These lists are combined into a tag cloud on the post list page.
5. `_projects` is a directory of project pages. These are not organised into a collection. Each page can hold a description or documentation about a hobby or open-source project.1. `_pages/index.md` - this is the default home page.
2. `_includes/components/intro.md` - this chunk is reused between the top of the homepage and the top of the about page.
3. `_pages/about.md` reuses the intro and adds a bit more content about yourself.
4. `_posts` is the default Jekyll collection of blog posts. Each post has a list of tags. These lists are combined into a tag cloud on the post list page.
5. `_projects` is a directory of project pages. These are not organised into a collection. Each page can hold a description or documentation about a hobby or open-source project.1. `_pages/index.md` - this is the default home page.
2. `_includes/components/intro.md` - this chunk is reused between the top of the homepage and the top of the about page.
3. `_pages/about.md` reuses the intro and adds a bit more content about yourself.
4. `_posts` is the default Jekyll collection of blog posts. Each post has a list of tags. These lists are combined into a tag cloud on the post list page.
5. `_projects` is a directory of project pages. These are not organised into a collection. Each page can hold a description or documentation about a hobby or open-source project.1. `_pages/index.md` - this is the default home page.
2. `_includes/components/intro.md` - this chunk is reused between the top of the homepage and the top of the about page.
3. `_pages/about.md` reuses the intro and adds a bit more content about yourself.
4. `_posts` is the default Jekyll collection of blog posts. Each post has a list of tags. These lists are combined into a tag cloud on the post list page.
5. `_projects` is a directory of project pages. These are not organised into a collection. Each page can hold a description or documentation about a hobby or open-source project.1. `_pages/index.md` - this is the default home page.
2. `_includes/components/intro.md` - this chunk is reused between the top of the homepage and the top of the about page.
3. `_pages/about.md` reuses the intro and adds a bit more content about yourself.
4. `_posts` is the default Jekyll collection of blog posts. Each post has a list of tags. These lists are combined into a tag cloud on the post list page.
5. `_projects` is a directory of project pages. These are not organised into a collection. Each page can hold a description or documentation about a hobby or open-source project.1. `_pages/index.md` - this is the default home page.
2. `_includes/components/intro.md` - this chunk is reused between the top of the homepage and the top of the about page.
3. `_pages/about.md` reuses the intro and adds a bit more content about yourself.
4. `_posts` is the default Jekyll collection of blog posts. Each post has a list of tags. These lists are combined into a tag cloud on the post list page.
5. `_projects` is a directory of project pages. These are not organised into a collection. Each page can hold a description or documentation about a hobby or open-source project.1. `_pages/index.md` - this is the default home page.
2. `_includes/components/intro.md` - this chunk is reused between the top of the homepage and the top of the about page.
3. `_pages/about.md` reuses the intro and adds a bit more content about yourself.
4. `_posts` is the default Jekyll collection of blog posts. Each post has a list of tags. These lists are combined into a tag cloud on the post list page.
5. `_projects` is a directory of project pages. These are not organised into a collection. Each page can hold a description or documentation about a hobby or open-source project.
## HTML Content
## HTML Content
## HTML Content
## HTML Content
## HTML Content
## HTML Content
## HTML Content
## HTML Content
## HTML Content
## HTML Content
## HTML Content
1. `_pages/index.md` - this is the default home page.
2. `_includes/components/intro.md` - this chunk is reused between the top of the homepage and the top of the about page.
3. `_pages/about.md` reuses the intro and adds a bit more content about yourself.
4. `_posts` is the default Jekyll collection of blog posts. Each post has a list of tags. These lists are combined into a tag cloud on the post list page.
5. `_projects` is a directory of project pages. These are not organised into a collection. Each page can hold a description or documentation about a hobby or open-source project.1. `_pages/index.md` - this is the default home page.
2. `_includes/components/intro.md` - this chunk is reused between the top of the homepage and the top of the about page.
3. `_pages/about.md` reuses the intro and adds a bit more content about yourself.
4. `_posts` is the default Jekyll collection of blog posts. Each post has a list of tags. These lists are combined into a tag cloud on the post list page.
5. `_projects` is a directory of project pages. These are not organised into a collection. Each page can hold a description or documentation about a hobby or open-source project.1. `_pages/index.md` - this is the default home page.
2. `_includes/components/intro.md` - this chunk is reused between the top of the homepage and the top of the about page.
3. `_pages/about.md` reuses the intro and adds a bit more content about yourself.
4. `_posts` is the default Jekyll collection of blog posts. Each post has a list of tags. These lists are combined into a tag cloud on the post list page.
5. `_projects` is a directory of project pages. These are not organised into a collection. Each page can hold a description or documentation about a hobby or open-source project.1. `_pages/index.md` - this is the default home page.
2. `_includes/components/intro.md` - this chunk is reused between the top of the homepage and the top of the about page.
3. `_pages/about.md` reuses the intro and adds a bit more content about yourself.
4. `_posts` is the default Jekyll collection of blog posts. Each post has a list of tags. These lists are combined into a tag cloud on the post list page.
5. `_projects` is a directory of project pages. These are not organised into a collection. Each page can hold a description or documentation about a hobby or open-source project.1. `_pages/index.md` - this is the default home page.
2. `_includes/components/intro.md` - this chunk is reused between the top of the homepage and the top of the about page.
3. `_pages/about.md` reuses the intro and adds a bit more content about yourself.
4. `_posts` is the default Jekyll collection of blog posts. Each post has a list of tags. These lists are combined into a tag cloud on the post list page.
5. `_projects` is a directory of project pages. These are not organised into a collection. Each page can hold a description or documentation about a hobby or open-source project.1. `_pages/index.md` - this is the default home page.
2. `_includes/components/intro.md` - this chunk is reused between the top of the homepage and the top of the about page.
3. `_pages/about.md` reuses the intro and adds a bit more content about yourself.
4. `_posts` is the default Jekyll collection of blog posts. Each post has a list of tags. These lists are combined into a tag cloud on the post list page.
5. `_projects` is a directory of project pages. These are not organised into a collection. Each page can hold a description or documentation about a hobby or open-source project.1. `_pages/index.md` - this is the default home page.
2. `_includes/components/intro.md` - this chunk is reused between the top of the homepage and the top of the about page.
3. `_pages/about.md` reuses the intro and adds a bit more content about yourself.
4. `_posts` is the default Jekyll collection of blog posts. Each post has a list of tags. These lists are combined into a tag cloud on the post list page.
5. `_projects` is a directory of project pages. These are not organised into a collection. Each page can hold a description or documentation about a hobby or open-source project.1. `_pages/index.md` - this is the default home page.
2. `_includes/components/intro.md` - this chunk is reused between the top of the homepage and the top of the about page.
3. `_pages/about.md` reuses the intro and adds a bit more content about yourself.
4. `_posts` is the default Jekyll collection of blog posts. Each post has a list of tags. These lists are combined into a tag cloud on the post list page.
5. `_projects` is a directory of project pages. These are not organised into a collection. Each page can hold a description or documentation about a hobby or open-source project.1. `_pages/index.md` - this is the default home page.
2. `_includes/components/intro.md` - this chunk is reused between the top of the homepage and the top of the about page.
3. `_pages/about.md` reuses the intro and adds a bit more content about yourself.
4. `_posts` is the default Jekyll collection of blog posts. Each post has a list of tags. These lists are combined into a tag cloud on the post list page.
5. `_projects` is a directory of project pages. These are not organised into a collection. Each page can hold a description or documentation about a hobby or open-source project.
