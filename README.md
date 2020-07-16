#include<iostream>
using namespace std;
int diskonn (){
  float bayar, diskon,total,uang,kembalian;
  cout << "==========================\n";
  
  cout << "Masukkan total Pembelian: ";
  cin >> bayar;
   if (bayar>500000){
   	diskon=bayar*0.10;
    total=bayar-diskon;
	cout<<endl<<"selamat anda mendapatkan diskon 10%"<<endl;
   }
   else{
   	total=bayar;
   	cout<<"Maaf anda tidak mendapat diskon"<<endl;
   }
  cout << "==========================\n";
  cout << "Jumlah potngan :"<<diskon<<endl;
  cout << "Total yang harus bayar: " <<total<<endl;
  cout << "uang konsumen :";cin>>uang;
  if (uang>=total){
  kembalian=uang-total;
  cout << "uang kembalian: "<<kembalian<<endl;
  }
  else{
  	cout<<"uang anda tidak cukup";
  } 
}
int main(){
	diskonn();
	return 0;
}
