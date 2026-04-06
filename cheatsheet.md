# 📋 Cheatsheet WSL & Git

## 🖥️ WSL / Linux Commands

### Navigasi
| Command | Fungsi |
|--------|--------|
| `pwd` | Lihat lokasi sekarang |
| `ls` | Lihat isi folder |
| `ls -la` | Lihat isi folder + file tersembunyi |
| `cd nama_folder` | Masuk ke folder |
| `cd ..` | Balik ke folder sebelumnya |
| `cd ~` | Langsung ke home directory |

### File & Folder
| Command | Fungsi |
|--------|--------|
| `mkdir nama_folder` | Bikin folder baru |
| `touch nama_file` | Bikin file baru |
| `rm nama_file` | Hapus file |
| `rm -rf nama_folder` | Hapus folder beserta isinya |
| `cp file1 file2` | Copy file |
| `mv file1 file2` | Rename / pindah file |
| `cat nama_file` | Lihat isi file |
| `echo 'teks' > file` | Tulis teks ke file |

### Nano (Text Editor)
| Command | Fungsi |
|--------|--------|
| `nano nama_file` | Buka file di nano |
| `Ctrl + X` | Keluar |
| `Ctrl + O` | Save |
| `Ctrl + W` | Search |
| `Y` lalu `Enter` | Konfirmasi save & keluar |

### Lain-lain
| Command | Fungsi |
|--------|--------|
| `clear` | Bersihkan terminal |
| `sudo` | Jalankan sebagai admin |
| `apt install nama` | Install package |
| `ping google.com` | Test koneksi internet |

---

## 🐙 Git Commands

### Setup Awal
git config --global user.name "username"
git config --global user.email "email@gmail.com"
git config --list

### Inisialisasi Repo
git init
git clone <url>

### Workflow Sehari-hari
git status
git add .
git add nama_file
git commit -m "pesan"
git push
git pull

### Branch
git branch
git branch nama_branch
git checkout nama_branch
git merge nama_branch

### Remote
git remote add origin <url>
git remote set-url origin <url>
git remote -v
git push -u origin main

### SSH
ssh-keygen -t ed25519 -C "email"
cat ~/.ssh/id_ed25519.pub
ssh -T git@github.com

### Log & Undo
git log --oneline
git diff
git restore nama_file
git reset HEAD~1
