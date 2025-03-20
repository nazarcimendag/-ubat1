# 1
def hesap_makinesi(sayi1, sayi2):
    toplam = sayi1 + sayi2
    fark = sayi1 - sayi2
    carpim = sayi1 * sayi2
    if sayi2 != 0:
        bolum = sayi1 / sayi2
    else:
        bolum = "Sıfıra bölme hatası"
    
    return toplam, fark, carpim, bolum
sayi1 = float(input("Birinci sayıyı girin: "))
sayi2 = float(input("İkinci sayıyı girin: "))

toplam, fark, carpim, bolum = hesap_makinesi(sayi1, sayi2)

print(f"Toplam: {toplam}")
print(f"Fark: {fark}")
print(f"Çarpım: {carpim}")
print(f"Bölüm: {bolum}")

# 2
def palindrom_mu(kelime):
    if kelime == kelime[::-1]:
        return True
    else:
        return False

kelime = input("Bir kelime girin: ")

if palindrom_mu(kelime):
    print(f"{kelime} -> Palindrom")
else:
    print(f"{kelime} -> Değil")


# 3
def kac_yil_sonra_100_yasinda(yas):
    if yas >= 100:
        return 0
    else:
        return 100 - yas

yas = int(input("Yaşınızı girin: "))

yil_sonra = kac_yil_sonra_100_yasinda(yas)

print(f"{yil_sonra} yıl sonra 100 yaşında olacaksınız.")

