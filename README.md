 public:
    //Function to find the first non-repeating character in a string.
    char nonrepeatingCharacter(string S)
    {
       //Your code here
       int i;
       map<char,int>m;
       int n=S.length();
       char d='$';
       for(i=0;i<n;i++){
           m[S[i]]++;
       }
       for(i=0;i<n;i++){
           if(m[S[i]]==1){
               return S[i];
           }
       }
       return d;
    }
