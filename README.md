import time

def geri_sayim(saniye):
    while saniye:
        print(f"Qalan vaxt: {saniye} saniyə", end="\r")
        time.sleep(1)
        saniye -= 1
    print("Zaman bitdi!")

saniye = int(input("Geri sayım üçün saniyəni daxil edin: "))
geri_sayim(saniye)
