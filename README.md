
#include<iostream>

using namespace std ;

int main(){

 int n,aux;
 cout<<"Ingrese la cantidad de numeros :";
 cin>>n;
 int V[n];
 for(int i=0;i<n;i++){
  cout<<"\n Numero "<<i+1<<" = ";
  cin>>V[i]
 }

 for(int i=0;i<n;i++){
  for(int j=i+1;j<n;j++){
   if(V[j]>V[j+1]){
    aux=V[j];
    V[i]=V[j+1];
    V[j+1]=aux;
    
   }
  }
 }

 cout<<"Elementos Ordenados:"<<endl;
 for(int i=0;i<n;i++){
  cout<<V[i]<<endl;
 }

 return 0;
}
