def generate_github_profile():
    # Ambil data dasar pengguna
    
    nama = input("Masukkan Nama Anda: samuel ")
    pekerjaan = input("Masukkan Pekerjaan Anda: ")
    bio = input("Tuliskan bio singkat Anda: ")
    project = input("Proyek terbaru Anda: ")
    skill1 = input("Skill utama #1: ")
    skill2 = input("Skill utama #2: ")
    skill3 = input("Skill utama #3: ")
    email = input("Masukkan Email Anda: ")
    linkedin = input("Link profil LinkedIn (opsional): ")
    twitter = input("Username Twitter (opsional): ")
    github_username = input("Masukkan Username GitHub Anda: ")

    # Isi README yang dihasilkan
    content = f"""
<h1 align="center">Hi 👋, I'm {nama}</h1>
<h3 align="center">Saya seorang {pekerjaan}</h3>

<p align="center">{bio}</p>

---

### 🔭 Proyek Terbaru
- 🌟 **{project}**

---

### 🚀 Keahlian Utama
![{skill1}](https://img.shields.io/badge/-{skill1}-blue?style=for-the-badge)
![{skill2}](https://img.shields.io/badge/-{skill2}-blue?style=for-the-badge)
![{skill3}](https://img.shields.io/badge/-{skill3}-blue?style=for-the-badge)

---

### 📫 Hubungi Saya
<p align="left">
  <a href="mailto:{email}"><img src="https://img.shields.io/badge/Email-D14836?style=for-the-badge&logo=gmail&logoColor=white" alt="Email"></a>
  <a href="https://linkedin.com/in/{linkedin}"><img src="https://img.shields.io/badge/LinkedIn-0077B5?style=for-the-badge&logo=linkedin&logoColor=white" alt="LinkedIn"></a>
  <a href="https://twitter.com/{twitter}"><img src="https://img.shields.io/badge/Twitter-1DA1F2?style=for-the-badge&logo=twitter&logoColor=white" alt="Twitter"></a>
</p>

---

### 📊 Statistik GitHub
<p align="center">
  <img src="https://github-readme-stats.vercel.app/api?username={github_username}&show_icons=true&theme=radical" alt="GitHub Stats" />
  <img src="https://github-readme-streak-stats.herokuapp.com/?user={github_username}&theme=radical" alt="GitHub Streak" />
</p>

### 🌟 Proyek Unggulan
<p align="left">
  <a href="https://github.com/{github_username}/repository1"><img src="https://github-readme-stats.vercel.app/api/pin/?username={github_username}&repo=repository1&theme=radical" alt="Project 1" /></a>
  <a href="https://github.com/{github_username}/repository2"><img src="https://github-readme-stats.vercel.app/api/pin/?username={github_username}&repo=repository2&theme=radical" alt="Project 2" /></a>
</p>

---

### 💬 Tentang Saya
- 💼 Saat ini bekerja sebagai {pekerjaan}
- 👨‍💻 Saya suka belajar hal baru di bidang {skill1}, {skill2}, dan {skill3}

---

> Dibuat dengan ❤️ oleh {nama}
    """

    # Tulis ke file README.md
    with open("README.md", "w") as file:
        file.write(content)

    print("Profil GitHub telah dibuat! Silakan cek file README.md")

# Panggil fungsi untuk menjalankan program
generate_github_profile()
