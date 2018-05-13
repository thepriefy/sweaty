<template>
  <div class="container" style="margin: 0 auto; padding: 0 20px;">
    <div>
      <figure class="image is-3by1" style="margin-bottom: 20px;">
        <img src="https://bulma.io/images/placeholders/720x240.png">
      </figure>
    </div>
    <div class="columns">

      <!-- Personal Records -->
      <div class="column is-hidden-touch">
        <div class="card">
          <header class="card-header">
            <p class="card-header-title">
              Personal Records
            </p>
          </header>
          <div class="card-content">
            <div class="content">
              <p>
                <strong>5 km. :</strong> -
                <br>
                <strong>10 km. :</strong> -
                <br>
                <strong>21 km. :</strong> -
                <br>
                <strong>42 km. :</strong> -
              </p>
            </div>
          </div>
          <footer class="card-footer">
            <a href="#" class="card-footer-item">See all</a>
          </footer>
        </div>
      </div>

      <!-- Latest Activities -->
      <div class="column">
        <div class="card">
          <header class="card-header">
            <p class="card-header-title">
              Latest Activities
            </p>
          </header>
          <div class="card-content">
            <article class="media">
              <div class="media-content">
                <div class="content">
                  <small>Running Activity</small>
                  <div class="columns is-mobile" style="width: 100%;">
                    <div class="column">
                      <strong>5.00 <span style="font-size: 10px;">km.</span></strong>
                    </div>
                    <div class="column" style="font-size: 12px;">
                      <strong>50 <span style="font-size: 10px;">min.</span></strong>
                    </div>
                    <div class="column" style="font-size: 12px;">
                      <strong>10 <span style="font-size: 10px;">min./km.</span></strong>
                    </div>
                  </div>
                </div>
              </div>
            </article>
          </div>
          <footer class="card-footer">
            <a href="#" class="card-footer-item">See all</a>
          </footer>
        </div>
      </div>

      <!-- Latest updates -->
      <div class="column">
        <div class="card">
          <header class="card-header">
            <p class="card-header-title">
              Latest updates
            </p>
          </header>
          <div class="card-content">
            <div class="content">
              Welcome to sweaty
              <br>
              <span style="font-size: 12px;">09 May 2018 11:11 AM.</span>
            </div>
          </div>
          <footer class="card-footer">
            <a href="#" class="card-footer-item">See all</a>
          </footer>
        </div>
      </div>
    </div>
  </div>
</template>
<script>
  export default {
    name: 'app-home'
  }

</script>
