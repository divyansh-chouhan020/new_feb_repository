#include <iostream>
using namespace std ;//check whether the elemnt is equal to the sum or not 
int main()
{
    int arr[]={-3,-1,0,4,6,7,9,3556};
    int size =sizeof (arr )/sizeof(int);
      int left =0;
      int right =size-1;
      int x ;
      cin >>x;
      while (left < right)
      {
        if (arr[left]+arr[right]<x)
        {
            left++;
        }
        else if (arr[left]+arr[right]>x)
        {
            right--;
        }
        else if (arr[left]+arr[right]==x)
        {
            cout <<"yes "<<"at index "<<left <<" "<<right;
            break;
        }

        };

}

