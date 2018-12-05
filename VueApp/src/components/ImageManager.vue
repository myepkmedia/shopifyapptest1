<template>
  <div class="hello">
    <div class="section">

<div class="container">

    <div class="columns">

      <div class="column is-two-fifths">
        
        <h1 class="title has-text-centered">{{ title }}</h1>
        
          <heading>Image Options</heading>
<div class="field">
  <label class="label">Select date</label>
<input type="date"/>
</div>
<div class="field">
  <label class="label">Select time</label>
<input type="time" id="timeCheck"/>
</div>
<div class="field">
  <label class="label">Schedule Your Image</label>
<a class="button is-info is-focused" @click="handleClick">Submit</a>
</div>


    </div>
      <div class="column is-four-fifths">
          <carousel>

              <img src="https://placeimg.com/200/200/any?1">
              <img src="https://placeimg.com/200/200/any?2">
              <img src="https://placeimg.com/200/200/any?3">
              <img src="https://placeimg.com/200/200/any?4">
              <img src="https://placeimg.com/200/200/any?5">
              <img src="https://placeimg.com/200/200/any?6">
              <img src="https://placeimg.com/200/200/any?7">
              <img src="https://placeimg.com/200/200/any?8">

            </carousel>
            <carousel>
                <template slot="prev"><span class="prev">prev</span></template>
                <template slot="next"><span class="next">next</span></template>
            </carousel>

            
      
      </div>
    </div>
  </div>

    </div>

    </div>
</template>

<script>
import carousel from 'v-owl-carousel'


export default {
  components: { 
    carousel 
  },
  methods: {
    handleClick: function() {
      
    }
  },
  name: 'ImageManager',
  data () {
    return {
      title: "Admin"
    }
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>


</style>
