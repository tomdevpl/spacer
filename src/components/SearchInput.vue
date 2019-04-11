<template>
        <input  
          id="search" 
          name="search"
          :value="value"
          @input="handleChange"
        />
</template>

<script>
export default {
    name: 'SearchInput',
    props: {
        value: {
            type: String,
            required: true,
        },
    },
    methods: {
        handleChange(e) {
            this.$emit('input', e.target.value);
        }
    }
};
</script>

<style <style lang="scss" scoped>
    input {
        margin-top: 50px;
        display: flex;
        flex-direction: column;
        width: 250px;
        color: #fff;
        text-align: center;
        font-size: 18px;
        font-weight: 300;
        height: 30px;
        border: 0;
        background: none;
        border-bottom: 1px solid #fff;
        transition: box-shadow .3s ease-in-out;

        @media (min-width:1024px) {
            font-weight: 400;
        }
    }

    input:focus {
        outline: none;
        box-shadow: 0 10px 10px -10px rgba(255, 255, 255, .5);
    }
</style>