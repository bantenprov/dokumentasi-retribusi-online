---
date: 2017-01-16
title: Perancangan database
categories:
  - Retribusi-Online
description: Perancangan database aplikasi Retribusi Online Pemerintah Provinsi Banten
type: Document
---

Seperti biasanya perangcangan aplikasi didahului oleh perancangan database, untuk melihat tabel - tabel yang diperlukan dan juga keterkaitan atau relasi antar tabel tabel tersebut.

## Perancangan Database

 [![Perancangan database sistem](/images/retribusi-online/perancangan-database/retibusi_online-perancangan-database-sistem.png)](/images/retribusi-online/perancangan-database/retibusi_online-perancangan-database-sistem.png)

## Tabel OPD

Adalah tabel yang menampung daftar Organisasi Perangkat Daerah yang ada di lingkungan Pemerintah provinsi Banten. Di dalam tabel ini terdapat beberapa field yang berhubungan dengan organisasi perangkat daerah. Berikut adalah field yang terdapat pada tabel daftar opd:

1. id: Merupakan **id** dari data opd.
2. timestamps: Merupakan tanggal di buatnya data.
3. softDeletes: Merupakan tanggal di hapusnya data. (Field ini akan terisi hanya jika data dihapus)

## Tabel Daftar Retribusi

Adalah tabel yang menampung daftar Retribusi Perangkat Daerah yang ada di lingkungan Pemerintah Provinsi Banten. Di dalam tabel ini terdapat beberapa field yang berhubungan dengan retribusi perangkat daerah. Berikut adalah field yang terdapat pada tabel daftar retribusi:

1. id: Merupakan **id** dari data retribusi.
2. uuid: Merupakan **id** dari data retribusi yang berjenis string dan unique.
3. nama: Merupakan data dari nama retribusi.
4. timestamps: Merupakan tanggal di buatnya data.
5. softDeletes: Merupakan tanggal di hapusnya data. (Field ini akan terisi hanya jika data dihapus)
6. opd_id: Merupakan **id** dari data OPD.
7. opd_uuid: Merupakan **id** dari data OPD yang berjenis string dan unique.
8. user_id: Merupakan **id** dari data user.
9. user_update: Merupakan data yang di update oleh user.

## Tabel Master Tarif

Adalah tabel yang menampung data master dari Tarif Retribusi Perangkat Daerah yang ada di lingkungan Pemerintah Provinsi Banten. Di dalam tabel ini terdapat beberapa field yang berhubungan dengan master data tarif retribusi perangkat daerah. Berikut adalah field yang terdapat pada tabel daftar master tarif:

1. id: Merupakan **id** dari data master tarif.
2. uuid: Merupakan **id** dari data master tarif yang berjenis string dan unique.
3. dasar_hukum: Merupakan data dasar hukum dari tarif retribusi.
4. status: Merupakan data status dari tarif retribusi.
5. timestamps: Merupakan tanggal di buatnya data.
6. softDeletes: Merupakan tanggal di hapusnya data. (Field ini akan terisi hanya jika data dihapus)
7. daftar_retribusi_id: Merupakan **id** dari data daftar retribusi.
8. daftar_retribusi_uuid: Merupakan **id** dari data daftar retribusi yang berjenis string dan unique.
9. user_id: Merupakan **id** dari data user.
10. user_update: Merupakan data yang di update oleh user.
 

## Tabel Tarif

Adalah tabel yang menampung daftar Tarif Retribusi Perangkat Daerah yang ada di lingkungan Pemerintah Provinsi Banten. Di dalam tabel ini terdapat beberapa field yang berhubungan dengan tarif retribusi perangkat daerah. Berikut adalah field yang terdapat pada tabel daftar tarif retribusi:

1. id: Merupakan **id** dari data tarif.
2. uuid: Merupakan **id** dari data tarif yang berjenis string dan unique.
3. uraian: Merupakan nama dari data uraian tarif.
4. jasa_pelayanan: Merupakan nama dari data tarif jasa pelayanan.
5. jasa_sarana: Merupakan nama dari data tarif jasa sarana.
6. satuan: Merupakan nama dari data tarif jasa satuan.
7. timestamps: Merupakan tanggal di buatnya data.
8. softDeletes: Merupakan tanggal di hapusnya data. (Field ini akan terisi hanya jika data dihapus)
9. master_tarif_id: Merupakan **id** dari data Master tarif.
10. user_id: Merupakan **id** dari data user.
11. user_update: Merupakan data yang di update oleh user.

## Tabel Transaksi

Adalah tabel yang menampung daftar Transaksi Retribusi Perangkat Daerah yang ada di lingkungan Pemerintah Provinsi Banten. Di dalam tabel ini terdapat beberapa field yang berhubungan dengan transaksi retribusi perangkat daerah. Berikut adalah field yang terdapat pada tabel daftar transaksi retribusi:

1. id: Merupakan **id** dari data transaksi.
2. uuid: Merupakan **id** dari data transaksi yang berjenis string dan unique.
3. nomor: Merupakan nama dari data nomor transaksi.
4. total: Merupakan nama dari data total transaksi.
5. grandtotal: Merupakan nama dari data total grand total transaksi.
6. denda: Merupakan nama dari data denda transaksi.
7. potongan: Merupakan nama dari data potongan transaksi.
8. timestamps: Merupakan tanggal di buatnya data.
9. softDeletes: Merupakan tanggal di hapusnya data. (Field ini akan terisi hanya jika data dihapus)
10. admin_id: Merupakan **id** dari data Admin.
11. customer_transaksi_id: Merupakan **id** dari data Transaksi Customer.
12. tarif_id: Merupakan **id** dari data Tarif.
13. admin_uuid: Merupakan **id** dari data admin yang berjenis string dan unique.
14. customer_transaksi_uuid: Merupakan **id** dari data transaksi customer yang berjenis string dan unique.
15. tarif_uuid: Merupakan **id** dari data tarif yang berjenis string dan unique.
 
