

<template>
    <section class="grid-area3">            
        <div class="msg-box">                                       
            <p class="msg-in" >Lorem ipsum dolor sit amet, consectetur</p>                                                                  
            <p class="msg-out">adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation</p>
            <p class="msg-out">sit amet, consectetur, adipisci</p>
            <p class="msg-in" >But I must explain to you how all this mistaken idea of denouncing pleasure and praising pain was born and I will give you a complete account of the system, and expound the actual teachings of the great explorer of the truth, the master-builder of human happiness. No one rejects,</p>  
            <p class="msg-out">dislikes, or avoids pleasure itself, because it is pleasure, but because those who do not know how to pursue pleasure rationally encounter consequence</p>
            <p class="msg-in" >which of us ever undertakes laborious physical exercise, except to obtain some advantage from it? But who has any right to find fault with </p>  
            <p class="msg-in" >usto odio dignissimos ducimus qui blanditiis praese</p>  
            <p class="msg-out">Et harum quidem rerum facilis est et expedita distinctio. Nam libero tempore, cum soluta nobis est eligendi optio cumque nihil imped</p>
            <p class="msg-in" >Et harum quidem rerum facilis est et expedita distinctio. Nam libero tempore, cum soluta nobis est eligendi optio cumque nihil impedit quo minus id quod maxime placeat facere possimus, omnis voluptas assumenda est, omnis dolor repellendus. Temporibus autem quibusdam et aut officiis debitis aut rerum necessitatibus saepe eveniet ut et voluptates repudiandae sint et molestiae non recusandae. Itaque earum rerum hic tenetur a sapiente delectus, ut aut reiciendis voluptatibus maiores alias consequatur aut perferendis doloribus asperior</p>  
        </div>             
      </section>
</template>

<script>
  export default {
    data() {
      return {
        dynamicContents: ['Conteúdo dinâmico 1', 'Conteúdo dinâmico 2']
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
    display: flex;
    margin-right: auto;
    padding: 4px 10px 4px 0px;
    max-width: 70%;
    background: #331f1f;
    border-radius: 0 10px 10px 0;
}

.msg-out {
    display: flex;
    justify-content: right;
    padding: 4px 0px 4px 10px;
    max-width: 70%;
    margin-left: auto;
    border-radius: 10px 0 0 10px;
    background: #005F4A;
}

</style>
