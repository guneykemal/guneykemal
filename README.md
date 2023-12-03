- 👋 Hi, I’m @guneykemal
- 👀 I’m interested in ...
- 🌱 I’m currently learning ...
- 💞️ I’m looking to collaborate on ...
- 📫 How to reach me ...

<!---
guneykemal/guneykemal is a ✨ special ✨ repository because its `README.md` (this file) appears on your GitHub profile.
You can click the Preview link to take a look at your changes.
--->
	           //    calısma sorusu 4 
            sectıgı urune gore odeme yapma 
	///
	int secim;
	printf("**************************************\n");
	printf("************TERCIH  LISTESI*************\n");
	printf("*************************************\n");
	printf("1-Kirtasiye:\n");
	printf("2-Giyim\n");
	printf("3-Mobilya\n");
	printf("4-Beyaz esya\n");
	printf("*******************************\n\n\n");
	printf("lutfen tercih ettiginiz urunu seciniz\n");
	scanf_s("%d", &secim);


	int kirtasiye, giyim, mobilya, beyazesya, aladet;
	float ilkfiyat, sonfiyat, indirimfyt, adetindirimi;

	if (secim == 1)
		printf("lutfen kirtasiye harcama tutarinizi giriniz\n");
	scanf_s("%f", &ilkfiyat);


	if (ilkfiyat < 300) {

		if (ilkfiyat > 100) {
			printf("lutfen ayni urunden aldiysaniz,aldiginiz adedi giriniz");
			scanf_s("%d", &aladet);
			printf("uygulanacak indirim: %.2f\n", indirimfyt = ilkfiyat * 0.03);
			printf("indirim uygulandiktan sonraki fiyat :%.2f\n", sonfiyat = ilkfiyat - indirimfyt);
			printf("son fiyat : %2.f\n", sonfiyat + 50);
			if (aladet == 2)
				printf("ayni urunden kincisine uygulanan indirimin sonucu : %2.f\n", sonfiyat + ilkfiyat * 0.5);
			else {
				printf("lutfen secimlerinizin dogrulugunu kontrol ediniz ");
			}

		}





		if (secim == 2) {

			printf("lutfen giyim harcama tutarinizi giriniz\n");
			scanf_s("%f", &ilkfiyat);

			if (ilkfiyat < 300) {

				printf("uygulanacak indirim: %.2f\n", indirimfyt = ilkfiyat * 0.05);
				printf("kargo ucreti : %.2f\n", ilkfiyat * 0.02);
				printf("indirimin uygulanmis hali %.2f\n", sonfiyat = (ilkfiyat - indirimfyt) + ilkfiyat * 00.2);

			}
			else if (ilkfiyat > 300) {

				printf("lutfen aldiginiz urunun adedini  giriniz\n");
				scanf_s("%d", &aladet);
				printf("uygulanacak indirim: %.2f\n", indirimfyt = ilkfiyat * 0.06);
				printf("kargo ucreti : %.2f\n", ilkfiyat * 0.02);
				printf("indirimin uygulanmis hali : %f\n", sonfiyat = (ilkfiyat - indirimfyt) + ilkfiyat * 00.2);
				if (aladet == 10) {
					printf("ayni urunden 10 adet alindiginda uygulanan indirim : %.2f\n", adetindirimi = sonfiyat * 00.1);
					printf("ayni urunden 10 adet alindiginda odenecek fiyat : %.2f\n", sonfiyat = sonfiyat + (sonfiyat * 10 / 100));

				}
			}
			else
				printf("lutfen secimlerinizin dogrulugunu kontrol ediniz ");


		}
		else if (secim == 3)
		{
			printf("lutfen mobilya harcama tutarinizi giriniz\n");
			scanf_s("%f", &ilkfiyat);

			if (ilkfiyat < 500)
			{
				printf("uygulanacak indirim: %.2f\n", indirimfyt = ilkfiyat * 0.03);
				printf("kargo ucretiniz bulunmamaktadir\n");
				printf("indirim uygulanmis hali : %.2f\n", sonfiyat = ilkfiyat - indirimfyt);
			}
		}


		if (secim == 4)
		{
			printf("lutfen beyaz esya harcama tutarinizi giriniz\n");
			scanf_s("%f", &ilkfiyat);

			if (ilkfiyat < 1000) {
				printf("uygulanacak indirim : %.2f\n", indirimfyt = ilkfiyat * 10 / 100);
				printf("kargo ucretiniz bulunmamaktadir\n");
				printf("indirim uygulanmis hali : %2.f\n", sonfiyat = (ilkfiyat - indirimfyt) - 250);

			}
			else if (ilkfiyat > 1000)
			{
				printf("uygulanacak indirim : %.2f\n", indirimfyt = ilkfiyat * 0.1);
				printf("kargo ucretiniz bulunmamaktadir\n");
				printf("indirim uygulanmis hali : %2.f\n", sonfiyat = (ilkfiyat - indirimfyt) - 250);

			}
			else
				printf("lutfen secimlerinizin dogrulugunu kontrol ediniz ");
		}

	}
}   ///





