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
		 		 vr8[]="tnerapeebjnwzmt",
		 vr9[]="egtzmawwqcavmhe",
		 vr10[]="rrdjwrnnhpdvpfr",
		 vr11[]="jdbjpkaaantbmow",
		 vr12[]="gnoswtkkrapsvos",
		 vr13[]="troceznnrtgodde",
		 vr14[]="rptlecppsnnhmns",
		 vr15[]="azogycbbakcirbn",
	 	 *pv[]={v1,v2,v3,v4,v5,v6,v7,v8,v9,v10,v11,v12,v13,v14,v15,vr1,vr2,vr3,vr4,vr5,vr6,vr7,vr8,vr9,vr10,vr11,vr12,vr13,vr14,vr15};

	for(int x=0;x<30;x++){
		if (strstr(*(pv+x),z) != '\0'){
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
		 dr1[]="zr", 
		 dr2[]="opt", 
		 dr3[]="gtrg", 
		 dr4[]="ylonj", 
		 dr5[]="cecodr", 
		 dr6[]="rcesbre", 
		 dr7[]="bazwjdgt", 
		 dr8[]="apctpjtna", 
		 dr9[]="ksndkwzesw", 
		 dr10[]="cnrkwrmrzmz", 
		 dr11[]="intralaamczk",
		 dr12[]="rhgaandpmnzrn", 
		 dr13[]="bmopnhwomgngch",
		 dr14[]="nndstpqeqwoqsdo",
		 dr15[]="sdvbdcbwrkrzop", 
		 dr16[]="eomvajssepfqm", 
		 dr17[]="sopvndoenobl", 
		 dr18[]="wfmwaowgnnq",
		 dr19[]="rhzutgtcio", 
		 		 dr20[]="emdqonozd", 
		 dr21[]="tmlmlwea", 
		 dr22[]="ntqgpee",
		 dr23[]="itcawr", 
		 dr24[]="wnwsb", 
		 dr25[]="wula", 
		 dr26[]="baj", 
		 dr27[]="ga", 
		 *pd1[]={d1,d2,d3,d4,d5,d6,d7,d8,d9,d10,d11,d12,d13,d14,d15,d16,d17,d18,d19,d20,d21,d22,d23,d24,d25,d26,d27,d28,d29,
		         dr1,dr2,dr3,dr4,dr5,dr6,dr7,dr8,dr9,dr10,dr11,dr12,dr13,dr14,dr15,dr16,dr17,dr18,dr19,dr20,dr21,dr22,dr23,dr24,dr25,dr26,dr27};
		 
	for(int x=0;x<56;x++){
		if (strstr(*(pd1+x),z) != '\0'){
		f++;
		}
	}
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
		 dd22[]="aiorncst", 
		 dd23[]="dnfqzma", 
		 dd24[]="obzgzw", 
		 dd25[]="qqsrz", 
		 dd26[]="lock", 
		 dd27[]="mdn", 
		 dd28[]="ph", 
		 dd29[]="o",
		 ddr1[]="bs",
		 ddr2[]="rne",
		 ddr3[]="imds",
		 ddr4[]="chdow",
		 ddr5[]="knovor",
		 ddr6[]="angsmfe",
		 ddr7[]="bstpbpht",
		 ddr8[]="rpratvmmn",
		 ddr9[]="canrndvzmi",
		 ddr10[]="ycckapawdtw", 
		 ddr11[]="gezdahcnultw",
		 ddr12[]="oletwnqjaqqnb",
		 ddr13[]="ztcwklwbdtmcug",
		 ddr14[]="aposprdesoogwat", 
		 ddr15[]="rrojwaowoglala",
		 ddr16[]="tnbjmpqswnpsj",
		 ddr17[]="gddzamretwwa",
		 ddr18[]="jrtrmwegoeb",
