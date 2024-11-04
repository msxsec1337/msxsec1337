def generate_github_profile():
    # Ambil data dasar pengguna
    nama = input("Masukkan Nama Anda: ")
    bio = input("Tuliskan bio singkat Anda: ")
    twitch = input("Link Twitch Anda: ")
    website = input("Link Website Anda: ")
    codepen = input("Link Codepen Anda: ")
    linkedin = input("Link LinkedIn Anda: ")

    # Isi README yang dihasilkan
    content = f"""
# Halo 👋🏾 👨🏾‍💻

Hai, saya {nama}! Saya seorang software engineer yang antusias membuat proyek open-source lebih mudah diakses, menciptakan teknologi untuk meningkatkan kualitas hidup, dan membangun komunitas.

Temukan saya di internet 🌎:
- Belajar secara publik di <a href="{twitch}">Twitch</a> atau <a href="{website}">website saya</a> 📹 ✍🏾
- Bereksperimen dengan interaksi di <a href="{codepen}">Codepen</a> 🏓
- Berbagi pembaruan di <a href="{linkedin}">LinkedIn</a> 💼

---

>> BY MSXSEC1337
    """

    # Tulis ke file README.md
    with open("README.md", "w") as file:
        file.write(content)

    print("Profil GitHub telah dibuat! Silakan cek file README.md")

# Panggil fungsi untuk menjalankan program
generate_github_profile()
