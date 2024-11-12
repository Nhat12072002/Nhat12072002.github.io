<template>
    <div class="nav-container">
        <ul class="nav-menu">
            <li class="nav-item">Giới thiệu</li>
            <li class="nav-item">Thông tin cá nhân</li>
            <li class="nav-item">Kỹ năng</li>
            <li class="nav-item">Sản phẩm/Dự án</li>
        </ul>
    </div>
</template>

<script setup>

</script>

<style scoped>
.nav-container {
    width: 100%;
    background: #1e1e2f; 
    color: #ffffff;
    display: flex;
    justify-content: center;
    padding: 15px 0;
    box-shadow: 0 4px 6px rgba(0, 0, 0, 0.3);
}

.nav-menu {
    display: flex;
    gap: 25px;
    padding: 0;
    margin: 0;
}

.nav-item {
    list-style: none;
    padding: 10px 15px;
    position: relative;
    cursor: pointer;
    font-size: 18px;
    font-weight: 600;
    color: #b0bec5; 
    transition: color 0.3s ease, transform 0.3s ease;
}

.nav-item:hover {
    color: #007bff; 
    transform: scale(1.1); 
}

.nav-item::after {
    content: "";
    position: absolute;
    width: 0;
    height: 3px;
    background-color: #007bff; 
    bottom: -5px;
    left: 0;
    transition: width 0.3s ease;
}

.nav-item:hover::after {
    width: 100%;
}
</style>
