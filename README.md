//# findwords
//tugas mencari kata
//Evania Intiha (1817051044)
//Nadhira Lua Zhafira (1817051043)
//Azzah Roudhoh (1857051001)
//Agnes Pramudani (1857051004)

#include <iostream>
#include <cstring>
using namespace std;

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
		 ab[]="nseswretniwwbgt",
		 ab1[]="bndoofhmmttnuaa",
		 ab2[]="rmdvmpmzdlqcwlj",
		 ab3[]="ihosbvvwuqmgasa",
		 ab4[]="cngptdanatolpwb",
		 ab5[]="kntanpcjdognwer",
		 ab6[]="asrrahqbsowtoee",
		 ab7[]="bpnkanwewsegcza",
		 ab8[]="racdwldoqrennid",
		 ab9[]="ccztkrapmwkpono",
		 ab10[]="yeewpwmamgorfbq",
		 ab11[]="glcsjjzrmnnqzql",
		 ab12[]="otoobdtezczgsom",
		 ab13[]="zprndrgnsmzrcdp",
		 ab14[]="artgjretawzknho",
		 *pa[]={a,a1,a2,a3,a4,a5,a6,a7,a8,a9,a10,a11,a12,a13,a14,ab,ab1,ab2,ab3,ab4,ab5,ab6,ab7,ab8,ab9,ab10,ab11,ab12,ab13,ab14};
	for(int x=0;x<30;x++){
		if (strstr(*(pa+x),z) != '\0'){
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
		 vr1[]="opmlqoaaerbajat",
		 vr2[]="hdoqbnzzeewslag", 
		 vr3[]="ncszfoccowpawub",
		 vr4[]="krgqrpggtnlgcnw",
		 vr5[]="zzznokeewgomqtw",
		 vr6[]="wmzngwssootqlti",
		 vr7[]="aszmmmwwsdaudmn",
