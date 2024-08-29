#include <iostream>

using namespace std;

// Function to find the maximum number of shops that can be opened
int no_of_shops(int S[], int E[], int k, int n) {
    int cnt = 0;
    int arr[k] = {0}; // Array to keep track of the end times of shops

    for (int i = 0; i < n; i++) {
        int start = S[i];
        int end = E[i];

        for (int j = 0; j < k; j++) {
            if (arr[j] <= start) {
                arr[j] = end;
                cnt++;
                break;
            }
        }
    }

    return cnt;
}

int main() {
    int S[] = {1, 2, 3}; // Start times of shops
    int E[] = {3, 4, 5}; // End times of shops
    int k = 2;           // Number of persons

    cout << "Max shops that can be visited: " << no_of_shops(S, E, k,3 ) << endl;

    return 0;
}