///

girilen kordınatların bolgesını bulan c kodu

int x, y;

printf("lutfen x degerini giriniz \n");
scanf_s("%d", &x);
printf("lutfen y degerini giriniz\n");
scanf_s("%d", &y);

if (x > 0 && y > 0)
{
	printf("girmis oldugunuz kordinatlar 1. bolgede yer almaktadir\n");

}
else if (x < 0 && y > 0)
{
	printf("girmis oldugunuz kordinatlar 2. bolgede yer almaktadir\n");

}
else if (x < 0 && y < 0)
{
	printf("girmis oldugunuz kordinatlar 3. bolgede yer almaktadir\n");

}
else if (x > 0 && y < 0)
{
	printf("girmis oldugunuz kordinatlar 4. bolgede yer almaktadir\n");
}
else
printf("lutfen x ve y degerlerini dogru girdiginizden emin olun\n");

///



 ///
 
 
 disaridan girilen uc basamakli bir sayinin basamaklarini tek tek bastiran c codu



int sayi, toplam, kalan;


	printf("lutfen 3 basamakli bir sayi giriniz\n");
	scanf_s("%d", &sayi);

	printf("girmis oldugunuz sayinin yuzler basamagi  : %d\n", kalan = sayi / 100);

	printf("girmis oldugunuz sayinin onlar basamagi : %d\n", kalan = (sayi / 10) % 10 );


	printf("girmis oldugunuz sayinin birler basamagi %d\n", kalan = sayi % 10);

}


///



///

gırılen bır sayının asal olup olmadıgını kontrol eden c codu

#include <iostream>

int main();
{
	 sayi1 = 0, i = 2, asal = 0;



	printf("lutfen asalligini kontrol etmek istediginiz sayiyi giriniz\n");
	scanf("%d", &sayi1);

	if (sayi1 < 0)
	{
		printf("lutfen pozitif bir sayi giriniz\n");
	}

	for (i = 2;i < sayi1;i++)
	{
		if (sayi1 % i == 0)
		{
			asal = 1;
			break;
			//printf("%d  asal sayi degildir\n", sayi1);

		}
		if (asal == 0)
		{
			printf("%d asal sayidir\n", sayi1);
		}
		else
			printf("%d sayisi asal degildir\n", sayi1);

	}
	


	///

 
9) 50 ile 150 arasındaki tek sayıların toplamını bulan algoritmanın akış
diyagramını çiziniz. 50 ve 150 icin fixlemedım haberın olsun zıyaretcı


int sayi1, sayi2, toplamt = 0, sayacc,sayact, ortt, toplamc = 0,ortc;

printf("bakmak istediginiz  araligik icin ilk sayiyi giriniz\n");
scanf_s("%d", &sayi1);
printf("bakmak istediginiz  araligik icin ikinci sayiyi  giriniz\n");
scanf_s("%d", &sayi2);


for ( sayi1;sayi1 < sayi2;sayi1++)
{
	sayacc=0;
	sayact=0;
	if (sayi1 > sayi2)
	{
		printf("lutfen ilk sayiyi ikinci sayidan kucuk giriniz\n");
	}
	else if (sayi1 % 2 == 0)
	{
		sayacc = sayacc + 1;
		toplamc = toplamc + sayi1;
		ortc = toplamc / sayacc;
	}
	else if (sayi1 % 2 != 0)
	{
		sayact = sayact + 1;
		toplamt = toplamt + sayi1;
		ortt = toplamt / sayact;
	}
	else
	{
		printf("lutfen girmis oldugunuz sayi degerlerini kontrol ediniz\n");
	}
}
printf(" cift t : %d", toplamc);
printf("cift ort : %d", ortc);
printf("tek t : %d", toplamt);
printf("tek ort %d", ortt);

///



