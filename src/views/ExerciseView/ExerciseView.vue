<template src="./ExerciseView.html">

</template>

<script>
//Components
import BannerComponent from '../../components/ExerciseOneComponents/BannerComponent.vue'
import CardsList from '../../components/ExerciseOneComponents/CardsList.vue'
import AccordionTabComponent from '../../components/ExerciseTwoComponents/AccordionTabComponent.vue'

//Data
import articleData from '../../json/data.json'
export default {
  name: 'ExerciseView',
  components: {
    BannerComponent,
    CardsList,
    AccordionTabComponent
  },
  data: () => {
    return {
      articles: articleData
    }
  }
}
</script>