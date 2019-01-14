<template>
 <div class="ui card">
     <div class="content">
         <div class="header">
             {{card.term}}
         </div>
         <div class="description">
             {{card.definition}}
         </div>
     </div>
 </div>
</template>

<script>
import Quiz from './Quiz';

export default {
props:['card'],
components: {
    Quiz
}

}
</script>