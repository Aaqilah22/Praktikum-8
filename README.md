# PERTEMUAN 11

# Soal

![Screenshot 2024-11-29 130143](https://github.com/user-attachments/assets/b2a572b9-928a-4d3d-9a24-878ea9859596)

## Customer

![Customer](https://github.com/user-attachments/assets/3fab7d58-7ac0-4eab-8bc7-d1410106b2a5)

Penjelasan :
- Atribut:
  - name: Nama customer.
  - address: Alamat customer.
- Konstruktor: Menginisialisasi name dan address.
- Getter: Memberikan akses ke nama dan alamat customer.

## Order

![Order](https://github.com/user-attachments/assets/f333dfc5-da70-4eea-8ef9-7497bdd690a8)

Penjelasan : 
- Atribut:
  - date: Tanggal pesanan.
  - status: Status pesanan (misalnya: "Processed").
  - orderDetails: List yang berisi objek OrderDetail.
- Metode:
  - calcSubTotal(): Menghitung total semua subtotal dari setiap barang.
  - calcTax(): Menghitung total pajak dari semua barang.
  - calcTotal(): Menghitung total keseluruhan (subtotal + pajak).
  - calcTotalWeight(): Menghitung total berat semua barang.
## OrderDetail

![OrderDetail](https://github.com/user-attachments/assets/c151f0e0-28ee-43d7-a2db-42e2270228d6)

penjelasan :
- Atribut:
  - quantity: Jumlah barang dalam pesanan.
  - taxStatus: Status pajak barang.
  - item: Objek dari kelas Item.
- Metode:
  - calcSubTotal(): Menghitung subtotal dengan mengalikan harga barang dengan jumlah.
  - calcTax(): Menghitung pajak dari subtotal.
  - calcWeight(): Menghitung total berat barang yang dipesan.

## Item

![Item](https://github.com/user-attachments/assets/89ba5c87-77f4-4ae7-bfbb-6690a1dbf56e)

Penjelasan :
- Atribut:
  - shippingWeight: Berat barang yang akan dikirim.
  - description: Deskripsi barang.
- Metode:
  - getPriceForQuantity(): Mengembalikan harga barang per unit (contoh: 1000).
  - inStock(): Mengembalikan status stok (asumsi selalu tersedia).
    
## Payment (abstrac)

![Payment](https://github.com/user-attachments/assets/71e76f26-f085-4faf-833f-a87a9ace3295)

penjelasan : 
- Atribut:
  - amount: Jumlah pembayaran.
- Metode abstrak:
  - authorized(): Harus diimplementasikan oleh kelas turunan (misalnya Cash, Check, atau Credit).
    
## Cash

![cash](https://github.com/user-attachments/assets/f2a9f21f-58ec-42a0-bb5b-9d120464e144)

Penjelasan :
- Atribut:
cashTendered: Jumlah uang tunai yang diterima.
- Metode:
authorized(): Mengecek apakah uang tunai cukup.
## Check

![Check](https://github.com/user-attachments/assets/a80f6e41-af2f-469e-94fd-91b6a15205b6)

Penjelasan : 
- Atribut:
  - name: Nama pada cek.
  - bankID: ID bank.
- Metode:
authorized(): Mengecek validitas ID bank.
## Credit

![Credit](https://github.com/user-attachments/assets/104fc0cf-4253-45e5-afdc-4ddf0968a5c1)

Penjelasan :
- Atribut:
  - number: Nomor kartu kredit.
  - type: Jenis kartu (Visa, MasterCard, dll.).
  - expDate: Tanggal kedaluwarsa.
- Metode:
authorized(): Mengecek apakah nomor kartu memiliki panjang 16 digit.
## Main

![Main1](https://github.com/user-attachments/assets/0d81b177-e54b-4052-9eba-a63847a5f1be)

![Main2](https://github.com/user-attachments/assets/08a4c354-90be-4394-b2b7-cb3013ebfbcb)

## Output

![OutPut8](https://github.com/user-attachments/assets/0ab7e668-2adc-4eda-8880-72b9fb4709b2)

# Selesai
