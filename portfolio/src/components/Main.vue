<script>
import Modal from '@/components/Modal.vue';

export default {
  name: 'App',
  components: {
    Modal,
  },
  data() {
    return {
      isModalVisible: false,
      isModalVisible1: false,
      isModalVisible2: false,
    };
  },
  methods: {
    showModal() {
      this.isModalVisible = true;
    },
    closeModal() {
      this.isModalVisible = false;
    },
    showModal1() {
      this.isModalVisible1 = true;
    },
    closeModal1() {
      this.isModalVisible1 = false;
    },
    showModal2() {
      this.isModalVisible2 = true;
    },
    closeModal2() {
      this.isModalVisible2 = false;
    }
  }
};
function clicbouton(){
    firstname.value=""
    lastname.value=""
    object.value=""
    message.value=""
}
</script>

<template>
    <h1>Adrien Godon</h1>
    <h2>Développeur web junior</h2>
    <h3 id="presentation">Présentation</h3>
    <p id="pres">Je suis actuellement en formation Développeur web et web mobile et je recherche un emploi en tant que développeur web junior.</p>
    <h3 id="creations">créations</h3>
    <div class="app">
      <p>Créez votre CV en HTML et CSS</p>
      <button type="button" class="btn" @click="showModal">
        <img src="@/assets/images/Cv.png" alt="Cv">
      </button>
      <Modal v-show="isModalVisible" @close="closeModal">
        <template v-slot:header>
            Créez votre CV en HTML et CSS
        </template>
        <template v-slot:body>
          <img src="@/assets/images/Cv.png" alt="Cv">
          <br/>
          <a href="https://github.com/IssoukaBlyat/Devoir_CV">https://github.com/IssoukaBlyat/Devoir_CV</a>
        </template>
        <template v-slot:footer>
          <p>Date de création : <date datetime="2023-09-29">29 septembre 2023</date></p>
        </template>
      </Modal>
    </div>
    <div class="app">
      <p>Rédiger un cahier des charges</p>
      <button type="button" class="btn" @click="showModal1">
        <img src="@/assets/images/cahier.png" alt="Cahier des charges">
      </button>
      <Modal v-show="isModalVisible1" @close="closeModal1">
        <template v-slot:header>
            Rédiger un cahier des charges
        </template>
        <template v-slot:body>
            <img src="@/assets/images/cahier.png" alt="Cahier des charges">
          <br/>
          <a href="https://https://github.com/IssoukaBlyat/Devoir_CV">https://https://github.com/IssoukaBlyat/Devoir_CV</a>
        </template>
        <template v-slot:footer>
          <p>Date de création : <date datetime="2023-10-12">12 octobre 2023</date></p>
        </template>
      </Modal>
    </div>
    <div class="app">
        <p>Dynamiser un espace commentaire</p>
      <button type="button" class="btn" @click="showModal2">
        <img src="@/assets/images/dynamism.png" alt="Dynamiser un espace de commentaire">
      </button>
      <Modal v-show="isModalVisible2" @close="closeModal2">
        <template v-slot:header>
            Dynamiser un espace commentaire
        </template>
        <template v-slot:body>
          <img src="@/assets/images/dynamism.png" alt="Dynamiser un espace de commentaire">
          <br/>
          <a href="https://github.com/IssoukaBlyat/Dynamiser-un-espace-commentaire">https://github.com/IssoukaBlyat/Dynamiser-un-espace-commentaire</a>
        </template>
        <template v-slot:footer>
          <p>Date de création : <date datetime="2023-10-26">26 octobre 2023</date></p>
        </template>
      </Modal>
    </div>
    <h3 id="contact">Contact</h3>
    <form action="mailto:adrien.godon@hotmail.com" method="post" enctype="text/plain">
        <div>
            <input type="text" name="firstname" placeholder="Prénom">
        </div>
        <div>
            <input type="text" name="lastname" placeholder="Nom">
        </div>
        <div>
            <input type="text" name="object" placeholder="Objet">
        </div>
        <div>
            <textarea name="message" cols="30" rows="10" placeholder="Écrire votre message"></textarea>
        </div>
        <input type="button" value="Envoyer le message." onclick="clicbouton()">
    </form>
</template>

<style scoped>
    * {
        text-align: center;
    }

    .app button {
        width: 500px;
    }

    .app p {
        text-decoration: underline;
    }

    img {
        width: 50%;
        height: 50%;
    }

    a {
        color: black;
        text-decoration: none;
    }

    #pres {
        margin-left: 250px;
        margin-right: 250px;
    }

    h3 {
        margin-left: 425px;
        margin-right: 425px;
        text-decoration: underline ;    
    }

    button {
        border-radius: 15%;
    }

    input, textarea {
        margin-top: 10px;
        border-radius: 15%;
    }
</style>