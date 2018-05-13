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
2. timestamps: Merupakan tanggal di buatnya data.
3. softDeletes: Merupakan tanggal di hapusnya data. (Field ini akan terisi hanya jika data dihapus)
4. opd_id: Merupakan **id** dari data OPD.
5. nama: Merupakan nama dari data retribusi.

## Tabel Master Tarif

Adalah tabel yang menampung data master dari Tarif Retribusi Perangkat Daerah yang ada di lingkungan Pemerintah Provinsi Banten. Di dalam tabel ini terdapat beberapa field yang berhubungan dengan master data tarif retribusi perangkat daerah. Berikut adalah field yang terdapat pada tabel daftar master tarif:

1. id: Merupakan **id** dari data master tarif.
2. timestamps: Merupakan tanggal di buatnya data.
3. softDeletes: Merupakan tanggal di hapusnya data. (Field ini akan terisi hanya jika data dihapus)
4. dasar_hukum: Merupakan data dasar hukum dari tarif retribusi.
5. status: Merupakan data status dari tarif retribusi.

## Tabel Tarif

Adalah tabel yang menampung daftar Tarif Retribusi Perangkat Daerah yang ada di lingkungan Pemerintah Provinsi Banten. Di dalam tabel ini terdapat beberapa field yang berhubungan dengan tarif retribusi perangkat daerah. Berikut adalah field yang terdapat pada tabel daftar tarif retribusi:

1. id: Merupakan **id** dari data tarif.
2. timestamps: Merupakan tanggal di buatnya data.
3. softDeletes: Merupakan tanggal di hapusnya data. (Field ini akan terisi hanya jika data dihapus)
4. master_tarif_id: Merupakan **id** dari data Master tarif.
5. jasa_pelayanan: Merupakan nama dari data tarif jasa pelayanan.
6. jasa_sarana: Merupakan nama dari data tarif jasa sarana.
7. satuan: Merupakan nama dari data tarif jasa satuan.

## Tabel Transaksi

Adalah tabel yang menampung daftar Transaksi Retribusi Perangkat Daerah yang ada di lingkungan Pemerintah Provinsi Banten. Di dalam tabel ini terdapat beberapa field yang berhubungan dengan transaksi retribusi perangkat daerah. Berikut adalah field yang terdapat pada tabel daftar transaksi retribusi:

1. id: Merupakan **id** dari data transaksi.
2. timestamps: Merupakan tanggal di buatnya data.
3. softDeletes: Merupakan tanggal di hapusnya data. (Field ini akan terisi hanya jika data dihapus)
4. tarif_id: Merupakan **id** dari data Tarif.
5. customer_id: Merupakan **id** dari data Customer.
6. nomor: Merupakan nama dari data nomor transaksi.
7. admin_id: Merupakan **id** dari data Admin.
8. total: Merupakan nama dari data total transaksi.
9. denda: Merupakan nama dari data denda transaksi.
10. potongan: Merupakan nama dari data potongan transaksi.
11. grandtotal: Merupakan nama dari data total grand total transaksi.

## Tabel Item

Adalah tabel yang menampung daftar Item Retribusi Perangkat Daerah yang ada di lingkungan Pemerintah Provinsi Banten. Di dalam tabel ini terdapat beberapa field yang berhubungan dengan item retribusi perangkat daerah. Berikut adalah field yang terdapat pada tabel daftar item retribusi:

1. id: Merupakan **id** dari data item.
2. timestamps: Merupakan tanggal di buatnya data.
3. softDeletes: Merupakan tanggal di hapusnya data. (Field ini akan terisi hanya jika data dihapus)
4. transaksi_id: Merupakan **id** dari data Transaksi.
5. rekening_id: Merupakan **id** dari data Rekening.
6. keterangan: Merupakan nama dari data keterangan item.
7. tarif_id: Merupakan **id** dari data Tarif.
8. tarif: Merupakan nama dari data tarif item.
9. jumlah: Merupakan nama dari data jumlah item.
10. subtotal: Merupakan nama dari data subtotal item.

## Tabel Nomor Rekening

Adalah tabel yang menampung daftar Rekening Retribusi Perangkat Daerah yang ada di lingkungan Pemerintah Provinsi Banten. Di dalam tabel ini terdapat beberapa field yang berhubungan dengan rekening retribusi perangkat daerah. Berikut adalah field yang terdapat pada tabel daftar rekening retribusi:

1. id: Merupakan **id** dari data rekening.
2. timestamps: Merupakan tanggal di buatnya data.
3. softDeletes: Merupakan tanggal di hapusnya data. (Field ini akan terisi hanya jika data dihapus)
4. kode: Merupakan nama dari data kode Rekening.
5. nama: Merupakan nama dari data nama Rekening.

## Tabel Customer

Adalah tabel yang menampung daftar Customer Retribusi Perangkat Daerah yang ada di lingkungan Pemerintah Provinsi Banten. Di dalam tabel ini terdapat beberapa field yang berhubungan dengan customer retribusi perangkat daerah. Berikut adalah field yang terdapat pada tabel daftar customer retribusi:

1. id: Merupakan **id** dari data customer.
2. timestamps: Merupakan tanggal di buatnya data.
3. softDeletes: Merupakan tanggal di hapusnya data. (Field ini akan terisi hanya jika data dihapus)
4. user_id: Merupakan **id** dari data user.
5. nama: Merupakan nama dari data nama Customer.

## Tabel Admin

Adalah tabel yang menampung daftar Admin Retribusi Perangkat Daerah yang ada di lingkungan Pemerintah Provinsi Banten. Di dalam tabel ini terdapat beberapa field yang berhubungan dengan admin retribusi perangkat daerah. Berikut adalah field yang terdapat pada tabel daftar admin retribusi:

1. id: Merupakan **id** dari data admin.
2. timestamps: Merupakan tanggal di buatnya data.
3. softDeletes: Merupakan tanggal di hapusnya data. (Field ini akan terisi hanya jika data dihapus)
4. user_id: Merupakan **id** dari data user.
5. opd_id: Merupakan **id** dari data opd.

## Tabel User

Adalah tabel yang menampung daftar User Retribusi Perangkat Daerah yang ada di lingkungan Pemerintah provinsi Banten. Di dalam tabel ini terdapat beberapa field yang berhubungan dengan user retribusi perangkat daerah. Berikut adalah field yang terdapat pada tabel daftar user:

1. id: Merupakan **id** dari data user.
2. timestamps: Merupakan tanggal di buatnya data.
3. softDeletes: Merupakan tanggal di hapusnya data. (Field ini akan terisi hanya jika data dihapus)




