# sorting-in-DSA
#include<bits/stdc++.h>
using namespace std;
/*void bubbleSort(int arr[],int n){
    for(int i=0;i<n-1;i++)
    {
        for(int j=0;j<n-1-i;j++)
        {
            if(arr[j]>arr[j+1])
            {
                swap(arr[j],arr[j+1]);
            }
        }
    }
    return;
}*/
/*void selectionSort(int arr[],int n)
{
    for(int i=0;i<n-1;i++)
    {
        int min_index=i;
        for(int j=i+1;j<n;j++)
        {
            if(arr[j]<arr[min_index])
            {
                min_index=j;
            }
        }
        if(min_index!=i)
        {
            swap(arr[i],arr[min_index]);
        }
    }
    return;
}*/
/*void insertionSort(int arr[],int n)
{
    for(int i=1;i<n;i++)
    {
        int curr=arr[i];
        int j=i-1;
        while(j>0 && arr[j]>curr)
        {
            arr[j+1]=arr[j];
            j--;
        }
        arr[j+1]=curr;
    }
    return;
}*/
/*int partition(int arr[],int first,int last)
{
    int pivot=arr[last];
    int i=first-1;
    for(int j=first;j<last-1;j++)
    {
        if(arr[j]<pivot)
        {
            i++;
            swap(arr[i],arr[j]);
        }
    }
    swap(arr[i+1],arr[last]);
    return i+1;
}
void quickSort(int arr[],int first,int last)
{
    if(first>=last)
    {
        return;
    }
    int pi=partition(arr,first,last);
    quickSort(arr,first,pi-1);
    quickSort(arr,pi+1,last);
}*/
/*int merge(int arr[],int l,int mid,int r)
{
    int an=mid-l+1;
    int bn=r-mid;
    int a[an];
    int b[bn];
    for(int i=0;i<an;i++)
    {
        a[i]=arr[l+i];
    }
    for(int j=0;j<bn;j++)
    {
        b[j]=arr[mid+1+j];
    }
    int i=0,j=0,k=l;
    while(i<an && j<bn)
    {
        if(a[i]<b[j]){
            arr[k++]=a[i++];
        }
        else{
            arr[k++]=b[j++];
        }
    }
    while(i<an){
        arr[k++]=a[i++];
    }
    while(j<bn)
    {
        arr[k++]=b[j++];
   }
}
void mergeSort(int arr[],int l,int r)
{
    if(l>=r)
    {
        return;
    }
    int mid=(l+r)/2;
    mergeSort(arr,l,mid);
    mergeSort(arr,mid+1,r);
    merge(arr,l,mid,r);
}*/
int main()
{
    int arr[]={9,6,4,3,45,78,23};
    int n=sizeof(arr)/sizeof(arr[0]);
    //bubbleSort(arr,n);
    //selectionSort(arr,n);
    //insertionSort(arr,n);
    //quickSort(arr,0,n-1);
   //mergeSort(arr,0,n-1);
    for(int i=0;i<n;i++)
    {
        cout<<arr[i]<<" ";
    }
    return 0;
}
