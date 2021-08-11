// Corregimos los cinco errores que se presentan en el programa
#include<iostream>

using namespace std ;

int main(){
// solicitamos al usuario que ingrese la cantidad de numeros a ordenar
 int n,aux;
 cout<<"Ingrese la cantidad de numeros :";
 cin>>n;
 int V[n];
 for(int i=0;i<n;i++){
  cout<<"\n Numero "<<i+1<<" = ";
  cin>>V[i];
 }
// definimos la burbuja
 for(int i=0;i<n;i++){
  for(int j=i+1;j<n;j++){
   if(V[j]>V[i]){
    aux=V[j];
    V[j]=V[i+1];
    V[i+1]=aux;
    
   }
  }
 }
// Ordenamos los numeros
 cout<<"Elementos Ordenados:"<<endl;
 for(int i=0;i<n;i++){
  cout<<V[i]<<endl;
 }

 return 0;
}
