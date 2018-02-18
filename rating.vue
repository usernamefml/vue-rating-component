<template>
<div>
<div class="rating">
<span>☆</span><span>☆</span><span>☆</span><span>☆</span><span>☆</span>
</div>
</div>
</template>

<script>
export default {
    name: 'StarRating',
    data: function() {
        return {
            data: "star rating"
        }
    }
}
</script>

<style scoped>
.rating {
unicode-bidi: bidi-override;
direction: rtl;
}
.rating > span {
display: inline-block;
position: relative;
width: 1.1em;
}
.rating > span:hover:before,
.rating > span:hover ~ span:before {
 content: "\2605";
 position: absolute;
}
</style>
