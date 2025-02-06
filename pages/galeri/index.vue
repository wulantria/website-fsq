
<template>
    <div class="gallery-container">
        <div class="gallery-item">
            <img src="/assets/img/foto1.jpg" alt="Kegiatan 1">
            <p>.....................</p>
        </div>
        <div class="gallery-item">
            <img src="/assets/img/foto2.jpg" alt="Kegiatan 2">
            <p>......................</p>
        </div>
        <div class="gallery-item">
            <img src="/assets/img/foto3.jpg" alt="Kegiatan 3">
            <p>.......................</p>
        </div>
        <div class="gallery-item">
            <img src="/assets/img/foto4.jpg" alt="Kegiatan 4">
            <p>.......................</p>
        </div>
        <div class="gallery-item">
            <img src="/assets/img/foto5.jpg" alt="Kegiatan 4">
            <p>.......................</p>
        </div>
        <div class="gallery-item">
            <img src="/assets/img/foto6.jpg" alt="Kegiatan 4">
            <p>.......................</p>
        </div>
        <div class="gallery-item">
            <img src="/assets/img/foto7.jpg" alt="Kegiatan 4">
            <p>.......................</p>
        </div>
        <div class="gallery-item">
            <img src="/assets/img/foto8.jpg" alt="Kegiatan 4">
            <p>.......................</p>
        </div>
        <div class="gallery-item">
            <img src="/assets/img/foto9.jpg" alt="Kegiatan 4">
            <p>.......................</p>
        </div>
        <div class="gallery-item">
            <img src="/assets/img/foto10.jpg" alt="Kegiatan 4">
            <p>.......................</p>
        </div>
        <div class="gallery-item">
            <img src="/assets/img/foto11.jpg" alt="Kegiatan 4">
            <p>.......................</p>
        </div>
        <div class="gallery-item">
            <img src="/assets/img/foto12.jpg" alt="Kegiatan 4">
            <p>.......................</p>
        </div>
    </div>
</template>

    <style scoped>
        body {
            font-family: Arial, sans-serif;
            margin: 0;
            padding: 0;
            background-color: #f4f4f4;
        }
        header {
            background-color: #333;
            color: white;
            text-align: center;
            padding: 20px 0;
        }
        .gallery-container {
            display: grid;
            grid-template-columns: repeat(auto-fill, minmax(250px, 1fr));
            gap: 15px;
            padding: 20px;
        }
        .gallery-item {
            background-color: white;
            border-radius: 8px;
            box-shadow: 0 4px 8px rgba(0, 0, 0, 0.1);
            overflow: hidden;
            transition: transform 0.3s ease;
        }
        .gallery-item img {
            width: 100%;
            height: auto;
            display: block;
        }
        .gallery-item:hover {
            transform: scale(1.05);
        }
        .gallery-item p {
            padding: 15px;
            text-align: center;
            font-size: 16px;
            color: #333;
            background-color: #fff;
        }
        footer {
            background-color: #333;
            color: white;
            text-align: center;
            padding: 10px;
            position: fixed;
            width: 100%;
            bottom: 0;
        }
    </style>