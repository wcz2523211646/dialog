<template>
    <div>
        {{msg}}
    </div>
</template>
<script>
import Dialog from "./js/dialog.js"
export default {
    name: "dilog",
    data() {
        return {
            msg: "666"
        }
    },
    mounted() {
        this.go();
    },
    methods: {
        go() {
            let dialog = new Dialog();
        }
    }
}
</script>
<style>
* {
    margin: 0;
    padding: 0;
}
.dialog {
    width: 300px;
    height: 300px;
    border: 1px solid #f00;
    border-radius: 10px;
    position: absolute;
    top: 0;
    bottom: 0;
    left: 0;
    right: 0;
    margin: auto;
}
.title {
    height: 30px;
    line-height: 30px;
    padding: 10px;
    border-bottom: 1px solid #f00;
}
.content {
    padding: 20px;
    position: relative;
}
.sp{
    margin-right: 15px;
    float: right;
}
.success{
	position: absolute;
	top: 150px;
	left: 5px;
	border: none;
	background: #0f0;
	color: #fff;
	border-radius: 5px;
}
.error{
	position: absolute;
	top: 150px;
	right: 5px;
	border: none;
	background: #f00;
	color: #fff;
	border-radius: 5px;
}
</style>