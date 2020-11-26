Docker adalah platform perangkat lunak yang memungkinkan Anda membuat, menguji, dan menerapkan aplikasi dengan cepat. Docker mengemas perangkat lunak ke dalam unit standar yang disebut kontainer yang memiliki semua yang diperlukan perangkat lunak agar dapat berfungsi termasuk pustaka, alat sistem, kode, dan waktu proses. Dengan menggunakan Docker, kita dapat dengan cepat menerapkan dan menskalakan aplikasi ke lingkungan apa pun dan yakin bahwa kode kita akan berjalan. Docker merupakan sebuah alat untuk membuat, men-deploy, menjalankan aplikasi dengan menggunakan kontainer. Simpelnya adalah docker akan membungkus aplikasi kita dengan kontainer yang kemudian kontainer tersebut akan dijalankan pada saat development & digunakan pada saat deployment. Docker berfungsi dengan menyediakan cara standar untuk menjalankan kode kita. 

Fitur Docker
o	Docker Engine, digunakan untuk membangun Docker images dan membuat kontainer Docker.
o	Docker Hub, registry yang digunakan untuk berbagai macam Docker images
o	Docker Compose, digunakan untuk mendefinisikan aplikasi menggunakan banyak kontainer Docker.
o	Docker untuk Mac, memungkinkan menjalankan kontainer Docker pada Mac.
o	Docker untuk Linux, memungkinkan menjalankan kontainer Docker pada Linux.
o	Docker untuk Windows, memungkinkan menjalankan kontainer Docker pada Windows.

Cara Kerja Docker
•	Docker image, merupakan file berisi informasi dan petunjuk untuk membangun container. Image juga berfungsi untuk menggunakan dan mengirimkan informasi;
•	Container, adalah lingkungan untuk mengemas dan menjalankan aplikasi. Ini mencakup kode, runtime, system tools, dan pengaturan. Container hanya bisa mengakses resource yang telah ditentukan dalam docker image;
•	Docker client, yaitu tempat di mana pengguna dapat mengirimkan perintah seperti docker build, docker pull, dan docker run kepada Docker daeomon;
•	Docker Engine Rest API, digunakan untuk berinteraksi dengan Docker daemon. Ini bisa diakses klien melalui HTTP;
•	Docker host, menyediakan lingkungan yang lengkap untuk menjalankan aplikasi. Dia bertanggung jawab terhadap penerimaan perintah yang diberikan Docker client;
•	Docker daemon, yaitu proses pengelolaan Docker images, kontainer, network, dan storage volumes. Docker daemon menerima request dari Docker API dan akan memprosesnya;
•	Docker registry, wadah untuk menyimpan Docker image. Docker image akan memberi reaksi sesuai perintah yang diberikan. Misalnya saat diberi perintah docker push, docker image akan didorong atau dibagikan ke registri Docker Hub;
•	Docker Hub adalah layanan yang disediakan untuk menemukan dan berbagi gambar container dengan tim.

Instalasi Docker
Untuk melakukan instalasi docker, kita update terlebih dahulu repository ubuntu anda dengan perintah.
	sudo apt update
Kemudian lakukan update CA certificates dengan perintah.
	sudo apt install apt-transport-https ca-certificates curl software-properties-common
Kemudian tambahkan GPG key dengan perintah.
	curl -fsSL https://download.docker.com/linux/ubuntu/gpg | sudo apt-key add -
Lalu lakukan verifikasi fingerprint dengan perintah
	sudo apt-key fingerprint 0EBFCD88
Jika berhasil maka akan muncul output seperti berikut
	pub   4096R/0EBFCD88 2017-02-22
	Key fingerprint = 9DC8 5822 9FC7 DD38 854A  E2D8 8D81 803C 0EBF CD88
	uid                  Docker Release (CE deb) <docker@docker.com>
	sub   4096R/F273FCD8 2017-02-22
Lalu tambahan repo docker seperti berikut
sudo add-apt-repository "deb [arch=amd64] https://download.docker.com/linux/ubuntu $(lsb_release -cs) stable"
Kemudian lakukan update kembali dengan perintah.
	sudo apt update
Kemudian hapus docker yang lama jika pernah melakukan instalasi docker versi lama dengan perintah.
	sudo apt purge lxc-docker
Lalu jalankan perintah berikut untuk melakukan instalasi docker.
	sudo apt install docker-ce

lalu lakukan pengecekan status service docker dengan perintah.
	sudo systemctl status docker
jika berhasil maka akan muncul output seperti berikut.
 
Agar dapat menggunakan docker tanpa sudo maka kita harus melakukan beberapa konfigurasi. Kita buat docker group dengan perintah berikut.
	sudo groupadd docker
kemudian tambahkan user ke docker group dengan perintah.
	sudo usermod -aG docker rizki
kita ganti dengan user linux kita. Lalu silahkan restart komputer. Kita akan melakukan test docker dengan perintah.
	docker run hello-world
Jika berhasil maka kita akan melihat output seperti gambar berikut.
 

Docker-compose adalah sebuah alat dari docker yang digunakan untuk mendefinisikan dan menjalankan aplikasi multi kontainer. Dengan docker-compose kita bisa menjalankan kontainer 1 dengan yang lainya dengan 1 perintah . Docker-compose juga menggunakan yaml file untuk menyimpan konfigurasi dari service yang dibuat.
Dengan docker-compose kita dapat menghubungkan dan menjalankan aplikasi kontainer dengan mudah . Kita dapat mengkontainerisasi aplikasi kita dan dengan menggunakan docker-compose dan juga untuk menjalankan aplikasi kontainer hanya dalam satu perintah. Docker compose ini sangat berguna ketika aplikasi kita terpisah - pisah pada komputer yang berbeda, contohnya adalah aplikasi yang dibuat berada pada 1 container sedangkan database yang akan digunakan oleh aplikasi tersebut berada pada container yang lain. Ketika menggunakan docker compose maka kita dapat menjalankan kedua container tersebut secara bersamaan dan bahkan kita dapat melakukan link ke container yang kita inginkan.

Instalasi Docker Compose
Untuk melakukan instalasi docker compose kita jalankan perintah berikut untuk melakukan akses root.
	sudo -s
kemudian jalankan perintah berikut.
curl -L https://github.com/docker/compose/releases/download/1.22.0/docker-compose-`uname -s`-`uname -m` -o /usr/local/bin/docker-compose
Setelah selesai lalu beri hak akses eksekusi dengan perintah.
	chmod +x /usr/local/bin/docker-compose
Lalu agar docker compose dapat diakses tanpa root, silahkan jalankan perintah berikut.
	sudo chmod -R 777 /usr/local/bin/docker-compose
Kemudian lakukan pengecekan docker compose dengan perintah
	docker-compose -version
Jika berhasil maka akan muncul output seperti berikut.
	docker-compose version 1.22.0, build 9e633ef

