

<template>
    <section class="grid">
      <div class="chat-window">
        <div v-for="content in dynamicContents" class="box msg-box">
          <div>
            {{ content }}
          </div>
        </div>
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

.grid {
    background-color: tomato;
    max-width: 700px;
    max-height: 75vh;
    box-shadow: 0 0 4px rgba(0,0,0,.14),0 4px 8px rgba(0,0,0,.28);
}
.chat-window {
    min-height: 40vh;
    max-height: 47vh;
    display: flex;
    flex-direction: column;
    background-color: #CCC9C9;
    overflow: auto;
}
.box{
    display: flex;
    min-height: 2vh;
    min-width: 30%;
    max-width: 35%;
    margin-top: 3vh;
    padding: 10px 10px 0 10px;
    color: whitesmoke;
}
.msg-box {
    background: #331f1f;
    border-radius: 0 10px 10px 0;
    box-shadow: 0 0 2px rgba(0,0,0,.12),0 2px 4px rgba(0,0,0,.24);
}

.msg {
    display: flex;
    font-size: 11pt;
    color: rgba(255,255,255,.7);
    margin: 0 0 10px 0;
}

.msg-self {
    display: flex;
    align-self: end;
    border-radius: 10px 0 0 10px;
    background: #005F4A;
}

</style>
