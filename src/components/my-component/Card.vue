<template>
     <div class="card-service">

          <h1>{{ title }}</h1>
          <p>{{ description }}</p>
          <slot></slot>
          <button class="btn-service">Detail</button>
          <!-- <MyBtn></MyBtn> -->

     </div>
</template>

<script>
export default {
     props: ['title', 'description']
}
</script>

<style scoped>
.btn-service
{
     margin-right: 1px;
     margin-bottom: 30px;
     margin-top: 10px;
     font-size: 16px;
     font-weight: 400;
     color: white;
     background-color: purple;
     padding: 15px 20px;
     border: none;
     border-radius: 5px;
}

.card-service
{
     text-align: start;
     min-height: 206px;
     padding: 30px 30px 0 30px;
     box-shadow: 0px 10px 30px rgba(0, 0, 0, 0.05);
     border-radius: 60px 0px 0px 0px;
     background: white;
     transition: all 0.5s ease;
     margin: 10px 10px;
}

.card-service h2
{
     font-size: 18px;
     line-height: 30px;
     color: #343b4e;
}

.card-service p
{
     font-weight: 400;
     color: #827f8d;
     margin: 0 0 10px 0;
}
</style>