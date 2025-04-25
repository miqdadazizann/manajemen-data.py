#AHMAD RIFAI
#AZRIL KHAYRU NAJA
#CHIKA ANDHARU WIDIYANTO
#MIQDAD AZIZAN NASAHA


data_siswa = []


def tampilkan_menu():
    print("\n=== Menu Manajemen Siswa ===")
    print("1. Tambah Siswa")
    print("2. Lihat Siswa")
    print("3. Edit Siswa")
    print("4. Hapus Siswa")
    print("5. Keluar")


def tambah_siswa():
    nama = input("Masukkan Nama: ")
    usia = input("Masukkan Usia: ")
    nilai = input("Masukkan Nilai Rata-rata: ")
    siswa = {"nama": nama, "usia": usia, "nilai": nilai}
    data_siswa.append(siswa)
    print(f"[Siswa {nama} berhasil ditambahkan!]")


def lihat_siswa():
    if len(data_siswa) == 0:
        print("\nBelum ada data siswa yang dimasukkan.")
    else:
        print("\n=== Daftar Siswa ===")
        for i, siswa in enumerate(data_siswa):
            print(f"{i+1}. Nama: {siswa['nama']}, Usia: {siswa['usia']}, Nilai: {siswa['nilai']}")



def edit_siswa():
    lihat_siswa()
    try:
        index = int(input("Masukkan nomor siswa yang ingin diedit: ")) - 1
        if 0 <= index < len(data_siswa):
            nama = input("Masukkan Nama baru: ")
            usia = input("Masukkan Usia baru: ")
            nilai = input("Masukkan Nilai Rata-rata baru: ")
            data_siswa[index] = {"nama": nama, "usia": usia, "nilai": nilai}
            print("Data siswa berhasil diperbarui.")
        else:
            print("Nomor siswa tidak valid.")
    except ValueError:
        print("Input tidak valid.")


def hapus_siswa():
    lihat_siswa()
    try:
        index = int(input("Masukkan nomor siswa yang ingin dihapus: ")) - 1
        if 0 <= index < len(data_siswa):
            siswa = data_siswa.pop(index)
            print(f"Siswa {siswa['nama']} berhasil dihapus.")
        else:
            print("Nomor siswa tidak valid.")
    except ValueError:
        print("Input tidak valid.")


while True:
    tampilkan_menu()
    pilihan = input("Pilih menu: ")

    if pilihan == '1':
        tambah_siswa()
    elif pilihan == '2':
        lihat_siswa()
    elif pilihan == '3':
        edit_siswa()
    elif pilihan == '4':
        hapus_siswa()
    elif pilihan == '5':
        print("Terima kasih telah menggunakan program ini.")
        break
    else:
        print("Pilihan tidak valid, silakan coba lagi.")
