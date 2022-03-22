<template>
  <Layout>
    <v-container> <v-row><v-col id="portrait"><v-img alt="Mitchell Russell" src="https://github.com/mrusse54/4400/blob/main/portfolio/src/bk.jpg?raw=true" width="400"></v-img ></v-col>
    <v-col ><h1>Hello my name is Blank</h1>
    <h2>I am a Computer Science student at BLANK majoring Software Engineering</h2>
    <h2>I am Currently a senior with a graduation date of Fall 2022</h2>
    <h2>I am exicted to begin a carreer in the Software Engineering feild</h2>
    <h2>I am looking for a job Software Engineering feild</h2>
    <h2>I have experince in	Javascript, C++, HTML, and Vue.js</h2>
    <h2>some more bullshit ...</h2></v-col>
      </v-row>
    </v-container>

<v-container class="indigo accent-3 #3D5AFE">
<v-timeline>
    <v-timeline-item
      v-for="(year, i) in years"
      :key="i"
      :color="year.color"
      small
    >
      <template v-slot:opposite>
        <span
          :class="`headline font-weight-bold ${year.colorText}--text`"
          v-text="year.year"
        ></span>
      </template>
      <div class="py-4 " color="white">
        <h2 :class="`headline font-weight-light mb-4 ${year.colorText}--text`" v-text="year.school">
          
        </h2>
        <div :class="` mb-0 ${year.colorText}--text`" v-text="year.bio" >
          
        </div>
      </div>
    </v-timeline-item>
  </v-timeline>
</v-container>

  </Layout>
</template>

<script>
export default {
  metaInfo: {
    title: "About us",
  },data: () => ({
      years: [
        {
          color: 'blue',
          colorText: 'white',
          year: '1960',
          school: 'Blank',
          bio: 'IDK WHAT I DID THERE',
        },
        {
          color: 'blue',
          colorText: 'white',
          year: '1960',
          school: 'Blank',
          bio: 'IDK WHAT I DID THERE',
        },
        {
          color: 'blue',
          colorText: 'white',
          year: '1960',
          school: 'Blank',
          bio: 'IDK WHAT I DID THERE',
        },
        {
          color: 'blue',
          colorText: 'white',
          year: '1960',
          school: 'Blank',
          bio: 'IDK WHAT I DID THERE',
        },
        {
          color: 'blue',
          colorText: 'white',
          year: '1960',
          school: 'Blank',
          bio: 'IDK WHAT I DID THERE',
        },
      ],
    }),
};
</script>

<style >

#portrait{
  margin-right: -700px;
}


</style>
