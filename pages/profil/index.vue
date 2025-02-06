<template>
    <div class="profile-card">
        <img src="/assets/img/profil.jpg" alt="Profile Image" class="profile-image" />
        <div class="profile-info">
            <!-- Welcome text now above and left-aligned -->
            <h2 class="text-left">Hello, Welcome to My Website!</h2>
            <p class="text-left"><strong>Name:</strong> {{ profile.name }}</p>
            <p class="text-left"><strong>Birthdate:</strong> {{ profile.birthdate }}</p>
            <p class="text-left"><strong>Address:</strong> {{ profile.address }}</p>
            <p class="text-left"><strong>Contact:</strong> {{ profile.contact }}</p>
            <p class="text-left"><strong>Education:</strong> {{ profile.education }}</p>
            <p class="text-left"><strong>Social Media:</strong> {{ profile.socialMedia }}</p>
            <p class="text-left"><strong>Bio:</strong> {{ profile.bio }}</p>
        </div>
    </div>
</template>

<script>
export default {
    data() {
        return {
            imageSrc: "https://via.placeholder.com/150",
            profile: {
                name: "Kiyotaka Ayanokouji",
                birthdate: "2000-01-01",
                address: "Tokyo, Japan",
                contact: "0101010101",
                education: "High School Student",
                socialMedia: "@kiyotaka_aya",
                bio: "A quiet, strategic thinker with hidden depths."
            }
        };
    }
};
</script>

<style scoped>
.profile-card {
    display: flex;
    align-items: center;
    gap: 20px;
    padding: 20px;
    border: 1px solid #ccc;
    border-radius: 10px;
    max-width: 100%;
    background-color: #f9f9f9;
}

.profile-image {
    width: 468px;
    height: 642px;
    object-fit: cover;
    border-radius: 10%;
}

.profile-info {
    flex: 1;
    text-align: left;
}

h2.text-left {
    text-align: center; 
    margin-bottom: 20px;
}

p {
    margin: 10px 0;
}
</style>
