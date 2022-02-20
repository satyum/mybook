# mybook

# kth max 
```c++
#include<bits/stdc++.h>

using namespace std;

int main()
{
int n;
cin>>n;
int k;
cin>>k;
vector<int>arr(n);
	for(int i=0;i<n;++i)
		{
			cin>>arr[i];
		}	
	sort(arr.begin(),arr.end());
	cout<<arr[k-1];
	
}

```
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

```c++
#include <bits/stdc++.h>
using namespace std;

# sort 0 1 2 
int main()
{
	int n;
	cin>>n;
	int arr[n];
	int low=0,mid=0,high=n-1;
	for(int i=0;i<n;++i)
	{
		cin>>arr[i];
	}
	while(mid<=high)
	{
			if(arr[mid]==0)
			{
			swap(arr[mid++],arr[low++]);
			}
			else if(arr[mid]==1)
			{
			mid++;
			}
			else if(arr[mid]==2)
			{
			swap(arr[mid],arr[high--]);
			}
	}
	for(int i=0;i<n;++i)
	{
		cout<<arr[i];
	}
	
}
```
## sort negative and positive
```c++
#include<bits/stdc++.h>

using namespace std;

int main()
{
	int n;
	cin>>n;
	vector<int>arr(n);
	for(int i=0;i<n;++i)
		{
			cin>>arr[i];
		}
	int l=0,r=n-1;
	while(l<r)
	{
		if(arr[l]<0 && arr[r]<0) l++;
		
		else if(arr[l]>0 && arr[r]>0) r--;
		
		else if(arr[l]>0 && arr[r]<0)
		{
				swap(arr[l++],arr[r--]);
		}else
		{
			l++;
			r--;	
		}
		
	}
	for(int i=0;i<n;++i)
		{
			cout<<arr[i];
		}
}
```
## cyclic rotate
```c++

void rotate(int arr[], int n)
{
    int left=0,right=n-1;
    while(left<right)
    {
        swap(arr[left],arr[right]);
        left++;
    }
```
