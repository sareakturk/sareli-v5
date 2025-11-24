# sareli-v5
#include <iostream>
#include <string>
using namespace std;

string UcusGuvenlıgıKontrolu (int yuk, int hiz, int yukseklık) {

int pil = 100; // Baslangıc pil seviyesi
pil -= (hiz /10) *5; // pil değerine gore pil seviyesi

cout << "Hesaplanan pil seviyesi"  << pil << endl;

// 1. yuk konrtolu
if (yuk > 500) {

    return "Agır Yuk, Ucamaz";
}

// 2. pil seviyesi kontrolü

else if (pil< 30){
    return "Pil seviyesi yetersiz ucarsan dusersin";
}

// 3. yukseklık kontrolu
else if ( yukseklık > 200) {
    return "Radar sinyali disindasiniz ucarsaniz dusersiniz";
}

else if (yukseklik < 20) {
    return "Yukseklik guvenli LUTFEN ucun";

}
// tum kosullar
else {
    return "Ucus guvenli";
}
int main () {
   const int dronSayisi = 3;
   int yukler [dronSayisi];
   int hizlar [dronSayisi];
   int yukseklıkler [ droneSayisi];

   cout << "Mini dron surusu ucus guvenlıgı programı" << endl;

   // kullanici verileri diziye girio . yukseklık hiz pil sayısı vb.
   for ( int i = 0; i<dronSayisi; i++) {
 cout << "/nDrone" << i+1 << "bilgileri giriniz: " endl;
 cout << "Yuk (gram): ";
 cin >> yukler [i];
 cout << "Hiz (m/s): ";
 cin >> hizlar [i];
 cout "Yukseklık (m): ";
 cin >> yukseklık [i];

   }
     cout << "/n dron surusu ucus durumları " << endl;

     //Her dron ıcın sonucu hesapla ve yazdır
     for (int i=0; i<dronSayisi; i++ ) {
        string sonuc = UcusGuvenlıgıKontrolu(yukler [1], hizlar[i], yukseklıkler[i];
        cout <<"Drone" << i+1 << ":  " << sonuc << endl;


     }






















}




















}
