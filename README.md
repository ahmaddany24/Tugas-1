1.
<img width="742" height="638" alt="image" src="https://github.com/user-attachments/assets/e6dbb4e4-29e2-43f1-9db2-3f14ed9f59db" />

<img width="749" height="526" alt="image" src="https://github.com/user-attachments/assets/6634dee7-af89-4c47-b1a0-77e49a7a3234" />

<img width="761" height="655" alt="image" src="https://github.com/user-attachments/assets/ad0d887c-e394-4718-9e86-a528a80d84b1" />





2.	Analisislah pada gambar kenapa saat instalasi perlu dipilih “/” pada opsi Mount Point ?

Mount point / atau root directory merupakan direktori utama dalam struktur filesystem
Linux. Hampir seluruh direktori dan file sistem Linux berada di bawah struktur root /.
Pada proses instalasi, partisi yang diberi mount point / digunakan sebagai lokasi utama filesystem sistem operasi. Dengan adanya mount point tersebut, sistem mengetahui bahwa partisi tersebut merupakan tempat utama untuk memasang dan menjalankan sistem Linux.
Struktur direktori seperti /bin, /etc, /usr, /var, /boot, dan direktori sistem lainnya berada di bawah root /. Oleh karena itu, instalasi Linux membutuhkan filesystem yang memiliki mount point /.
Dalam praktikum, opsi Something else digunakan agar partisi dapat diatur secara manual, kemudian salah satu partisi diberikan mount point / menggunakan filesystem Ext4. Modul juga menjelaskan bahwa opsi tersebut digunakan untuk mengelola partisi harddisk sebagai tempat filesystem dan penyimpanan data.
 
mount point / diperlukan karena merupakan titik utama/root dari filesystem Linux dan menjadi lokasi utama sistem operasi Linux diinstal serta menjalankan berbagai direktori system.


3.	Berikan penjelasan tentang ext4, ext3, swap, ntfs, fat32,btrfs !

a.	Ext4
Ext4 (Fourth Extended Filesystem) merupakan filesystem yang banyak digunakan pada sistem operasi Linux. Ext4 merupakan pengembangan dari Ext3 dan menyediakan kemampuan pengelolaan file serta penyimpanan yang lebih baik.
Pada praktikum, Ext4 digunakan untuk partisi Linux seperti /home dan /. Modul secara khusus menggunakan Ext4 Journaling File System untuk partisi tersebut.

b.	Ext3
Ext3 (Third Extended Filesystem) merupakan filesystem Linux yang merupakan pengembangan dari Ext2. Salah satu karakteristik penting Ext3 adalah penggunaan journaling, yaitu pencatatan perubahan filesystem untuk membantu menjaga konsistensi filesystem ketika terjadi gangguan seperti mati listrik atau sistem berhenti secara tiba-tiba.

c.	Swap
Swap merupakan ruang pada media penyimpanan yang digunakan Linux sebagai memori virtual. Swap dapat membantu ketika kebutuhan memori melebihi kapasitas RAM yang tersedia.
Dalam praktikum, swap dibuat sebagai partisi tersendiri dengan memilih Use As: Swap Area. Contoh ukuran yang diberikan dalam modul adalah 1024 MB.

d.	NTFS
NTFS (New Technology File System) merupakan filesystem yang dikembangkan dan banyak digunakan oleh sistem operasi Windows. NTFS mendukung ukuran file dan partisi yang
besar serta menyediakan berbagai fitur seperti permission dan journaling.
NTFS umumnya digunakan untuk partisi Windows dan penyimpanan yang membutuhkan kompatibilitas dengan Windows.
 
e.	FAT32
FAT32 (File Allocation Table 32) merupakan filesystem yang memiliki kompatibilitas luas dengan berbagai sistem operasi dan perangkat. FAT32 sering digunakan pada flashdisk, kartu memori, dan media penyimpanan lain.
Keterbatasan penting FAT32 adalah ukuran maksimum sebuah file sekitar 4 GB, sehingga kurang sesuai untuk menyimpan file individual yang berukuran sangat besar.

f.	Btrfs
Btrfs (B-tree File System) merupakan filesystem Linux modern yang dirancang untuk
mendukung fitur-fitur seperti snapshot, subvolume, checksum, dan pengelolaan storage yang lebih fleksibel.
Btrfs dapat digunakan pada sistem Linux ketika dibutuhkan fitur manajemen filesystem yang lebih modern.
