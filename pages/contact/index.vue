    <template>
        <div class="contact-info">
        <h2>Contact Information</h2>
        
        <div class="contact-item">
            <h3>Phone Number:</h3>
            <p>{{ contact.phone }}</p>
        </div>
        
        <div class="contact-item">
            <h3>Email Address:</h3>
            <p>{{ contact.email }}</p>
        </div>
    
        <div class="contact-item">
            <h3>Address:</h3>
            <p>{{ contact.address }}</p>
        </div>
    
        <div class="contact-item">
            <h3>Social Media:</h3>
            <ul>
            <li v-for="(link, platform) in contact.socialMedia" :key="platform">
                <a :href="link" target="_blank">{{ platform }}</a>
            </li>
            </ul>
        </div>
    
        <div class="contact-item">
            <h3>Working Hours:</h3>
            <p>{{ contact.workingHours }}</p>
        </div>
        </div>
    </template>
    
    <script>
    export default {
        data() {
        return {
            contact: {
            phone: "+1 (123) 456-7890",
            email: "contact@website.com",
            address: "123 Main St, City, Country",
            socialMedia: {
                Facebook: "https://www.facebook.com/profile.php?id=61558026103264",
                Instagram: "https://twitter.com/yourprofile",
            },
            workingHours: "Mon - Fri: 9:00 AM - 6:00 PM"
            }
        };
        }
    };
    </script>
    
    <style scoped>
    .contact-info {
        max-width: 800px;
        margin: 0 auto;
        padding: 20px;
        background-color: #f9f9f9;
        border-radius: 8px;
        box-shadow: 0 2px 8px rgba(0, 0, 0, 0.1);
    }
    
    h2 {
        text-align: center;
        margin-bottom: 20px;
    }
    
    .contact-item {
        margin-bottom: 20px;
    }
    
    .contact-item h3 {
        margin: 10px 0;
        font-weight: bold;
    }
    
    .contact-item p,
    .contact-item ul {
        margin: 0;
        padding-left: 20px;
    }
    
    ul {
        list-style-type: none;
        padding: 0;
    }
    
    ul li {
        margin: 5px 0;
    }
    
    ul li a {
        color: #007bff;
        text-decoration: none;
    }
    
    ul li a:hover {
        text-decoration: underline;
    }
    </style>
    