class Mahasiswa:#kelas mahasiswa
    def __init__(self, nama, npm, jurusan):# memiliki parameter nama dan jurusan  
        self.nama = nama #string atribut nama
        self.npm = npm  #string atribut npm
        self.jurusan = jurusan #Jurusan (objek dari kelas Jurusan)
    
    def tampilkan_info(self): #method untuk menampilkan informasi
        print("Nama    :", self.nama) # method akan mencetak nama yang di inputkan
        print("NPM     :", self.npm) # akan mencetak npm 

class Jurusan: #kelas jurusan
    def __init__(self, nama_jurusan): #memiliki parameter nama_jurusan
        self.nama_jurusan = nama_jurusan #inisialisasi atribut nama_jurusan pada objek Jurusan dengan nilai dari parameter nama_jurusan
        self.daftar_mahasiswa = []  # merupakan daftar kosong yang digunakan untuk menyimpan daftar mahasiswa 
    
    def tambah_mahasiswa(self, mahasiswa): # metode yang digunakan untuk menambahkan objek Mahasiswa ke dalam daftar mahasiswa jurusan.
        self.daftar_mahasiswa.append(mahasiswa) #digunakan untuk menambahkan objek mahasiswa ke dalam daftar mahasiswa jurusan.
    
    def tampilkan_daftar_mahasiswa(self): #metode yang digunakan untuk menampilkan daftar mahasiswa yang terdaftar dalam jurusan ini.
        print("\nDaftar Mahasiswa di Jurusan", self.nama_jurusan) #mencetak judul "Daftar Mahasiswa di Jurusan" diikuti dengan nama jurusan
        for mahasiswa in self.daftar_mahasiswa: #iterasi melalui setiap objek mahasiswa dalam daftar mahasiswa jurusan
            mahasiswa.tampilkan_info() #memanggil metode tampilkan_info() pada setiap objek mahasiswa tersebut untuk menampilkan informasi mahasiswa.

class Universitas:#kelas universitas
    def __init__(self, nama_universitas):#konstruktor kelas Universitas yang digunakan untuk menginisialisasi objek Universitas.
        self.nama_universitas = nama_universitas #inisialisasi atribut nama_universitas pada objek universitas
        self.daftar_jurusan = []  # merupakan daftar kosong yang digunakan untuk menyimpan daftar jurusan
    
    def tambah_jurusan(self, jurusan): #Metode ini menerima parameter jurusan, yang merupakan objek Jurusan yang akan ditambahkan ke daftar.
        self.daftar_jurusan.append(jurusan) #digunakan untuk menambahkan objek jurusan ke dalam daftar jurusan universitas.
    
    def tampilkan_daftar_jurusan(self): #digunakan untuk menampilkan daftar jurusan yang ada di universitas
        print("\nDaftar Jurusan di Universitas", self.nama_universitas) #mencetak judul "Daftar Jurusan di Universitas" diikuti dengan nama universitas 
        for jurusan in self.daftar_jurusan:# melakukan iterasi melalui setiap objek jurusan dalam daftar jurusan yang ada di objek Universitas.
            print("*", jurusan.nama_jurusan) #mencetak nama jurusan


universitas_xyz = Universitas("XYZ University")# Membuat objek Universitas XYZ

jurusan_ti = Jurusan("Teknik Informatika") #objek jurursan
jurusan_tm = Jurusan("Teknik Mesin")#objek jurursan
jurusan_ars = Jurusan("Arsitektur")#objek jurursan
jurusan_te= Jurusan("Teknik Elektro")#objek jurursan
jurusan_si = Jurusan("Sistem Informasi")#objek jurursan
jurusan_ts = Jurusan("Teknik Sipil")#objek jurursan
universitas_xyz.tambah_jurusan(jurusan_ti) #menambahkan jurusan ke universitas xyz
universitas_xyz.tambah_jurusan(jurusan_tm) #menambahkan jurusan ke universitas xyz
universitas_xyz.tambah_jurusan(jurusan_ars)#menambahkan jurusan ke universitas xyz
universitas_xyz.tambah_jurusan(jurusan_te)#menambahkan jurusan ke universitas xyz
universitas_xyz.tambah_jurusan(jurusan_si)#menambahkan jurusan ke universitas xyz
universitas_xyz.tambah_jurusan(jurusan_ts)#menambahkan jurusan ke universitas xyz

universitas_xyz.tampilkan_daftar_jurusan() # Menampilkan daftar jurusan yang ada di Universitas XYZ

pilihan_jurusan = input("\nMasukkan nama jurusan yang dipilih: ")# Memilih jurusan sesuai daftar jurusan yang tersedia
for jurusan in universitas_xyz.daftar_jurusan: #iterasi melalui setiap objek jurusan dalam daftar jurusan yang ada di objek universitas_xyz.
    if jurusan.nama_jurusan == pilihan_jurusan: #Jika benar maka jurusan tersebut dianggap sebagai jurusan yang dipilih.
        jurusan_terpilih = jurusan #nilai dari variabel jurusan_terpilih diubah menjadi objek jurusan


if jurusan_terpilih: #jika bernilai true atau jurusan ada pada daftar jurusan
    nama_mahasiswa = input("Masukkan nama mahasiswa: ") # Input nama Mahasiswa
    npm_mahasiswa = input("Masukkan NPM mahasiswa: ") # Input  NPM Mahasiswa

    data_mahasiswa = Mahasiswa(nama_mahasiswa, npm_mahasiswa, jurusan_terpilih) # Membuat objek Mahasiswa dengan inputan nama dan NPM, dan memilih jurusan
    jurusan_terpilih.tambah_mahasiswa(data_mahasiswa) #menambahkan objek mahasiswa tersebut ke dalam jurusan terpilih

    # Menampilkan daftar mahasiswa yang terdaftar dalam Jurusan terpilih di Universitas XYZ
    jurusan_terpilih.tampilkan_daftar_mahasiswa() #memanggil metode tampilkan_daftar_mahasiswa pada objek jurusan_terpilih untuk menampilkan daftar mahasiswa yang terdaftar dalam jurusan terpilih di Universitas XYZ.

else:
    print("Jurusan tidak ditemukan.")#jika bernilai false atau jurusan tidak ada pada daftar jurusan

