<!-- Container for profile section with animated typing text -->
<div style="text-align: center; padding: 20px;">
    <img src="https://github.com/khushii-23/khushii-23/blob/main/Pixel%20BG%20-%20Apartment%20_%20Kerotheraphy%5B18%2B%5D.gif" style="width: 100%; max-width: 800px;" alt="logo" />
    <h1 style="font-family: 'Courier New', Courier, monospace; color: #f0f0f0;">
        <span id="typed-text"></span><span class="cursor">|</span>
    </h1>
    <h3 style="color: #00e676;">A Passionate Website Developer from India</h3>
</div>

<!-- Profile details -->
<p align="left">
    <img src="https://komarev.com/ghpvc/?username=khushii-23&label=Profile%20views&color=0e75b6&style=flat" alt="Profile Views" />
</p>

<ul>
    <li>🌱 I’m currently learning <strong>MERN</strong></li>
    <li>👨‍💻 Check out all my projects at <a href="https://github.com/khushii-23/" target="_blank" style="color: #00e676;">GitHub</a></li>
    <li>📫 How to reach me: <strong>ch.khushi826@gmail.com</strong></li>
    <li>📄 Learn more about my experiences: <a href="https://www.canva.com/design/DAGFA6TTHJw/zq35RgeF3J57um97JNuPeQ/edit?utm_content=DAGFA6TTHJw&utm_campaign=designshare&utm_medium=link2&utm_source=sharebutton" target="_blank" style="color: #00e676;">Resume</a></li>
</ul>

<!-- Social media icons with hover animation -->
<h3 align="left">Connect with me:</h3>
<p align="left">
    <a href="https://linkedin.com/in/khushi-bhakar-a9a485309/" target="blank">
        <img src="https://raw.githubusercontent.com/rahuldkjain/github-profile-readme-generator/master/src/images/icons/Social/linked-in-alt.svg" alt="LinkedIn" width="40" height="40" style="margin-right: 10px; transition: transform 0.3s ease;" onmouseover="this.style.transform='scale(1.1)'" onmouseout="this.style.transform='scale(1)'"/>
    </a>
    <a href="https://instagram.com/_khushi_bhakar/" target="blank">
        <img src="https://raw.githubusercontent.com/rahuldkjain/github-profile-readme-generator/master/src/images/icons/Social/instagram.svg" alt="Instagram" width="40" height="40" style="margin-right: 10px; transition: transform 0.3s ease;" onmouseover="this.style.transform='scale(1.1)'" onmouseout="this.style.transform='scale(1)'"/>
    </a>
    <a href="https://discord.gg/casual_khush_35606" target="blank">
        <img src="https://raw.githubusercontent.com/rahuldkjain/github-profile-readme-generator/master/src/images/icons/Social/discord.svg" alt="Discord" width="40" height="40" style="transition: transform 0.3s ease;" onmouseover="this.style.transform='scale(1.1)'" onmouseout="this.style.transform='scale(1)'"/>
    </a>
</p>

<!-- Languages and tools with glow effect on hover -->
<h3 align="left">Languages and Tools:</h3>
<p align="left">
    <a href="https://www.cprogramming.com/" target="_blank">
        <img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/c/c-original.svg" alt="C" width="40" height="40" style="margin-right: 10px; transition: all 0.3s ease;" onmouseover="this.style.filter='brightness(1.5)'" onmouseout="this.style.filter='none'"/>
    </a>
    <a href="https://www.w3schools.com/cpp/" target="_blank">
        <img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/cplusplus/cplusplus-original.svg" alt="C++" width="40" height="40" style="margin-right: 10px; transition: all 0.3s ease;" onmouseover="this.style.filter='brightness(1.5)'" onmouseout="this.style.filter='none'"/>
    </a>
    <a href="https://developer.mozilla.org/en-US/docs/Web/JavaScript" target="_blank">
        <img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/javascript/javascript-original.svg" alt="JavaScript" width="40" height="40" style="margin-right: 10px; transition: all 0.3s ease;" onmouseover="this.style.filter='brightness(1.5)'" onmouseout="this.style.filter='none'"/>
    </a>
    <a href="https://reactjs.org/" target="_blank">
        <img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/react/react-original-wordmark.svg" alt="React" width="40" height="40" style="margin-right: 10px; transition: all 0.3s ease;" onmouseover="this.style.filter='brightness(1.5)'" onmouseout="this.style.filter='none'"/>
    </a>
</p>

<!-- GitHub stats section with smooth scroll animation -->
<div style="text-align:center;">
    <p><img src="https://github-readme-stats.vercel.app/api/top-langs?username=khushii-23&show_icons=true&locale=en&layout=compact" alt="Top Languages" style="animation: fadeIn 2s;" /></p>
    <p><img src="https://github-readme-stats.vercel.app/api?username=khushii-23&show_icons=true&locale=en" alt="GitHub Stats" style="animation: fadeIn 2.5s;" /></p>
    <p><img src="https://github-readme-streak-stats.herokuapp.com/?user=khushii-23&" alt="GitHub Streak Stats" style="animation: fadeIn 3s;" /></p>
</div>

<!-- Typing animation script -->
<script>
    const textArray = ["Hello, I'm Khushi Bhakar"];
    let i = 0, j = 0, currentText = "", isDeleting = false, speed = 100;

    function typeWriter() {
        if (i < textArray.length) {
            if (!isDeleting && j < textArray[i].length) {
                currentText += textArray[i].charAt(j);
                j++;
                document.getElementById("typed-text").innerHTML = currentText;
                speed = 100;
            } else if (isDeleting && j > 0) {
                currentText = currentText.slice(0, --j);
                document.getElementById("typed-text").innerHTML = currentText;
                speed = 50;
            }

            if (j === textArray[i].length && !isDeleting) {
                isDeleting = true;
                speed = 2000;
            } else if (isDeleting && j === 0) {
                isDeleting = false;
                i++;
                if (i >= textArray.length) i = 0;
            }
        }
        setTimeout(typeWriter, speed);
    }

    window.onload = function() {
        setTimeout(typeWriter, 500);
    }
</script>

<!-- CSS for smooth animations -->
<style>
    @keyframes fadeIn {
        0% { opacity: 0; }
        100% { opacity: 1; }
    }
    .cursor {
        font-weight: 100;
        font-size: 24px;
        color: #00e676;
        animation: blink 0.7s infinite;
    }
    @keyframes blink {
        0%, 100% { opacity: 1; }
        50% { opacity: 0; }
    }
</style>
