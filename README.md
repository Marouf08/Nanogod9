<p align="center">
  <a href="https://git.io/typing-svg">
    <img src="https://readme-typing-svg.demolab.com?font=EB+Garamond&weight=800&size=28&duration=4000&pause=1000&random=false&width=435&lines=+NANO_GOD_BUG;WHATSAPP+CRASH+x+BUG+BOT;DEVELOPED+BY+𝐊𝐀𝐍𝐆+𝐉𝐈𝐍𝐇𝐘𝐔𝐊" alt="Typing SVG" />
  </a>
</p>

![Nanogod9](https://files.catbox.moe/dohubs.jpg)
<p align="center">
<a href="https://youtube.com/@ssk-familycampagny"><img src="https://img.shields.io/badge/YouTube-ff0000?style=for-the-badge&logo=youtube&logoColor=ff000000&link=https://youtube.com/@ssk-familycampagny" /><br>
<a href="https://whatsapp.com/channel/0029Vajrhmz96H4IsEjh4a41"><img src="https://img.shields.io/badge/WhatsApp Channel-25D366?style=for-the-badge&logo=whatsapp&logoColor=white&link=https://whatsapp.com/channel/0029VaG9VfPKWEKk1rxTQD20" /><br>
<a href="https://t.me/+13472314632"><img src="https://img.shields.io/badge/Telegram-00FFFF?style=for-the-badge&logo=telegram&logoColor=white" />
---

## DEVELOPED BY 𝐊𝐀𝐍𝐆 𝐉𝐈𝐍𝐇𝐘𝐔𝐊

---

## CREATE YOUR FORK
<a href="https://github.com/Gungun243/Nanogod9/fork">
  <img title="DEMON-CELESTE" src="https://img.shields.io/badge/FORK-DEMON-CELESTE-red?color=red&style=for-the-badge&logo=stackshare">
</a>

---

### 🔐 Generate Pair Code For Session

#### PAIRING SERVER 
<a href="https://drk-tech-1.onrender.com/" target="_blank">
  <img alt="Pairing Code Server " src="https://img.shields.io/badge/PAIRING CODE-green?style=for-the-badge&logo=opencv&logoColor=white"/>
</a>

---


  
---

## ⚠️ WARNING ⚠️

I am not responsible for any damage caused by this bot. Use this bot at your own risk. It is developed for educational purposes only. Any malicious use is strictly discouraged.

---

<details>
  <summary><strong>Show more</strong></summary>


---

## Developer 💀

<a href="https://github.com/Gungun243">
  <img src="https://github.com/Gungun243.png" width="200" height="200" alt="NAOFUMI-SAMA"/>
</a>
<p align="center"><strong>NAOFUMI-SAMA</strong></p>

---

## Contributors 🤝

<a href="https://github.com/BarryAllen100">
  <img src="https://github.com/BarryAllen100.png" width="200" height="200" alt="BarryAllen100"/>
</a>
<p align="center"><strong>BarryAllen100</strong>

---

## GitHub Deployment

```yaml
name: Node.js CI

on:
  push:
    branches:
      - main
  pull_request:
    branches:
      - main
  schedule:
    - cron: '0 */6 * * *'  

jobs:
  build:

    runs-on: ubuntu-latest

    strategy:
      matrix:
        node-version: [20.x]

    steps:
    - name: Checkout repository
      uses: actions/checkout@v3

    - name: Set up Node.js
      uses: actions/setup-node@v3
      with:
        node-version: ${{ matrix.node-version }}

    - name: Install dependencies
      run: npm install

    - name: Install FFmpeg
      run: sudo apt-get install -y ffmpeg

    - name: Start application with timeout
      run: |
        timeout 21590s npm start  # Limits run to 5h 59m 50s

    - name: Save state (Optional)
      run: |
        ./save_state.sh
