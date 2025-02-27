# Git x Github workflow basic for beginner

## Mengatur config global untuk pertama kali username dan user email, serta mengatur nama default branch(best practicenya mengubah yg default awalnya 'master' menjadi 'main' karena 'main' sesuai dengan kaidah di github
git config --global user.name fauzan hamdi<br>
git config --global user.email fauzanhamdi5@gmail.com<br>
git config --global init.defaultBranch main 

### setelah itu bisa dicek dengan command yg sama tanpa input diakhir
git config --global user.name <br>
(output = fauzan hamdi)

git config --global user.email <br>
(output = fauzanhamdi5@gmail.com)

git config --global init.defaultBranch<br>
(output = main)

### tambahan, command jika ingin melihat semua detail config <br>
git config --list --show-origin
<br>
<br>
## Local Machine
