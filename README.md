# Codeforcescpp-276A
#include <bits/stdc++.h>

using namespace std;

int main(){
  int n,k,f,t;
  vector<int> v;
  cin >> n >> k;
  for(int i=0;i<n;i++){
    cin >> f >> t;
    if(k >= t){
      v.push_back(f);
    }
    else{
      v.push_back(f-(t-k));
    }
  }
  cout << *max_element(v.begin(),v.end());
  return 0;
}
