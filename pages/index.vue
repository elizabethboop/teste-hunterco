
<template>
  <div class="container mb-3 v-card">
    <div class="row">
      <div v-for="(job, i) in jobs":key="i" class="col-sm-3 col-lg-3 col-md-3 v-card__text v-card1 card bg-light mb-3" style="max-width: 18rem;">
          <div class="v-card__text thumbnail text-center">
              <img :src="job.url_banner">
              <div class="caption">
                  <h5 class="pull-right">{{ job.nome_empresa }} - {{ job.vaga }}</h5>
                  <p> {{ job.senioridade }} - {{ job.valor }}</p>
                  <p> {{ job.cidade }}</p>
              </div>
              <button type="button" class="btn btn-primary btn-lg btn-block v-fundo">Conhecer</button>
          </div>
      </div>
    </div>
  </div>
</template>

<script>
import Jobs from '@/components/Jobs.js'
export default {
  data() {
    return {
      jobs: Jobs.getJobs()
    }
  },
}
</script>

<style>

.mb-3{
    margin-bottom: 20px!important
}
.container {
  margin-top: 70px;
}
.v-card {
    display: block;
    border-radius: 2px;
    min-width: 0;
    position: relative;
    text-decoration: none;
    transition: .3s cubic-bezier(.25,.8,.5,1);
    box-shadow: 0 2px 1px -1px rgba(0,0,0,.2), 0 1px 1px 0 rgba(0,0,0,.14), 0 1px 3px 0 rgba(0,0,0,.12);
    text-shadow: 0 0 black;
    background-color: #e5e6e7;
  }

.caption {
    height: 150px;
    overflow: hidden;
}

.caption h4 {
    white-space: nowrap;
}

.thumbnail img {
    width: 100%;
}

.ratings {
    padding-right: 10px;
    padding-left: 10px;
    color: #d17581;
}

.thumbnail {
    padding: 0;
}

.v-fundo{
  background-color: #007b79;
}

.v-card__text {
    padding: 16px;
    width: 100%;
}
.color{
    background-color: #00bfbd;
    color: white;
}

</style>
