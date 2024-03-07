

import random

def sabit_oyun():
    print("Sabit Oyununa Hoş Geldiniz!")
    print("1 ile 100 arasında bir sayıyı tahmin edin.")
    
    # Rasgele bir sayı seç
    sabit_sayi = random.randint(1, 100)
    tahmin_sayisi = 0
    
    while True:
        tahmin = int(input("Tahmininizi girin: "))
        tahmin_sayisi += 1
        
        if tahmin < sabit_sayi:
            print("Daha büyük bir sayı girin.")
        elif tahmin > sabit_sayi:
            print("Daha küçük bir sayı girin.")
        else:
            print(f"Tebrikler! {sabit_sayi} sayısını {tahmin_sayisi} tahminde buldunuz.")
            break
