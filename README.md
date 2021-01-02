# codes
All the codeing question and their solution are presesnt which are asked in the interview of different company from different site.

MY HackerRank certificate
1. https://www.hackerrank.com/certificates/10ffb7afaec5
2. https://www.hackerrank.com/certificates/16ac92c64e30

Coding Problems:-
1. Morse Problem
2. Count All Palindrome Sub-Strings in a String
3. Next Smallest palindrome
4. Next Greatest Palindrome
5. All sorting algorithms
6. Linear and binary search
7. Find next greater number with same set of digits

// For running code faster.
#pragma GCC optimize ("O2")


arr = list(map(int, input().split()))


Finding prime best logic

 int countPrimes(int n) {
        if(n<=2)
            return 0;
        
        vector<bool> vect(n);
        fill(vect.begin()+2,vect.end(), true);
        int count=1;
        for(int i=2; i*i<n;i++){
            if(!vect[i]) continue;
            for(int j = i*i;j<n;j+=i)
                vect[j]=false;
        }
        for(int i=3;i<n;i+=2){
            if(vect[i])
                count++;
        }
        
        return count;
    }


Work of split() in c++

vector<string> str1;
        string str2="";
        for(char c : s){
            if(c == ' '){
                str1.push_back(str2);
                str2 = "";
                continue;
            }
            str2+=c;
        }
        str1.push_back(str2);
 
 
 For Finding maximum in c++ for any number of variables.
 cout<<max({1,2,3,...});
