# cf_751_div2
This repository contains my solutions to problem of codeforces 751 div 2.
#include <bits/stdc++.h>
using namespace std;
typedef long long ll;
#define pll pair<ll,ll>
#define vll vector<ll>
#define  ln "\n"
#define pii pair<int,int>
#define fi first
#define se second
#define pb push_back
#define mp make_pair
#define be begin
#define ub upper_bound
#define lb lower_bound
#define bi binary_search
#define sll set <ll>
#define msll multiset <ll>
#define vpll vector <pair<ll,ll>>
#define mll  map <ll,ll>
#define all(v) v.begin(),v.end()
#define mem1(a)  memset(a,-1,sizeof(a))
#define mem0(a)  memset(a,0,sizeof(a))
#define i1(x) cin>>x
#define i2(x1,x2) cin>>x1>>x2
#define i3(x1,x2,x3) cin>>x1>>x2>>x3
#define i4(x1,x2,x3,x4) cin>>x1>>x2>>x3>>x4
#define o1(x) cout<<x<<ln
#define o2(x1,x2) cout<<x1<<" "<<x2<<ln
#define o3(x1,x2,x3) cout<<x1<<" "<<x2<<" "<<x3<<ln
#define o4(x1,x2,x3,x4) cout<<x1<<" "<<x2<<" "<<x3<<" "<<x4<<ln
#define rep(i,s,e) for(ll i=s;i<e;i++)
#define rrep(i,s,e) for(ll i=s-1;i>=e;i--)
#define geta(a,n) for(ll i=0;i<n;i++)cin>>a[i];
const ll mod = 1e9 + 7;
const ll infinity = 1e18;

void  solve()
{
 string s;
 i1(s);
 ll n=s.length();
 mll m;
 rep(i,0,n)
 {
   int k=s[i]-'a';
   m[k]++;
 }
 char c1;
 string s1="";
 rep(i,0,26)
 {
  if(m[i]!=0)
  {
    c1='a'+i;
    break;
  }
 }
 ll f=0;
 rep(i,0,n)
 {
  if(f!=0||s[i]!=c1)
  {
    s1=s1+s[i];
   
  }
  else if(c1==s[i])
  {
    f=1;
  }
 }
 o2(c1,s1);
}


int main()
{
  ios_base::sync_with_stdio(false);
  cin.tie(NULL);
  cout.tie(NULL);
  ll t = 1;
  cin >> t;
  //cout<<t<<ln;
  for(ll i=1;i<=t;i++)
  {
    // o1(6-t);
    //cout<<"Case #"<<i<<": ";
    solve();
    
  }
  return 0;
}
