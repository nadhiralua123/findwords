//# findwords
//tugas mencari kata
//Evania Intiha (1817051044)
//Nadhira Lua Zhafira (1817051043)
//Azzah Roudhoh (1857051001)
//Agnes Pramudani (1857051004)

#include <iostream>
#include <cstring>
using namespace std;
#include <iostream>
#include <cstring>
using namespace std;
const int r=15,c=15;
char az[r][c] = {{'t','g','b','w','w','i','n','t','e','r','w','s','e','s','n'},
	{'a','a','u','n','t','t','m','m','h','f','o','o','d','n','b'},
    {'j','l','w','c','q','l','d','z','m','p','m','v','d','m','r'},
    {'a','s','a','g','m','q','u','w','v','v','b','s','o','h','i'},
    {'b','w','p','l','o','t','a','n','a','d','t','p','g','n','c'},
    {'r','e','w','n','g','o','d','j','c','p','n','a','t','n','k'},
    {'e','e','o','t','w','o','s','b','q','h','a','r','r','s','a'},
    {'a','z','c','g','e','s','w','e','w','n','a','k','n','p','b'},
    {'d','i','n','n','e','r','q','o','d','l','w','d','c','a','r'},
    {'o','n','o','p','k','w','m','p','a','r','k','t','z','c','c'},
    {'q','b','f','r','o','g','m','a','m','w','p','w','e','e','y'},
    {'l','q','z','q','n','n','m','r','z','j','j','s','c','l','g'},
    {'m','o','s','g','z','c','z','e','t','d','b','o','o','t','o'},
    {'p','d','c','r','z','m','s','n','g','r','d','n','r','p','z'},
    {'o','h','n','k','z','w','a','t','e','r','j','g','t','r','a'}};
int horizontal(char* z){
	int f;
	char a[]="tgbwwinterwsesn",
		 a1[]="aaunttmmhfoodnb",
		 a2[]="jlwcqldzmpmvdmr",
		 a3[]="asagmquwvvbsohi",
		 a4[]="bwplotanadtpgnc",
		 a5[]="rewngodjcpnatnk",
		 a6[]="eeotwosbqharrsa",
		 a7[]="azcgeswewnaknpb",
		 a8[]="dinnerqodlwdcar",
		 a9[]="onopkwmparktzcc",
		 a10[]="qbfrogmamwpweey",
		 a11[]="lqzqnnmrzjjsclg",
		 a12[]="mosgzczetdbooto",
		 a13[]="pdcrzmsngrdnrpz",
		 a14[]="ohnkzwaterjgtra",
		*pa[]={a,a1,a2,a3,a4,a5,a6,a7,a8,a9,a10,a11,a12,a13,a14};
	for(int x=0;x<15;x++){
		if (strstr(*(pa+x),z) != '\0' ||(strstr(strrev(*(pa+x)), z) > 0))
        {
		f++;
		}
	}
	if(f==0)
		return 0;
	else
		return 1;	
}
