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
int vertikal(char* z){
	int f;
	char v1[]="tajabreaaoqlmpo", 
		 v2[]="galsweezznbqodh", 
		 v3[]="buwapwoccofzscn", 
		 v4[]="wncglntggprqgrk", 
		 v5[]="wtqmogweekonzzz", 
		 v6[]="itlqtoosswgnzmw", 
		 v7[]="nmduadswwmmmzsa", 
		 v8[]="tmzwnjbeeparent", 
		 v9[]="ehmvacqwwamztge", 
		 v10[]="rfpvdphnnrwjdrr",
		 v11[]="wombtnaaakpjbdj", 
		 v12[]="sovsparkktwsong", 
		 v13[]="eddogtrnnzecort", 
		 v14[]="snmhnnsppceltpr", 
		 v15[]="nbrickabbcygoza",
	 	 *pv[]={v1,v2,v3,v4,v5,v6,v7,v8,v9,v10,v11,v12,v13,v14,v15};
	for(int x=0;x<15;x++){
		if (strstr(*(pv+x),z) != '\0' ||(strstr(strrev(*(pv+x)), z) > 0))
		{
		f++;
		}
	}
	if(f==0)
		return 0;
	else
		return 1;	
}
int diagonal1(char *z){
	int f;
	char d1[]="t",
		 d2[]="ag",
		 d3[]="jab",
		 d4[]="aluw",
		 d5[]="bswnw", 
		 d6[]="rwacti",
		 d7[]="eepgqtn", 
		 d8[]="aewlmlmt", 
		 d9[]="dzonoqdme", 
		 d10[]="oictgtuzhr", 
		 d11[]="qnngwoawmfw", 
		 d12[]="lboneodnvpos", 
		 d13[]="mqfpessjavmoe", 
		 d14[]="pozrkrwbcdbvds", 
	         d15[]="odsqowqeqptsdnn",
		 d16[]="hcgngmowhnpomb", 
		 d17[]="nrznmpdnaaghr", 
		 d18[]="kzcmaalartni", 
		 d19[]="zmzrmrwkrnc", 
		 d20[]="wsezwkdnsk", 
		 d21[]="antjptcpa", 
		 d22[]="tgdjwzab", 
		 d23[]="erbsecr", 
		 d24[]="rdocec",
		 d25[]="jnoly", 
		 d26[]="grtg", 
		 d27[]="tpo", 
		 d28[]="rz", 
		 d29[]="a",
		 *pd1[]={d1,d2,d3,d4,d5,d6,d7,d8,d9,d10,d11,d12,d13,d14,d15,d16,d17,d18,d19,d20,d21,d22,d23,d24,d25,d26,d27,d28,d29};
	for(int x=0;x<29;x++){
		if (strstr(*(pd1+x),z) != '\0' ||(strstr(strrev(*(pd1+x)), z) > 0))
		{
		f++;
		}}
	if(f==0)
		return 0;
	else
		return 1;	
}
int diagonal2(char *z){
	int f;
	char dd1[]="n",
		 dd2[]="sb", 
		 dd3[]="enr", 
		 dd4[]="sdmi", 
		 dd5[]="wodhc", 
		 dd6[]="rovonk", 
		 dd7[]="efmsgna", 
		 dd8[]="thpbptsb", 
		 dd9[]="nmmvtarpr",
		 dd10[]="imzvdnrnac", 
		 dd11[]="wtdwapakccy", 
		 dd12[]="wtlunchadzeg", 
		 dd13[]="bnqqajqnwtelo", 
		 dd14[]="gucmtdbwlkwctz", 
		 dd15[]="tawgoosedrpsopa", 
		 dd16[]="alalgowoawjorr", 
		 dd17[]="jspnwsqpmjbnt", 
		 dd18[]="awwtermazddg", 
	         dd19[]="beogewmrtrj", 
		 dd20[]="recnkgmegr", 
		 dd21[]="eznponzne", 
