###Day5

##T1

#WA*2

#没仔细省题，没看到格格数据是之间不用加空格于是wa两次（还以为是IOS流的问题QWQ）

#Code:
#include<bits/stdc++.h>
using namespace std;

int main()
{
  int k,n;cin >>n >>k;
  for(int q=0;q <n;q++)
    if(q <k)cout <<1;
    else cout <<4;

  return 0;
}


##T2

#AC

#code：
#include<bits/stdc++.h>
using namespace std;

const int Max = 1e5 +5;

struct WOW_IS
{
  int n,m,k;
  void UWU()
  {
    cin >>n;

    for(int q=2;q <=n ;q+=2)
      cout <<q <<" ";

    for(int q=1;q <=n ;q+=2) 
      cout <<q <<" ";
    
    cout <<endl;
  }
};

int main()
{
  ios::sync_with_stdio(0);
  cin.tie(0);cout.tie(0);

  int T;cin >>T;
  while(T--)
  {
    WOW_IS OWO;
    OWO.UWU();
  }
  return 0;
}


/*       |   |
      ___|___|___
_____    |   |
|   |  _________
|___|  |   |   |
       |___|___|
       |   |   |
       |___|___|
*/


##T3

#AC

#code:
#include<bits/stdc++.h>
using namespace std;

const int Max = 1e5 +5;

struct WOW_IS
{
  int n,m,a,b,c;
  void UWU()
  {
    cin >>a >>b >>c;
    cout <<100 <<endl;
    for(int q=0;q <50;q++)
      cout <<a  <<" ";
    for(int q=50;q <95;q++)
      cout <<b  <<" ";
    for(int q=95;q <99;q++)
      cout <<c  <<" ";
    cout << (int)1e9<<endl;
  }
};

int main()
{
  ios::sync_with_stdio(0);
  cin.tie(0);cout.tie(0);

  WOW_IS OWO;
  OWO.UWU();

  return 0;
}



##T4

#AC

#Code:
#include<bits/stdc++.h>
using namespace std;

const int Max = 1e3 +5;

struct WOW_IS
{
  int n,m,k;
  int num[Max][Max] ;
  void UWU()
  {
    cin >>n >>m;
    puts("Yes");
    int cnt = 0;
    for(int y=1;y <=m;y++)
      for(int x=1;x <= min(n,y);x++)
        num[x][y - x + 1] = ++cnt;
    
    for(int x =2;x <=n;x++)
      for(int y = 0;y <m &&  y + x <=n;y++)
        num[x + y][m - y] = ++cnt;

    for(int q=1;q <=n;q++)
    {
      for(int w=1;w <=m;w++)
        cout <<num[q][w] <<" ";
      cout <<endl;
    }
  }
};

int main()
{

  int T;cin >>T;
  while(T--)
  {
    WOW_IS OWO;
    OWO.UWU();
  }
  return 0;
}


/*       |   |
      ___|___|___
_____    |   |
|   |  _________
|___|  |   |   |
       |___|___|
       |   |   |
       |___|___|
*/


##T5

#AC

#Code:#include<bits/stdc++.h>
using namespace std;

const int Max = 1e5 +5;

struct WOW_IS
{
  int n,m,k;
  void UWU()
  {
    cin >>n;
    if(n == 2){cout <<"1 2\n";return;}
    if(n == 4){cout <<-1 <<endl;return ;}
    for(int q=1;q <(n + (n%2?3:4))/2;q++)
      cout <<q <<" "<<q+1 <<endl;
    for(int q=2;q <=(n - (n%2?1:2))/2 ;q++)
      cout <<q <<" "<<n/2+1 + q<<endl;
  }
};

int main()
{


  int T;cin >>T;
  while(T--)
  {
    WOW_IS OWO;
    OWO.UWU();
  }
  return 0;
}


/*       |   |
      ___|___|___
_____    |   |
|   |  _________
|___|  |   |   |
       |___|___|
       |   |   |
       |___|___|
*/

##T6

#AC

#Code:
#include<bits/stdc++.h>
using namespace std;

const int Max = 1e5 +5;

struct WOW_IS
{
  int n,m,k;
  void UWU()
  {
    cin>>n;
    if(n ==1 || (n%4 == 0)){puts("impossible");return;}

    cout <<"1 0 ";
    
    for(int q=2;q <n;q++)
    {
      if(q%4 == 3)
      {
        cout <<q +1<<" "<<q<<" ";
        q++;
      }
      else cout <<q <<" ";
    }
    cout <<endl;

  }
};

int main()
{
  int T;cin >>T;
  while(T--)
  {
    WOW_IS OWO;
    OWO.UWU();
  }
  return 0;
}


/*       |   |
      ___|___|___
_____    |   |
|   |  _________
|___|  |   |   |
       |___|___|
       |   |   |
       |___|___|
*/

