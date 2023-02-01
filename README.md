

#include<iostream>

using namespace std;

int main()
{
	string module[6]= {"Mathematics","Biology","Physics","Chemistry","Communication_English","Programming101"};
	int creditValue[6]={120,120,130,110,90,120};
	int studA_Marks[6]={60,74,54,80,62,45};
	int ct = 690;
	int fm=0,cpt=0; //decalring final mark(fm) and Cumulative pass score(cps)
	//calculate Cumulative pass score for Student A
	
	//calculate total final mark
	for(int i=0;i<=5;i++)
	{
		fm=fm+studA_Marks[i];
		
	}
	//calculate cummulative pass core/ total percentage
	cpt=(fm*100)/ct;
	cout<<"Cummulative pass score for student A is "<<cpt<<endl;
	
	//determine GPA score
	if(cpt>=80 && cpt<=100)
	{
		cout<<"Your GPA is 4.0"<<endl;
	}
	else if(cpt>=60 and cpt<=79)
	{
		cout<<"Your GPA is 3.0 "<<endl;
	}
	else if(cpt>=50 && cpt<=59)
	{
		cout<<"Your GPA is 2.0"<<endl;
	}
	else if(cpt>=40 && cpt<=49)
	{
		cout<<"Your GPA is 1.0"<<endl;
	}
	else if(cpt>=0 && cpt<=39)
	{
		cout<<"Your GPA is "<<endl;
	}
  
  return 0;
}
