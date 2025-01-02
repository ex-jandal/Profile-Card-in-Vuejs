<script setup>
import profileImage from '@/assets/profile_image.jpg';
</script>

<template>
  <!-- Boxicons Package -->
  <link href='https://unpkg.com/boxicons@2.1.4/css/boxicons.min.css' rel='stylesheet'>
  <div id="app">
  <div class="profile-card">
        <div class="image">
            <img src="./assets/profile_image.jpg" alt="profile-photo" class="profile-img">
        </div>

        <div class="info-text">
            <span class="name">Ex.Jandal</span>
            <span class="detalis">Cybersecurity Interest & Blogger</span>
        </div>

        <div class="media-account">
            <a href="https://www.x.com/ex_jandal" class="link">
                <i class='bx bxl-twitter'></i>
            </a>
            <a href="https://www.instagram.com/ex.jandal/" class="link">
                <i class='bx bxl-instagram'></i>
            </a>
            <a href="https://github.com/ex-jandal" class="link">
                <i class='bx bxl-github'></i>
            </a>
            <a href="https://linktr.ee/ex.jandal" class="link">
                <i class='bx bx-link-external'></i>
            </a>
        </div>

        <div class="buttons">
            <button onclick="window.location.href='https://linktr.ee/ex.jandal';" class="button">Visit My Web</button>
            <button onclick="window.location.href='https:///wa.me/00967776491899?text=Hello%20there!';" class="button">Massage Me</button>
        </div>
    </div>
  </div>
</template>

<style scoped>

.profile-card {
    display: flex;
    flex-direction: column;
    align-items: center;
    max-width: 400px;
    width: 100%;
    background-color: hsl(0, 0%, 100%);
    box-shadow: 0 5px 10px rgba(0, 0, 0, 0.1);
    border-radius: 25px;
    padding: 25px;
    position: relative;
}

.profile-card::before {
    content: '';
    position: absolute;
    top: 0;
    left: 0;
    border-radius: 25px 25px 0 0;
    height: 36%;
    width: 100%;
    background-color: hsl(230, 39%, 36%);
}
.image {
    position: relative;
    height: 150px;
    width: 150px;
    border-radius: 50%;
    background-color: hsl(230, 39%, 36%);
    padding: 3px;
    margin-bottom: 10px;
}

.image .profile-img {
    height: 100%;
    width: 100%;
    object-fit: cover;
    border-radius: 50%;
    border: 3px solid hsl(0, 0%, 100%);
}

.profile-card .info-text {
    display: flex;
    flex-direction: column;
    align-items: center;
    color: hsl(0, 0%, 16%);
}

.info-text .name {
    font-size: 22px;
    font-weight: 500;
}

.info-text .detalis {
    font-size: 15px;
    font-weight: 400;
}

.profile-card .media-account {
    display: flex;
    align-items: center;
    margin-top: 15px;
}

.media-account .link {
    display: flex;
    align-items: center;
    justify-content: center;
    color: hsl(0, 0%, 100%);
    font-size: 18px;
    height: 35px;
    width: 35px;
    border-radius: 50%;
    margin: 0 8px;
    text-decoration: none;
    background-color: hsl(230, 39%, 36%);
    transition: color,background-color 0.3s ease;
}

.profile-card .buttons {
    display: flex;
    align-items: center;
    margin-top: 25px;
}

.buttons .button {
    border: none;
    border-radius: 25px;
    color: hsl(0, 0%, 100%);
    font-size: 14px;
    font-weight: 400;
    padding: 8px 24px;
    margin: 0 10px;
    background-color: hsl(230, 39%, 36%);
    cursor: pointer;
    transition: color,background-color 0.3s ease;
}

.buttons .button:hover, .link:hover {
    background-color: hsl(0, 0%, 85%);
    color: hsl(230, 39%, 36%);
}

</style>
