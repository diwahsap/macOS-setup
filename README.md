# macOS-setup

Hai, ini merupakan catatan dan konfigurasi untuk macOS.

## Jika ingin update OS major, jangan lupa:
1. List semua aplikasi dengan cara ketik `ls -l /Applications` di Terminal. Simpan hasilnya di file.
2. Screenshot kondisi sekarang, siapa tau kangen, hehe.
3. Pastikan sinkronisasi VSCode sudah aktif.
4. Pastikan sudah backup file di Downloads, Documents, dan Desktop.
5. Log out dari iCloud.

## Jika baru _fresh install_, ikuti langkah ini:
### System
1. Check `pmset -g` untuk melihat apakah ada _power management_ yang aktif.
2. Coba _sleep_.

### Terminal-terminal-an
 1. Install Homebrew
`/bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"`
2. Install Iterms2
`brew install --cask iterm2`
3. Install ZSH, Git, Oh My ZSH, Powerlevel10k, and Nerd Fonts. Ikuti Tutorial [ini](https://medium.com/@danieljames/how-to-setup-iterm2-with-zsh-and-powerlevel10k-on-macos-9b9b1b8b3c9a)
4. Install aplikasi yang sering digunakan menggunakan Homebrew. Lihat dari list aplikasi yang sudah diinstall sebelumnya.

### Aplikasi VSCode
1. Login dan sinkronisasi VSCode. 
2. Jangan lupa buat alias untuk VSCode, sesuaikan dengan kebutuhan. Python, LaTeX, dsb.

### Calender
1. Loginkan akun Google ke macOS.
2. Sesuaikan calender dengan acara yang sering digunakan.

### Python
- [Python di Sublime Text](/sublime-text/README.md)

### Git
- [Git, Panduan Ringkas](https://rogerdudler.github.io/git-guide/index.id.html)
- [Password Authentication in GitHub](https://levelup.gitconnected.com/fix-password-authentication-github-3395e579ce74)
- [Using GitHub with SSH (Secure Shell)](https://www.geeksforgeeks.org/using-github-with-ssh-secure-shell/)