<template>
  <div class="home">
    <div class="container">
      <div class="card is-mobile">
        <div class="card-content has-text-centered">
          <div class="title">Jadwal Uas Gan!</div>
          <Table></Table> <br>
          <div class="content has-text-left">PS: ini Matkul yang diambil semuanya, matkul tambahan kontak Dheja aja kalo mau ditambahin</div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
// @ is an alias to /src
import Table from '../components/Table'

export default {
  name: 'home',
  components: {
    Table
  }
}
</script>
