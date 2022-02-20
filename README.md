# mybook
# max and min in array
```c++
#include <bits/stdc++.h>

using namespace std;

int main(){

int arr[]={1, 2, 3 ,5, 4,7,6};
int size=sizeof(arr)/sizeof(arr[0]);
int max=arr[0],min=arr[0];

    for(int i=0;i<size;++i)
    {
        if(arr[i]>max) max=arr[i];
        else
        if(arr[i]<min) min=arr[i];
    }

    cout<<"max :"<<min;
    cout<<"min :"<<max;

    return 0;
}
```
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
