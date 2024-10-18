#include <bits/stdc++.h>
using namespace std;

class Solution {
  public:
    int binarysearch(vector<int> &arr, int k) {
        int low = 0;
        int high = arr.size()-1;
        while(low<=high)
        {
            int mid = (low+high)/2;
            if(arr[mid]>k)
            {
                high = mid-1;
            }
            else if(arr[mid]<k)
            {
                low = mid+1;
            }
            else
            {
                return mid;
            }
        }
        return -1;
    }
};

int main() {
    int t;
    cin >> t;
    while (t--) {
        int k;
        cin >> k;
        vector<int> arr;
        string input;
        cin.ignore();
        getline(cin, input);
        stringstream ss(input);
        int number;
        while (ss >> number) {
            arr.push_back(number);
        }
        Solution ob;
        int res = ob.binarysearch(arr, k);
        cout << res << endl;
    }
    return 0;
}
