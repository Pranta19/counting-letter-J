#include <bits/stdc++.h>
using namespace std;

int main() {
    string s;
    cin >> s;
    
    int freq[26] = {0}; // Initialize the array to store the frequency of each letter
    
    // Count the occurrences of each character
    for (char c : s) {
        freq[c - 'a']++;
    }

    // Print the characters and their frequencies in ascending order
    for (int i = 0; i < 26; i++) {
        if (freq[i] > 0) {
            cout << char(i + 'a') << " : " << freq[i] << endl;
        }
    }

    return 0;
}
