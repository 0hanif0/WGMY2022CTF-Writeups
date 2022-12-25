## OSINT
Chal Name: When am I

![image](https://user-images.githubusercontent.com/23289982/209468393-cff87ba5-cbe4-4997-a108-b3a7ffddf1cf.png)

## HINT
There is something in the picture, that helps you to verify your password. Ever played Hangman?

## SOLUTION
* download dan extract file diberi

![whenami](https://user-images.githubusercontent.com/23289982/209468454-c52f0534-5dc6-4178-8020-0a5b9d8b52b1.jpg)

* pada mulanya aku tak tahu nak mula dari mana sebab gambar tersebut menunjukkan aktiviti untuk comic fiesta
* seterunya aku upload gambar guna web [aperi solve](https://www.aperisolve.com)

![image](https://user-images.githubusercontent.com/23289982/209468585-73046c6f-bcb3-4d6c-a587-1b15cbe9e815.png)

* aku jumpa hint yang aku tak sangka boleh dapat iaitu password `OUROKRONII`
* aku yakin bahawa gambar tersebut mempunyai `steghide` yang guna password
* aku menggunakan [Steganographic Decoder](https://futureboy.us/stegano/decinput.html) beserta password `OUROKRONII` untuk melihat hidden information
* aku menjumpai hint seterusnya

![image](https://user-images.githubusercontent.com/23289982/209468760-a9f750bf-6f68-41b8-a1bf-cf661db698d4.png)

* akan tetapi hint tersebut tidak habis disitu, terdapat cipher yang perlu decode untuk mendapat flag
* aku yakin bahawa cipher tersebut adalah `book cipher` disebabkan format cipher tersebut berbentuk `1:2:3`
* ini youtube [book cipher](https://www.youtube.com/watch?v=xnAr4rEPxNo) untuk mengetahui lebih lanjut
* seterusnya bagaimana untuk decode `book cipher` sekiranya tiada text atau ayat untuk dijadikan rujukan
* hint seterusnya ialah `Among Us - 1:36:18` ini aku tidak pasti pada mulanya
* hint `[Viewer Rules]` membawa maksud rules untuk viewer sebagai contoh livestreaming
* seterusnya aku mencari video streaming di youtube bertajuk `among us` dan berdurasi `1:36:18` dan jumpa video tersebut

![image](https://user-images.githubusercontent.com/23289982/209469172-9501a35e-2813-4d3f-b8be-514df84e79da.png)

* [youtube among us](https://www.youtube.com/watch?v=hdwCWIAR3q4&t=1s)
* di bahagian description terdapat viewer rules yang mungkin boleh dijadikan rujukan untuk book cipher

![image](https://user-images.githubusercontent.com/23289982/209469305-df0625e0-2ac7-4be4-9941-492585a0c0a7.png)

* seterusnya kita mulakan decode
* cipher `1:2:3` 1 - number of lines(merah), 2 - number of words(hijau), 3 - number of characters(biru) 

![image](https://user-images.githubusercontent.com/23289982/209469965-c03e8fdb-4860-4bc1-9fa0-ca87d455e5e6.png)

* ini kaedah aku decode secara manual, terpulang kepada korang untuk decode ada cara online,script, dan sebagainya

![image](https://user-images.githubusercontent.com/23289982/209470196-b3c40cc4-653e-485d-ac94-43c4b15dd76a.png)

flag `wgmy{eeb7ac660269f45046a0e8abaa51dfec}`
