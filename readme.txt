link flowchart matriks :
https://drive.google.com/file/d/1TldQMEbhimgDOMgQL8hXAgBm9d-e_0uH/view?usp=sharing

START
Pseudocode matriks :
# Inisialisasi matriks a dan b
a = [[4, 1, 3], 
     [2, 5, 3], 
     [3, 7, 4]]

b = [[1, 2, 5], 
     [4, 3, 2], 
     [6, 2, 4]]

# Deklarasi matriks kosong untuk hasil
c = []

# Hitung jumlah baris dan kolom dari matriks a dan b
baris_a = len(a)
kolom_a = len(a[0])

baris_b = len(b)
kolom_b = len(b[0])

# Cetak informasi matriks a dan b
print("Baris matriks a adalah:", baris_a)
print("Kolom matriks a adalah:", kolom_a)
print()
print("Baris matriks b adalah:", baris_b)
print("Kolom matriks b adalah:", kolom_b)

# Kondisi pengecekan apakah matriks bisa dikalikan
if kolom_a == baris_b:
    print("Matriks a dan b dapat dikalikan.")
    
    # Inisialisasi matriks hasil perkalian dengan elemen nol
    c = [[0 for _ in range(kolom_b)] for _ in range(baris_a)]
    
    # Proses perkalian matriks
    for i in range(baris_a):
        for j in range(kolom_b):
            for k in range(kolom_a):
                c[i][j] += a[i][k] * b[k][j]
    
    # Cetak hasil matriks
    print("Hasil perkalian matriks a dan b adalah:")
    for row in c:
        print(row)
else:
    print("Matriks a dan b tidak dapat dikalikan.")
END

  * Bilangan yang terdapat dalam kolom matriks
  pada command inisiasi di atas hanya contoh dari bilangan matriks yang saya buat.
  Dapat kalian sesuakan dengan bilangan matriks yang kalian kerjakan.
