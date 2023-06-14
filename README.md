#include <iostream>
#include <conio.h>
#include <math.h>
using namespace std;
main(){
	int tipo,operacion;
	float a,b,res;
	char opc;
	
	cout<<"MENU"<<endl;
	cout<<"1)suma"<<endl;
	cout<<"2)resta"<<endl;
	cout<<"3)multiplicacion"<<endl;
	cout<<"4)division"<<endl;
	cout<<"seleccionar tipo"<<endl;
	cin>>tipo;
	if(tipo!=1&&tipo!=2&&tipo!=3&&tipo!=4){
		cout<<"ERROR";
	}

	else{
	cout<<"seleccione numero"<<endl;
	cin>>a;
	cout<<"seleccione numero2"<<endl;
	cin>>b;
	switch(tipo){
		case 1:
			res=a+b;
			break;
		case 2:
			res=a-b;
			break;
		case 3:
			res=a*b;
			break;
		case 4:
			cout<<"a)resultado"<<endl;
			cout<<"b)residuo"<<endl;
			cout<<"seleccionar operacion"<<endl;
			cin>>opc;
			
			if(opc=='a'){
				if(b==0||a==0){
					cout<<"No se puede dividir entre 0";
				}
				else{
			res=a/b;
		}
			}
			else if(opc=='b'){
				res=fmod(a, b);
			}
			break;
			cout<<" resultado de la opreccion: "<<res<<endl;
			getch();
			
	}
	cout<<"resultado de la opreacion"<<res<<endl;
			getch();
}
}