## Tabel Item

Adalah tabel yang menampung daftar Item Retribusi Perangkat Daerah yang ada di lingkungan Pemerintah Provinsi Banten. Di dalam tabel ini terdapat beberapa field yang berhubungan dengan item retribusi perangkat daerah. Berikut adalah field yang terdapat pada tabel daftar item retribusi:

1. id: Merupakan **id** dari data item.
2. uuid: Merupakan **id** dari data item yang berjenis string dan unique.
3. keterangan: Merupakan nama dari data keterangan item.
4. tarif: Merupakan nama dari data tarif item.
5. jumlah: Merupakan nama dari data jumlah item.
6. subtotal: Merupakan nama dari data subtotal item.
7. timestamps: Merupakan tanggal di buatnya data.
8. softDeletes: Merupakan tanggal di hapusnya data. (Field ini akan terisi hanya jika data dihapus)
9. transaksi_id: Merupakan **id** dari data transaksi.
10. tarif_id: Merupakan **id** dari data tarif.
11. rekening_id: Merupakan **id** dari data rekening.
12. transaksi_uuid: Merupakan **id** dari data transaksi yang berjenis string dan unique.
13. tarif_uuid: Merupakan **id** dari data tarif yang berjenis string dan unique. 
14. rekening_uuid: Merupakan **id** dari data rekening yang berjenis string dan unique.

## Tabel Nomor Rekening

Adalah tabel yang menampung daftar Rekening Retribusi Perangkat Daerah yang ada di lingkungan Pemerintah Provinsi Banten. Di dalam tabel ini terdapat beberapa field yang berhubungan dengan rekening retribusi perangkat daerah. Berikut adalah field yang terdapat pada tabel daftar rekening retribusi:

1. id: Merupakan **id** dari data rekening.
2. uuid: Merupakan **id** dari data rekening yang berjenis string dan unique.
3. kode: Merupakan nama dari data kode rekening.
4. nama: Merupakan nama dari data nama rekening.
5. timestamps: Merupakan tanggal di buatnya data.
6. softDeletes: Merupakan tanggal di hapusnya data. (Field ini akan terisi hanya jika data dihapus)
7. user_id: Merupakan **id** dari data user.
8. user_update: Merupakan data yang di update oleh user.

## Tabel Customer

Adalah tabel yang menampung daftar Customer Retribusi Perangkat Daerah yang ada di lingkungan Pemerintah Provinsi Banten. Di dalam tabel ini terdapat beberapa field yang berhubungan dengan customer retribusi perangkat daerah. Berikut adalah field yang terdapat pada tabel daftar customer retribusi:

1. id: Merupakan **id** dari data customer.
2. uuid: Merupakan **id** dari data customer yang berjenis string dan unique.
3. nama: Merupakan nama dari data nama customer.
4. timestamps: Merupakan tanggal di buatnya data.
5. softDeletes: Merupakan tanggal di hapusnya data. (Field ini akan terisi hanya jika data dihapus)
6. user_id: Merupakan **id** dari data user.
 

## Tabel Retribusi Customer

Adalah tabel yang menampung daftar Retribusi Customer Perangkat Daerah yang ada di lingkungan Pemerintah Provinsi Banten. Di dalam tabel ini terdapat beberapa field yang berhubungan dengan customer retribusi perangkat daerah. Berikut adalah field yang terdapat pada tabel daftar customer retribusi:

1. id: Merupakan **id** dari data retribusi customer.
2. uuid: Merupakan **id** dari data customer yang berjenis string dan unique.
3. timestamps: Merupakan tanggal di buatnya data.
4. softDeletes: Merupakan tanggal di hapusnya data. (Field ini akan terisi hanya jika data dihapus)
5. customers_id: Merupakan **id** dari data customer.
6. daftar_retribusi_id: Merupakan **id** dari data retribusi.
7. user_id: Merupakan **id** dari data user.
8. user_update: Merupakan data yang di update oleh user.

## Tabel Admin

Adalah tabel yang menampung daftar Admin Retribusi Perangkat Daerah yang ada di lingkungan Pemerintah Provinsi Banten. Di dalam tabel ini terdapat beberapa field yang berhubungan dengan admin retribusi perangkat daerah. Berikut adalah field yang terdapat pada tabel daftar admin retribusi:

1. id: Merupakan **id** dari data admin.
2. uuid: Merupakan **id** dari data admin yang berjenis string dan unique.
3. timestamps: Merupakan tanggal di buatnya data.
4. softDeletes: Merupakan tanggal di hapusnya data. (Field ini akan terisi hanya jika data dihapus)
5. user_id: Merupakan **id** dari data user.
6. opd_id: Merupakan **id** dari data opd.

## Tabel User

Adalah tabel yang menampung daftar User Retribusi Perangkat Daerah yang ada di lingkungan Pemerintah provinsi Banten. Di dalam tabel ini terdapat beberapa field yang berhubungan dengan user retribusi perangkat daerah. Berikut adalah field yang terdapat pada tabel daftar user:

1. id: Merupakan **id** dari data user.
2. timestamps: Merupakan tanggal di buatnya data.
3. softDeletes: Merupakan tanggal di hapusnya data. (Field ini akan terisi hanya jika data dihapus)




