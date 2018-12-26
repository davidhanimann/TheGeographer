<template>
    <Page class="page" actionBarHidden=true>
     <StackLayout>
         <Label text="Welcome to The Geographer" height="70" font-size="20pt"/>
         <Label :text="value" @tap="onButtonTap"/>
         <Label text="Welcome to The Geogrsdhfjkashdfjkhjapher"/>
         <Image src="res://icon" stretch="none"/>
         <Slider v-model="value" />
     </StackLayout>
    </Page>
</template>

<script>
    export default {
        data () {
            return {
                value: 0
            }
        },
        computed: {
            message() {
                return "Blank ddd Vue app";
            }
        },
        methods: {
          onButtonTap () {
            console.log('Hello');
          }
        }
    };
</script>

<style scoped lang="scss">
    // Start custom common variables
    @import '../app-variables';
    // End custom common variables

    // Custom styles
    .fa {
        color: $accent-dark;
    }

    .info {
        font-size: 20;
    }
</style>
