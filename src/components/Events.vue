<script setup>
import{ref} from "vue"
const events = ref([
    {
        name:"Community Outreach at Northern Kenya",
        image:"../../public/Images/daniel-mtombosola-IC36xB8p_iY-unsplash.jpg",
        date:"July 6th 2025",
        location:"Northern Kenya School",
        category:"Community Outreach",


    },
    {
        name:"Food Festvial",
        image:"../../public/Images/victoria-shes-UC0HZdUitWY-unsplash - Copy.jpg",
        date:"July 1st 2025",
        location:"Jamuhuri Sports Grounds",
        category:"Food",


    },
    {
        name:"Sports Day",
        image:"../../public/Images/473404032_1945665719297789_6006268278205799850_n.jpg",
        date:"July 14th 2025",
        location:"Ulinzi Sports Complex",
        category:"Sports",


    },
    {
        name:"Software Development Bootcamp",
        image:"../../public/Images/mohammad-rahmani-N5bT5RctFZ8-unsplash.jpg",
        date:"August 1st 2025",
        location:"Jitegemee University",
        category:"Technology and IT",


    }

])

</script>

<template>
    <v-container>
        <v-row>
            <v-col md = "4" v-for = "event in events" :key = "event">
                 <v-card
    class="mx-auto"
    max-width="280"
    color="blue"


  >
    <v-img
      class="align-end text-white"
      height="200"
      :src="event.image"
      cover
    >
      <v-card-title>{{ event.name }}</v-card-title>
    </v-img>

    <v-card-subtitle class="pt-4">
      {{ event.date }}
    </v-card-subtitle>

    <v-card-text>
      <div>{{ event.location }}</div>

      <div>Nairobi,Kenya</div>
    </v-card-text>

    <v-card-actions>
      <v-btn color="orange" :text="event.category"></v-btn>

      <v-btn color="orange" text="Explore"></v-btn>
    </v-card-actions>
  </v-card>

            </v-col>
        </v-row>
    </v-container>
 
</template>