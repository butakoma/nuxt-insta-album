<template>
  <section class="container">
    <div class="columns body-columns">
      <div class="column is-half is-offset-one-quarter">
        <card></card>
        <footer class="footer">
          <div class="container is-fluid">
            <div class="content has-text-centered">
              <p>
                <strong>Bulma</strong> by
                <a href="http://jgthms.com">Jeremy Thomas</a>. The source code is licensed
                <a
                  href="http://opensource.org/licenses/mit-license.php"
                >MIT</a>. The website content is licensed
                <a
                  href="http://creativecommons.org/licenses/by-nc-sa/4.0/"
                >CC BY NC SA 4.0</a>.
              </p>
            </div>
          </div>
        </footer>
      </div>
    </div>
  </section>
</template>

<script>
import Card from '@/components/Card.vue'
export default {
  components: {
    Card
  }
}
</script>

<style>
.navbar {
  position: fixed;
  left: 0;
  top: 0;
  z-index: 2;
  background-color: white;
  justify-content: space-around;
  width: 100%;
  border-bottom: 1px solid lightgray;
}
.navbar-menu {
  flex-grow: 0.5;
  justify-content: center;
}
.navbar-menu .navbar-item {
  flex-grow: 1;
  justify-content: center;
}
.navbar-menu .navbar-item .control {
  width: 50%;
}
.body-columns {
  margin-top: 10vh;
}
.card {
  margin-top: 5rem;
}
.card .header {
  padding: 5px 10px;
}
.card-footer .columns {
  width: 100%;
}
.card-footer .columns input {
  border: none;
  border-radius: 0;
  box-shadow: none;
}
.card-footer .columns .column:last-child {
  display: flex;
  align-items: center;
}
.card-footer .columns .column:last-child button {
  border: none;
}
.footer {
  margin-top: 10vh;
  padding: 2rem 1.5rem;
}
</style>
