<template>
    <div class="searchWrapper">
        <input  
          id="search" 
          v-model="searchValue"
          @input="handleInput"
        />
    </div>
</template>

<script>
export default {
    name: 'SearchInput',
}
</script>

<style <style lang="scss" scoped>
    .searchWrapper {
        margin-top: 50px;
        display: flex;
        flex-direction: column;
        width: 250px;
  }

    input {
        height: 30px;
        border: 0;
        background: none;
        border-bottom: 1px solid #fff;
  }
</style>
