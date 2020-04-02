<template>
	<view>
		<text class="mdi" :class="icon" :style="style"></text>     
	</view>
</template>

<script>
    import "./materialdesignicons.min.css";
	export default {
        props: {
            icon: {
                type: String
            }, 
            color: {
                type: String
            },
            size: {
                type: Number,
                default: 20
            }
        },
		data() {
			return {
				
			};
		},
        computed:{
            style() {
                
                return `color: ${this.color}; font-size: ${this.size}px`;
            }
        }
	}
</script>

<style lang="less">

</style>
