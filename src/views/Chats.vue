<template>
  <Chartheader/>
  <div v-for="(chat , i) in chats" :key="i">
    <ChatsList :data="chat" />
  </div>

</template>

<script>
    import Chartheader from "../components/chats/Header.vue";
    import ChatsList from "../components/chats/Lists.vue";
export default {
    components: {Chartheader , ChatsList},
    data(){
    return{
      chats:[
      {
        image:"https://yt3.ggpht.com/yti/AJo0G0na7iNN2Q1j4uZ1VNTB82qHboOP7TZArEDIvzATzQ=s108-c-k-c0x00ffffff-no-rj",
        name:"Hitesh Pachora",
        message:"zope ? ",
        time:"11.45 PM",
        count: 3
      },
      {
        image:"https://yt3.ggpht.com/yti/AJo0G0na7iNN2Q1j4uZ1VNTB82qHboOP7TZArEDIvzATzQ=s108-c-k-c0x00ffffff-no-rj",
        name:"Manu sir",
        message:"Hii Hitesh, how are you ? ",
        time:"11.45 PM",
        count: 1
      },
      {
        image:"https://yt3.ggpht.com/yti/AJo0G0na7iNN2Q1j4uZ1VNTB82qHboOP7TZArEDIvzATzQ=s108-c-k-c0x00ffffff-no-rj",
        name:"Aabid",
        message:"kaise ho",
        time:"10.00 PM",
        count: 4
      },
      {
        image:"https://yt3.ggpht.com/yti/AJo0G0na7iNN2Q1j4uZ1VNTB82qHboOP7TZArEDIvzATzQ=s108-c-k-c0x00ffffff-no-rj",
        name:"HR.Pragti",
        message:"Hii sir ",
        time:"9.45 AM",
        count: 1
      },
      {
        image:"https://yt3.ggpht.com/yti/AJo0G0na7iNN2Q1j4uZ1VNTB82qHboOP7TZArEDIvzATzQ=s108-c-k-c0x00ffffff-no-rj",
        name:"Nitin",
        message:"Hii, how are you sir ? ",
        time:"9.45 AM",
        count: 0
      },
    ]
    };
  }

};
</script>

<style>

</style>