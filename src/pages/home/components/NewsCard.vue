<script setup lang="ts">
import { NDivider, NCard, NButton, darkTheme, NGradientText } from 'naive-ui'
</script>

<template>
    <n-config-provider :theme="darkTheme">
        <n-gradient-text class="title" :gradient="{
            deg: 90,
            from: 'rgb(255, 255, 255)',
            to: 'rgb(170, 170, 170)',
        }">
            电波湮灭 - E-Vanish
        </n-gradient-text>
        <br />
        <n-gradient-text class="content" :gradient="{
            deg: 90,
            from: 'rgb(255, 255, 255)',
            to: 'rgb(255, 255, 255)',
        }">
            -------------------------------------------------------------------------<br />
            电波湮灭E-Vanish将于2025年8月15日与知名音乐厂牌「漂流瓶DRIFT BEATS」第二次联动决定<br />
            本次联动将收录来自音乐厂牌的曲目，作为电波湮灭E-Vanish音游专区体验区Phira原创新手教程。
        </n-gradient-text>
        <br />
        <br />
        <br />
        <n-gradient-text t class="hinded" :gradient="{
            deg: 90,
            from: 'rgb(255, 255, 255)',
            to: 'rgb(255, 255, 255)',
        }">
            它是：<br />
            「Afterg■■■.wav」<br />
            by ■■■■<br />
        </n-gradient-text>
        <br />
        <n-gradient-text class="content" :gradient="{
            deg: 90,
            from: 'rgb(255, 255, 255)',
            to: 'rgb(255, 255, 255)',
        }">
            敬请期待！
        </n-gradient-text>
    </n-config-provider>
</template>

<style scoped>
.title {
    font-size: 5vw;
    font-weight: bold;
    color: rgba(0, 0, 0, 0);
}

.content {
    font-size: 1.5vw;
    font-weight: bold;
    color: rgba(0, 0, 0, 0);
}

.hinded {
    position: flex;
    justify-content: center;
    align-items: center;
    width: 100%;
    text-align: center;
    font-size: 3vw;
    color: rgba(0, 0, 0, 0);
}
</style>
