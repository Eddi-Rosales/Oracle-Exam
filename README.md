# LPI 010-160 practice exam

The Linux Essentials certificate validates a demonstrated understanding of the following: FOSS, the various communities, and licenses. Knowledge of open source applications in the workplace as they relate to closed source equivalents.

<p align="center">
  <img src="https://www.lpi.org/wp-content/uploads/2023/04/Essentials-Linux_250_0.png" alt="alt text">
</p>

This bash script/[webpage](https://noam-alum.github.io/lpi_010_160_exam/) lets you practice for LPI 010-160 (Linux Essentials) with real questions from the exam.

<hr>

# Take the exam online

You can take the exam online [here](https://noam-alum.github.io/lpi_010_160_exam/).

![Online test](https://noam-alum.github.io/lpi_010_160_exam/hero.webp)

With extensive results:

![results-page](https://noam-alum.github.io/lpi_010_160_exam/results-page.png)

# Installation

## Linux:
### wget
```bash
wget -O lpi_010_160_exam.zip https://codeload.github.com/Noam-Alum/lpi_010_160_exam/zip/refs/heads/main
unzip lpi_010_160_exam.zip
cd lpi_010_160_exam-main/
chmod +x lpi.sh
```
### git clone
```bash
git clone --single-branch --branch main --depth 1 https://github.com/Noam-Alum/lpi_010_160_exam.git
cd lpi_010_160_exam/
chmod +x lpi.sh
```

## Windows:

> If you want to use this bash script on Windows and you have *[WSL](https://blogs.windows.com/windowsdeveloper/2016/03/30/run-bash-on-ubuntu-on-windows/)* you can follow the instructions for **Linux**.

I tested this with [Git bash](https://git-scm.com/downloads), and it works well, first you would have to install **Git bash** on your computer, then you'd have to install [jq](https://github.com/jqlang/jq/releases) for windows and put the exe file in a folder so it can to be included in the $PATH variable, e.g. `[GIT BASH FOLDER]\mingw64\bin` (Usually `C:\Program Files\Git`), finally you can run the script just make sure its has the execute bit on.

### git clone
```bash
git clone --single-branch --branch main --depth 1 https://github.com/Noam-Alum/lpi_010_160_exam.git
cd lpi_010_160_exam/
chmod +x lpi.sh

# ! Make sure you followed the instructions above !
```

<br>
<hr>

# Usage

You can execute the script by simply running:
```bash
./lpi.sh
```
> You must have **jq** installed!

<br>

Then you should get the first question of the bunch, e.g. :
```
noam ◈ noam ⊛ lpi_010_160_exam ⊛ ❯❯ ./lpi.sh 


    ██╗     ██████╗ ██╗    ███████╗██╗  ██╗ █████╗ ███╗   ███╗
    ██║     ██╔══██╗██║    ██╔════╝╚██╗██╔╝██╔══██╗████╗ ████║
    ██║     ██████╔╝██║    █████╗   ╚███╔╝ ███████║██╔████╔██║
    ██║     ██╔═══╝ ██║    ██╔══╝   ██╔██╗ ██╔══██║██║╚██╔╝██║
    ███████╗██║     ██║    ███████╗██╔╝ ██╗██║  ██║██║ ╚═╝ ██║
    ╚══════╝╚═╝     ╚═╝    ╚══════╝╚═╝  ╚═╝╚═╝  ╚═╝╚═╝     ╚═╝


-ˋˏ✄┈┈┈┈ Setting environment ...

 ➣ Validating url.
 ➣ Fetching LPI questions from  https://alum.sh/files/lpi/lpi_questions.json .

-ˋˏ✄┈┈┈┈ Done! ʘ‿ʘ


LPI practice exam:
━━━━━━ʕ•㉨•ʔ━━━━━━━

 ➣ Which of the following tar options handle compression? (Choose two.)

   1) -z
   2) -g
   3) -z2
   4) -bz
   5) -j

   ➣ Answer number 1 (1 - 5):
```

---

>[!NOTE]
> You can also try [jhardoin](https://github.com/jhardoin/)s [Anki deck](https://apps.ankiweb.net/) based on this repo [here](https://github.com/jhardoin/Linux-Essentials/).
