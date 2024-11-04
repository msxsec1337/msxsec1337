def generate_github_profile():
    # Ambil data dasar pengguna
    nama = input("Masukkan Nama Anda: ")
    pekerjaan = input("Masukkan Pekerjaan Anda: ")
    bio = input("Tuliskan bio singkat Anda: ")
    project = input("Proyek terbaru Anda: ")
    skill1 = input("Skill utama #1: ")
    skill2 = input("Skill utama #2: ")
    skill3 = input("Skill utama #3: ")
    email = input("Masukkan Email Anda: ")
    linkedin = input("Link profil LinkedIn (opsional): ")
    twitter = input("Username Twitter (opsional): ")

    # Isi README yang dihasilkan
    content = f"""
# Halo 👋, Saya {nama}!

Saya adalah seorang {pekerjaan}. {bio}

---

### 🔭 Proyek Terbaru
Saya sedang mengerjakan **{project}**.

---

### 🚀 Keahlian Utama
- {skill1}
- {skill2}
- {skill3}

---

### 📫 Hubungi Saya
- **Email**: {email}
- **LinkedIn**: [{linkedin}](https://linkedin.com/in/{linkedin}) (opsional)
- **Twitter**: [@{twitter}](https://twitter.com/{twitter}) (opsional)

---

![Profil Statistik GitHub](https://github-readme-stats.vercel.app/api?username=USERNAME&show_icons=true&theme=radical)

"""

    # Tulis ke file README.md
    with open("README.md", "w") as file:
        file.write(content)

    print("Profil GitHub telah dibuat! Silakan cek file README.md")

# Panggil fungsi untuk menjalankan program
generate_github_profile()
