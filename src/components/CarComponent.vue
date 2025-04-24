<script>
export default {
    props: {
        colorClass: {
            type: String,
            default: 'orangeBack'
        }
    }
}

</script>

<template>
    <div class="[colorClass]">
        <slot></slot>
    </div>

</template>

<style scoped>
.orangeBack {
    background-color: hsl(31, 77%, 52%);
    width: fit-content;
    border-radius: 6px 0 0 6px;
    padding: 42px;
}

.darkcyanBack {
    background-color: hsl(184, 100%, 22%);
    width: fit-content;
    padding: 42px;
}

.verydarkcyanBack {
    background-color: hsl(179, 100%, 13%);
    width: fit-content;
    border-radius: 0 6px 6px 0;
    padding: 42px;
}

@media (max-width: 800px) {
    .orangeBack {
        border-radius: 6px 6px 0 0;

    }

    .verydarkcyanBack {
        border-radius: 0 0 6px 6px;
    }
}
</style>