///

 
6) YBS 103 - Programlamaya Giriş dersinin değerlendirme oranları,
Nihai Not = Ara Sınav x 0.3 + Proje x 0.2 + Dönem Sonu Sınavı x 0.5
olarak belirlenmiştir.Buna göre bir öğrencinin elde edeceği nihai nota göre
alacağı harf notunun ne olduğunu hesaplayan algoritmanın akış diyagramını
çiziniz. (0 - 49 F1, 50 - 54 D1, 55 - 59 D2, 60 - 64 C2, 65 - 69 C1, 70 - 74 B3, 75 - 79 B2, 80 -
	84 B1, 85 - 89 A3, 90 - 94 A2, 94 - 100 A1)
	
	
	
int nihainot, arasinav, proje, dss, ort;

printf("lutfen ara sinav notunuzu giriniz\n");
scanf_s("%d", &arasinav);
printf("lutfen proje notunu giriniz \n");
scanf_s("%d", &proje);
printf("lutfen donem sonu sınav sonucunuzu giriniz\n");
scanf_s("%d", &dss);
printf("nihai notunuz : %d ", nihainot = arasinav * 0.3 + proje * 0.2 + dss * 0.5);
if (nihainot < 50)
{
	printf("harf notunuz F ");
}
else if (nihainot < 60)
{
	printf("harf notunuz D ");
}
else if (nihainot < 70)
{
	printf("harf notunuz C ");
}
else if (nihainot < 85)
{
	printf("harf notunuz B ");
}
else if (nihainot < 100)
{
	printf("harf notunuz A ");
}
else
{
	printf("lutfen notlarinizi basarili girdiginizden emin olun");
}

///



///


	4) Dışarıdan programa bir ürünün fiyatı ve ürünün kodu okutulacaktır.Buna göre,
	okutulan ürünün fiyatına, ürün koduna göre KDV oranı ekleyen ve son fiyatı
		hesaplayan algoritmanın akış diyagramını çiziniz.
		Not: Ürün kodu 1 ise KDV oranı % 18, ürün kodu 2 ise KDV oranı % 10, ürün kodu
		3 ise KDV oranı % 5 olacaktır.Diğer tüm durumlarda KDV oranı % 1 alınacaktır.


	int urun, kodu, sonfiyat;
	printf("lutfen urunun fiyatini giriniz\n");
	scanf_s("%d", &urun);
	printf("*****************************\n");
	printf("urun kodu = 1\n");
	printf("urun kodu = 2\n");
	printf("urun kodu = 3\n");
	printf("*****************************\n");
	scanf_s("%d\n", &kodu);

	if (kodu == 1)
	{
		printf("urunun fiyati : %d", sonfiyat = urun - (urun * 0.18));
	}
	else if (kodu == 2)
	{
		printf("urunun fiyati : %d", sonfiyat = urun - (urun * 0.1));
	}
	else if (kodu == 3)
	{
		printf("urunun fiyati : %d",sonfiyat = urun - ( urun * 0.05));
	}
	else
	{
		printf("urunun fiyati %d", sonfiyat = urun - (urun * 0.01));
	}

 ///



///

boy kılo indeksıne gore tanım yapan c codu

 float boy, yas, cinsiyet, idealerkek, idealkadın;
	printf("boyunuzu giriniz:");
	scanf_s("%f", &boy);
	printf("yasinizi giriniz");
	scanf_s("%f", &yas);
	printf("**************\n");
	printf("1-Kadin\n");
	printf("2-Erkek\n");
	printf("seciminizi yapiniz.\n");
	scanf_s("%f", &cinsiyet);

	if (cinsiyet == 1)
	{

		printf("ideal kadin : %f",idealkadın = (boy - 100 + yas / 10) * 0, 8);
		scanf_s("%f", &idealkadın);
	}
	else(cinsiyet== 2);
	{

		printf("ideal erkek :%f ",idealerkek = (boy - 100 + yas / 10) * 0, 9);
		scanf_s("%f", &idealerkek);
	}

}

///


///

girilen sayiların sayı adedıne bolen yanı ortalamasını alan c codu

	
	int sayi, sayac = 0, toplam = 0, ort;
	printf("lutfen bir sayi giriniz\n");
	scanf_s("%d\n", &sayi);
	while (1)

	{
		if (sayi == -1)
			break;
		else  if (sayi != -1) {
			printf("lutfen bir sayi giriniz\n");
			scanf_s("%d\n", &sayi);
			sayac++;
			toplam = toplam + sayi;
		}

	}

	printf("tebrikler girmis oldugunuz sayilarin ortalamasini  buldunuz : %d\n",ort = toplam / sayac);  */

///
                    
				