##T7

#AC

#Code:
#include<bits/stdc++.h>
using namespace std;

const int Max = 1e5 +5;

struct WOW_IS
{
  int n,m,k;
  void UWU()
  {
    cin>>n;
    if(n ==1 || (n%4 == 0)){puts("impossible");return;}

    cout <<"1 0 ";
    
    for(int q=2;q <n;q++)
    {
      if(q%4 == 3)
      {
        cout <<q +1<<" "<<q<<" ";
        q++;
      }
      else cout <<q <<" ";
    }
    cout <<endl;

  }
};

int main()
{
  int T;cin >>T;
  while(T--)
  {
    WOW_IS OWO;
    OWO.UWU();
  }
  return 0;
}


/*       |   |
      ___|___|___
_____    |   |
|   |  _________
|___|  |   |   |
       |___|___|
       |   |   |
       |___|___|
*/


##T8

#AC

#Code:
#include<bits/stdc++.h>
using namespace std;

const int Max = 55;

struct WOW_IS
{
  int n,m,k;
  int uwu[Max][Max] = {};
  void UWU()
  {
    cin >>n >>k;
    if(k <n || k >n *(n-1) + 1){puts("No");return;}
    puts("Yes");
    
    uwu[1][1] = k;
    int cnt1 = n * n,cnt2 = 1;
    for(int q=2;q <=n;q++)
      uwu[q][q] = cnt1--;
    for(int q=1; q<=n;q++)
      for(int w=1;w <=n;w++)
      {
        if(q == w)continue;
        if(cnt2 == k)cnt2++;
        uwu[q][w] = cnt2++;
      }
    for(int q=1;q <=n;q++)
    {
      for(int w=1;w <=n;w++)
        cout <<uwu[q][w] <<" ";
      cout <<endl;
    }
  }
};

int main()
{

  int T;cin >>T;
  while(T--)
  {
    WOW_IS OWO;
    OWO.UWU();
  }
  return 0;
}


/*       |   |
      ___|___|___
_____    |   |
|   |  _________
|___|  |   |   |
       |___|___|
       |   |   |
       |___|___|
*/


##T9


#AC

#Code:
#include<bits/stdc++.h>
using namespace std;

const int Max = 55;

struct WOW_IS
{
  int n,m;
  int num[Max][Max];
  int cnt = 0;
  void UWU()
  {
    cin >>n;
    puts("Yes");
    num[1][1] = 1;num[1][2] = 2;num[2][1] =3;num[2][2] = 4;
    int cnt = 4;
    for(int q=3;q <=n;q++)
    {
      cnt ++;
      for(int w= 1;w <q;w++)
        num[q][w] = num[w][q] = cnt;
      num[q][q] = ++cnt;
    }
    for(int q=1;q <=n;q++)
    {
      for(int w=1;w <=n;w++)
        cout <<num[q][w] <<" ";
      cout <<endl;
    }
  }
};

int main()
{

  WOW_IS OWO;
  OWO.UWU();

  return 0;
}
/*       |   |
      ___|___|___
_____    |   |
|   |  _________
|___|  |   |   |
       |___|___|
       |   |   |
       |___|___|
*/


##J

#WA*4

#后三个char不为">>>"的情况没判断对，后来直接substr过了

Code：
#include<bits/stdc++.h>
using namespace std;

const int Max = 1e5 +5;

struct WOW_IS
{
  string s;
  void out()
  {
    cout <<"No" <<endl;
    return ;
  }
  void UWU()
  {
    cin >>s;
    s = " "+s;
    int n = s.size(); 
    int end = n;
    for(;end >=0;end--)
      if(s[end] == '-')
        break;
    end++;
    // cout <<end <<endl;
    // cout <<s.substr(n-3,3)<<endl;
    if(s[1]=='-' ||end <=2 || s.substr(n-3,3)!=">>>" )
    {
      cout <<"No" <<endl;
      return;
    }
    int m =0;
    for(int q=2;q <end;q++)
      if(s[q] == '>')m++;
    
    for(int q= n-3;q >=end;q--)
      m++;

    cout <<"Yes " <<m <<endl;

    for(int q= n-3;q >=end;q--)
      cout <<1 <<" "<<q +2<<endl;
    
    for(int q=2;q <end;q++)
      if(s[q] == '>')
        cout <<q <<" "<<end +2 - q +1<<endl;
  
  }
};

int main()
{
  ios::sync_with_stdio(0);
  cin.tie(0);cout.tie(0);

  int T;cin >>T;
  while(T--)
  {
    WOW_IS OWO;
    OWO.UWU();
  }
  return 0;
}


/*       |   |
      ___|___|___
_____    |   |
|   |  _________
|___|  |   |   |
       |___|___|
       |   |   |
       |___|___|
*/


##T11

#willAC (run


