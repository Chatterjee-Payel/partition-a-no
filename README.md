# partition-a-no
public:
    string stringPartition(string S, int a, int b){
        // code here 
         for(int i=1;i<S.size();i++)
         {
           string res1=S.substr(0,i);
           string res2=S.substr(i,S.size()-1);
           if(stoi(res1)%a==0 && stoi(res2)%b==0)
           {
               return res1+" "+res2;
           }
         }
         return "-1";
         
    }
};
