# Git x Github workflow basic for beginner

![20250301_130353](https://github.com/user-attachments/assets/e37bf948-4579-4580-bfef-db0c5fbb1e2e)

## Mengatur config global untuk pertama kali username dan user email, serta mengatur nama default branch(best practicenya mengubah yg default awalnya 'master' menjadi 'main' karena 'main' sesuai dengan kaidah di github
`git config --global user.name fauzan hamdi` <br>
`git config --global user.email fauzanhamdi5@gmail.com` <br>
`git config --global init.defaultBranch main `

### setelah itu bisa dicek dengan command yg sama tanpa input di akhir
`git config --global user.name` <br>
(output = fauzan hamdi)

`git config --global user.email` <br>
(output = fauzanhamdi5@gmail.com)

`git config --global init.defaultBranch` <br>
(output = main)

### tambahan, command jika ingin melihat semua detail config <br>
`git config --list --show-origin`
<br>
<br>
## Local Machine

1. `git init` => Di folder project di pc kita, command ini digunakan pertama kali untuk mengenerate hidden file .git yg berisi segala functional yg memungkinkan kita menjalankan git workflow di folder kita. <br>
* `ls -a` => Untuk mengecek apakah .git kita sudah muncul.

2. `git add index.js` | `git add .`<br>
=> Menambahkan file2 atau folder2 ke staging area sebelum di commit. ganti nama file dengan titik ( . ) di akhir command jika ingin include semua file dan folder <br>
* `git status` => Mengecek status terkini dari flow git di projek kita.

3. `git commit -m "message here"` =>  Mengcommit file atau folder yg sudah ditambahkan di staging area ke local repo sebelum dipush ke github <br>
* Ada dua shortcut untuk git add dan commit sekaligus : <br>
` git commit -am "message here" ` <br>
` git add . && git commit -m "message here" `

5. `git push` => Jika ingin ngepush pertama kali ke github maka terlebih dahulu harus add new repo di github, kemudian ikuti langkah2 command untuk ` ...or push an existing repository from cli ` yg mana terdiri dari 3 command :<br>
` git remote add origin https://github.com/{github username}/{github repo}.git ` <br>
` git branch -M main `<br>
` git push -u origin main `<br>
tapi untuk push yg kedua kali dan seterusnya cukup dengan `git push`<br>

## Remote Repo(Github)

- `git pull` => Jika sebelumnya sudah pernah push dari local repo ke github dan melakukan perubahan folder atau kode pada file di githubnya langsung. Kemudian ingin perubahan ini juga berlaku di local repo maka cukup menggunakan command `git pull`

- `git clone` => Jika ada repo milik sendiri atau orang lain(yg disetting public) dan ingin mengclonenya ke local repo kita cukup dapatkan path https dari githubnya kemudian command `git clone https://github.com/{github username}/{github repo}.git .` Jangan lupa tambahkan titik di akhir agar diclone di folder saat ini tanpa membuat folder baru dan memasukkan hasil clone di dalamnya.

## What to learn next?

- Branching
- Pull Request
- Merging
- Etc.


### Source : https://www.youtube.com/watch?v=vA5TTz6BXhY&t=1805s
