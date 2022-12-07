<template>

    <div :class="book.released? 'red': 'grey100' ">
        <h2> {{book.movieName}}</h2>
        <h4> {{book.year}}</h4>
        <h4> {{book.rating}} </h4>
        <h4> {{book.Genres}} </h4>
    </div>

</template>

<script>


export default{
    name: 'BookItem',
    props:{
        book: Array
    }
}


</script>

<style scoped>


h4{
    margin: 5px;
}

div{
    background-color: #91a0a1;
    color: black;
    padding: 1em;
}

.red{
background-color: orangered ;

}
.grey{
    background-color: rgb(63, 60, 60);
}


</style>