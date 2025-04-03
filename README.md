# 59A-WORD-PROB-ON-CODEFORCES

#include <bits/stdc++.h>
using namespace std;

int main() {
    string s;
    cin >> s;
    
    int dom = 0;
    
    for (int i = 0; i < s.size(); i++) {
        if (isupper(s[i])) dom++;
        else dom--;
    }

    if (dom > 0) {
        for (auto &c : s) c = toupper(c);  // Convert all to uppercase
    } else {
        for (auto &c : s) c = tolower(c);  // Convert all to lowercase
    }

    cout << s << endl;

    return 0;
}
