<template>
    <div class="wrapper">
        <ul class="tab-menu" >
            <li v-for="( article, index) in articles" :key="article.id" class="tab-item">
              <button @click="setActiveTab(index,'large')" :class="{ 'is-active':  activeTab === index }" class="tab-trigger-item tab-title" :data-target="'tab' + (index)">{{  article.title }}</button>
            </li>
     
        </ul>
        
        <ul class="tab-section">
        <li v-for="(article, index) in articles" :key="article.id" class="tab-item">
            <button 
              :class="{ 'is-active': activeTab === index }" 
              class="tab-trigger-item tab-title" 
              :data-target="'tab' + (index)" 
              @click="setActiveTab(index,'small')">{{  article.title }}</button>
                <div v-if="activeTab === index" :id="'tab' + (index)" :class="{ 'is-active': activeTab === index }" class="tab-content">
                    <div v-html=" article.content"></div>
                </div>
        </li>
        </ul>
        <div class="spacer xxx-large"></div>
    </div>
</template>

<script>
export default {
     name: 'AccordionTabComponent',
     props: ['articles'],
     data() {
        return {
          activeTab: 0 
        };
      },
     methods: {
      setActiveTab(index,size) {
         
          if(this.activeTab == index && size == "small") {
            this.activeTab = -1;
          }else {
            this.activeTab = index;
          }
        }
      }

}
</script>

