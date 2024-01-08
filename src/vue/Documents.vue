<script setup>
import { ref } from 'vue'
</script>

<template>
  <div class="documents">
    <header class="documents_header">
      <h1>EMERGENCY MEDICAL SERVICES</h1>
      <h2>EMS</h2>
    </header>
    <section class="documents_section">
      <div class="documents_section-avatar">
        <img src="../ui/img/uAvatar.png">
      </div>
      <div class="documents_section-info">
        <div class="documents_section-info-counter">
          <div class="documents_section-info-count">
            <a>Имя:</a>
            <p>{{ PersName.Name }}</p>
          </div>
          <div class="documents_section-info-count">
            <a>Фамилия:</a>
            <p>{{ PersName.Surname }}</p>
          </div>
        </div>
        <div class="documents_section-info-counter">
          <div class="documents_section-info-count">
            <a>Место жительста:</a>
            <p>{{ Typing.Place }}</p>
          </div>
          <div class="documents_section-info-count">
            <a>Должность</a>
            <p>{{ Typing.Post }}</p>
          </div>
        </div>
      </div>
    </section>
    <footer class="documents_footer">
      <h5>Подпись:</h5>
      <img src="../ui/img/Los-Santos.png" alt="">
    </footer>
  </div>
</template>


<script>
export default {
  name: 'DocumentPage',
  data() {
    return {
      PersName: {
        Name: "Hold",
        Surname: "Xuianov"
      },
      Typing: {
        Place: "Los-Santos",
        Post: "Уебок",
      }
    }
  }
}

</script>


<style>
  @import url(../ui/main.css);
  @import url(../ui/scss/main.scss);
</style>

