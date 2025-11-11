<template>
    <form>
            <label>Başlık</label>
            <input type="text" v-model="title" required>
            <label>İş Detayı</label>
            <textarea v-model="details" required></textarea>
            <button>Ekle</button>
    </form>
</template>

<script>
export default {
    data(){
        return{
            title:'',
            details:''
        }
    }
}
</script>

<style>

</style>