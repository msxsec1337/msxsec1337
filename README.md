def create_readme():
    # Mengambil input dari pengguna
    nama = input("Masukkan nama Anda: ")
    instagram = input("Masukkan URL Instagram Anda: ")
    website = input("Masukkan URL website Anda: ")
    codepen = input("Masukkan URL Codepen Anda: ")
    linkedin = input("Masukkan URL LinkedIn Anda: ")
    twitch = input("Masukkan URL Twitch Anda: ")

    # Konten README.md
    readme_content = f"""# Halo 👋🏾 👨🏾‍💻

Hai, saya **{nama}**! Saya seorang software engineer yang antusias membuat proyek open-source lebih mudah diakses, menciptakan teknologi untuk meningkatkan kualitas hidup, dan membangun komunitas.

## SOSMED

- Belajar secara publik di [Twitch]({twitch}) atau [website saya]({website}) 📹 ✍🏾
- Bereksperimen dengan interaksi di [Codepen]({codepen}) 🏓
- Berbagi pembaruan di [LinkedIn]({linkedin}) 💼
- Ikuti saya di [Instagram]({instagram}) 📸 <img src="https://github.com/gauravghongde/social-icons/raw/master/SVG/Color/Instagram.svg" alt="Instagram" width="48" height="48"/>

---

> BY MSXSEC1337
"""

    # Menyimpan konten ke dalam README.md
    with open("README.md", "w") as readme_file:
        readme_file.write(readme_content)
    
    print("README.md telah dibuat!")

# Menjalankan fungsi
create_readme()
