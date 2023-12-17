<template>
    <ul>
        <li v-for="goal in goals" :key="goal">
            <!-- scoped slots -->
         <slot :goal="goal" another-prop=".rtyretyry.."></slot>
        </li>
    </ul>
</template>
<script>


export default{
    data(){
       return{
        goals:['Finish the Course', 'Learn Vue']
        } ;
    },
}
</script>
