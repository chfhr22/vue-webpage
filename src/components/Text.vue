<template>
    <section id="textType" :class="['text__wrap', element]">
        <span class='blind'>텍스트 유형</span>
        <h2>{{ title }}</h2>
        <div class="text__inner container">
            <div :class="['text', text.name]" v-for="(text, key) in textInfo" :key="key">
                <h3 class="title">{{ text.title }}</h3>
                <p class="desc">{{ text.desc }}</p>
                <a href="/" class="btn">더보기</a>
            </div>
        </div>
    </section>
</template>
<script>
export default {
    props: {
        element: String,
        title: String
    },
    data: function () {
        return {
            textInfo: [
                {
                    name: "t1",
                    title: "검색 이팩트",
                    desc: "자바스크립트의 기본 메서드를 통해 검색 스크립트를 완성하는 튜토리얼입니다.",
                },
                {
                    name: "t2",
                    title: "클릭 이팩트",
                    desc: "자바스크립트의 기본 메서드를 통해 검색 스크립트를 완성하는 튜토리얼입니다.",
                },
                {
                    name: "t3",
                    title: "찾기 이팩트",
                    desc: "자바스크립트의 기본 메서드를 통해 검색 스크립트를 완성하는 튜토리얼입니다.",
                },
                {
                    name: "t4",
                    title: "보기 이팩트",
                    desc: "자바스크립트의 기본 메서드를 통해 검색 스크립트를 완성하는 튜토리얼입니다.",
                },
                {
                    name: "t5",
                    title: "오버 이팩트",
                    desc: "자바스크립트의 기본 메서드를 통해 검색 스크립트를 완성하는 튜토리얼입니다.",
                },
                {
                    name: "t6",
                    title: "검색 이팩트",
                    desc: "자바스크립트의 기본 메서드를 통해 검색 스크립트를 완성하는 튜토리얼입니다.",
                }
            ]
        }
    }
}
</script>