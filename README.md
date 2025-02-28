# Git x Github workflow basic for beginner

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

3. `git commit -m "message here"` =>  Mengcommit file atau folder yg sudah ditambahkan di staging area ke local repo sebelum dipush ke github

4. `git push` => Jika ingin ngepush pertama kali ke github maka terlebih dahulu harus add new repo di github, kemudian ikuti langkah2 command untuk ` ...or push an existing repository from cli ` yg mana terdiri dari 3 command :<br>
` git remote add origin https://github.com/{github username}/{github repo}.git ` <br>
` git branch -M main `<br>
` git push -u origin main `<br>
tapi untuk push yg kedua kali dan seterusnya cukup dengan `git push`<br>

## Remote Repo(Github)

- `git pull` =>
