<script>
window.addEventListener('scroll', function () {
    var container = document.querySelector('.promote-container');
    var containerTop = container.getBoundingClientRect().top;
    var containerHeight = container.offsetHeight;
    var windowHeight = window.innerHeight;
    if (containerTop + containerHeight < windowHeight) {
        container.classList.add('wave');
    } else {
        container.classList.remove('wave');
    }
});
</script>

<template>
    <div class=" promote-container">
        <div class="row">
            <div class="promote-main d-flex justify-content-center">
                <img src="../../../assets/img/下載.jpg " class="promote-main__img" alt="">
                <div style="margin-left: 120px;">
                    <h1 class="content-title">鄭仲智皮包 共享中....
                    <br>
                    歡迎各位！
                </h1>
                <a href="https://thehapp.com/space/result?lat=25.008323165610395&lng=121.45451073244777"
                    class="content-link">一起共襄盛舉 <font-awesome-icon icon="arrow-right" />
                </a>
            </div>
        </div>
        <div class="box">
            <div class="list">
                <div v-for="i in 7" class="photo">{{ i }}</div>
                <!-- 複製一份照片元素，放到列表的最後 -->
                <div v-for="i in 7" class="photo">{{ i }}</div>
                    <!-- <div class="photo">1</div>
                    <div class="photo">2</div>
                    <div class="photo">3</div>
                    <div class="photo">4</div>
                    <div class="photo">5</div>
                    <div class="photo">6</div>
                    <div class="photo">7</div>
                    <div class="photo">1</div>
                    <div class="photo">2</div>
                    <div class="photo">3</div>
                    <div class="photo">4</div>
                    <div class="photo">5</div>
                        <div class="photo">6</div>
                        <div class="photo">7</div> -->
                </div>
            </div>
        </div>
    </div>
</template>


<style>
.box {
    position: relative;
    width: 800px;
    height: 250px;

    overflow: hidden;
    display: flex;
    justify-content: center;
    align-items: center;
}

.list {
    left: 0px;
    display: flex;
    position: absolute;
    
}

.photo {
    width: 344px;
    border: 3px solid red;
    margin-left: 2px;
    font-size: 5rem;
    justify-content: center;
    align-items: center;
    margin-right: 24px;
}

.content-link {
    display: flex;
    align-items: center;
    font-weight: 400;
    font-size: 21px;
    line-height: 1.4;
    letter-spacing: .5px;
    color: #3f916a;
    margin-top: 24px;
}

.content-title {
    font-weight: 500;
    font-size: 34px;
    line-height: 1.4;
    display: flex;
    letter-spacing: .5px;
    color: #4a4a4a;
}

.promote-main__img {
    width: 566px;
    height: 315px;
    border-radius: 8px;
    background: rgba(255, 255, 255, .2);
    background-position: 75% 50%;
    background-repeat: no-repeat;
    background-size: cover;
}

.promote-container {
    position: relative;
    padding: 175px 0;
    margin-bottom: 100px;
    background-color: #fff7f2;
    overflow: hidden;
}
</style>
