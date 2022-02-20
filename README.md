# mybook

#reverse an array
```c++
#include <bits/stdc++.h>
using namespace std;

int main() {
	int arr[]={1,2,3,4,5,6};
	int n=sizeof(arr)/sizeof arr[0];
	for(int i=0,j=n-1;i<j;i++,j--)
	{
		swap(arr[i],arr[j]);
	}
	for(int i=0;i<n;++i)
	{
		cout<<arr[i];
	}
	return 0;
}
```
# reverse a  string
```c++
    #include<bits/stdc++.h>
     
    using namespace std;
     
    int main()
    {
     string s="test";
     int size=s.length();
     int l=0;
     int r=size-1;
     while(l<r)
     {
     	swap(s[l++],s[r--]);
     }
     cout<<s;
     return 0;
    }
```
