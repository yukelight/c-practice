# c-practice-折半查询
#include<iostream>
using namespace std;
char *Char_cut(char s[]){
	int i, k,j;
	i=0;
	while(s[i]==' '){
		i++;
	}
	j=i;
	while(s[j]!='\0'){
		s[j-i]=s[j];
		j++;
	}
	s[j-i]='\0';
	return s;
}
int main(){
	char str[100];
	cout<<"type please"<<endl;
	cin.getline(str,99);
	cout<<Char_cut(str)<<endl;
	
}
