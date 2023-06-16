

<template>
    <section class="grid-area3">   
        <div class="msg-box" v-for="item in messagesFromApi"> 
            <p v-if="item.type === 'in'"  class="msg-in" >{{item.message}}</p> 
            <p v-if="item.type === 'out'"  class="msg-out" >{{item.message}}</p>                                                                 
        </div>             
      </section>
</template>

<script>
  export default {
    data() {
      return {
        messagesFromApi: [
        {
          phone: "119999999",
          message: "Mensagem oi",
          type: "out",
          date: "16/03/2023 14:00"
        },
        {
          phone: "119999999",
          message: "Mensagem oi",
          type: "out",
          date: "16/03/2023 14:00"
        }
      ]
      };
    }
  };
</script>

<style scoped>
.grid-area3 {
    height: 65vh;
    box-shadow: 0 0 4px rgba(0,0,0,.14),0 4px 8px rgba(0,0,0,.28);
    background: #CCC9C9;
    overflow: auto;
}

.msg-box {
    display: flex;    
    flex-direction: column;
    gap: 20px;   
    margin-top: 15px;
    color: rgba(255,255,255,.7);
    font-size: 11pt;

}

.msg-in {
    margin-left: 0.3%;
    display: flex;
    margin-right: auto;
    padding: 4px 10px 4px 0px;
    max-width: 70%;
    background: #331f1f;
    border-radius: 0 10px 10px 0;
}

.msg-out {
    margin-right: 0.3%;
    display: flex;
    justify-content: right;
    padding: 4px 0px 4px 10px;
    max-width: 70%;
    margin-left: auto;
    border-radius: 10px 0 0 10px;
    background: #005F4A;
}

</style>
