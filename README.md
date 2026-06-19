# imerswastorefinalpikselkasirantihacker
kita terapkan "ZERO TRUST ARCHITECTURE". Artinya, Backend Code.gs sekarang Haram Hukumnya percaya sama role yang dikirim frontend.

Konsep Keamanannya:

Saat user Login, backend akan mengembalikan Token Kripto (Hash Password) ke Frontend.

Setiap kali ada request ke Backend (bikin akun, edit akun, hapus, atur paket harga), Frontend WAJIB menyertakan requestor_id dan requestor_token.

Backend akan membongkar tabel Users untuk mencocokkan ID dan Token tersebut. Kalau cocok, Backend mengambil Real Role langsung dari Database (bukan dari inputan hacker).

Backend mengunci akses mati-matian: User biasa yang maksa bikin akun Admin lewat API bakal langsung kena blokir: "SECURITY ALERT!" 🚨
