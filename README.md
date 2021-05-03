# Elevator_exemple_Omron_PLC
Sysmac programında geliştirmiş olduğum 3 katlı asansör uygulamasının kodları içerir. Dizi mantığı ile asansörün gideceği yeri hafızasında saklamaktadır.

## Kat algılama

Bu uygulamayı reelde yapmayıp simülasyon ortamında yaptığım için kat1, kat2, kat3 algılatmasını manuel yapılacak şekilde ayarladım.

![enter image description here](https://github.com/hrngcmn/Elevator_exemple_Omron_PLC/blob/main/Screenshot_6.png?raw=true)

## Asansör çağırma ve hafızaya aldırma işlemi yapılması
![enter image description here](https://github.com/hrngcmn/Elevator_exemple_Omron_PLC/blob/main/hafizaya_alma_ss.png?raw=true)
![enter image description here](https://github.com/hrngcmn/Elevator_exemple_Omron_PLC/blob/main/hafizaya_alma_Devam.png?raw=true)

Bu işlemin yapılması için dizi oluşturulması gerekmektedir. Çalışma mantığını şöyle açıklayım;
Buton2 ye basıldı dizi[0] da buton 2 ye basıldığının bilgisi var.
Sonrasında buton3e basıldı dizi[1] e 3 e gitmesi için bilgi atandı. 
Sonrasında buton1e basıldı dizi[2] ye 1 e gitmesi için bilgi atandı.

## Yukarı hareket şartları
![enter image description here](https://github.com/hrngcmn/Elevator_exemple_Omron_PLC/blob/main/ileri_gitme_%C5%9Fartlari.png?raw=true)

## Aşağı hareket şartları
![enter image description here](https://github.com/hrngcmn/Elevator_exemple_Omron_PLC/blob/main/geri_gitme_%C5%9Fartlar%C4%B1.png?raw=true)

## Motor ileri - geri 
![enter image description here](https://github.com/hrngcmn/Elevator_exemple_Omron_PLC/blob/main/ileri_geri.png?raw=true)

Kapı motorları çalışıyorken asansörün ileri geri hareketi yapılmayacaktır 

## Kata gittikten sonra hafızadaki işleme geçişi

![enter image description here](https://github.com/hrngcmn/Elevator_exemple_Omron_PLC/blob/main/hafizadaki_islemi_alma.png?raw=true)
Dizide kaydırma yapılmaktadır.

## Kapı - Açma - Kapama
![enter image description here](https://github.com/hrngcmn/Elevator_exemple_Omron_PLC/blob/main/g%C3%B6rev_Atama.png?raw=true)
