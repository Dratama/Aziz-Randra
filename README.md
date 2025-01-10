import sys
import time


def jalanin_lirik():
    # Ubah lirik lagu dan delay hurufnya sesuai yang kalian mau
    lirik = [
        ("I hold imagination cover all of the sadness", 0.1),
        ("I don't feel something special, turn off the phone to get some spatial", 0.09),
        ("Never thought i'd living in true", 0.09),
        ("The truth that has been so blue", 0.09),
        ("It was in a blink of an eye", 0.09),
        ("Find a way how to say goodbye", 0.09),
        ("I've got to take me away from all sadness", 0.09),
    ]

    # Ubah delay dari setiap baris lagu (sesuaikan jumlah)
    delay = [0.3, 0.2, 0.3, 0.4, 0.6, 0.3, 0.3]
    # Ubah judul lagu
    print("\n== Somebody Pleasure_Aziz Rendra ==")
    for i, (baris_lagu, delay_karakter) in enumerate(lirik):
        for karakter in baris_lagu:
            print(karakter, end='')
            sys.stdout.flush()
            time.sleep(delay_karakter)
        time.sleep(delay[i])
        print('')
    # Ganti nama pembuat
    print("// Code by Andra Pratama")


jalanin_lirik()
