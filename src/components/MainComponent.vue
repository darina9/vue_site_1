<template>
          <main class="news">
        <article class="news__banner">          
            
            <div class="news__banner_info">
                <h1 class="news__banner_title big_title">
                     Articles & News
                </h1>
                <p class="news__banner_text text">
                    <a href="#" class="news__banner_link"> Home / Blog</a>
                </p></div>
           
        </article>
        <article class="news__post center">
            <h1 class="news__post_title big_title">
                Latest Post
            </h1>
            <div class="news__post_content">
                <img class="post__content_img" src="../assets/img/post.png">
                <div class="post__content_info">
                    <h2 class="post__content_title little_title">
                        Low Cost Latest Invented Interior Designing Ideas
                    </h2>
                    <p class="post__content_text text">
                        Lorem ipsum dolor sit amet, adipiscing Aliquam eu sem vitae turpis dignissim maximus.posuere in.Contrary to popular belief.</p>
                        <p class="post__content_text text" > Lorem Ipsum is not simply random text. It has roots in a piece of classica.
                    </p>
                    <div class="post__content_date">
                        <p class="date_text">26 December,2022 </p>
                        <button class="date_btn">
                            <img class="date_btn_img" src="../assets/img/arrow.svg">
                        </button> </div>
                </div>
                </div>
            
        </article>
        <article id="news" class="news__news center">
            <div class="news__info news_title">
                <h2 class="news__info_title big_title ">Articles & News</h2>
            </div>
            <div class="news__info_content" >
                <section class="info__content_item" v-for="card in cards" :key="card.id">                   
                    <img class="info__content_picture " :src="card.src" >
                        <button class="info_picture_btn date_text"> {{card.buttonText}} </button>    
                    <h3 class="info__content_title little_title">{{card.title}}</h3>
                    <div class="info__content_date">
                        <p class="date_text">
                            {{card.date}}
                        </p>
                        <button class="date_btn">
                            <img class="date_btn_img" src="../assets/img/arrow.svg">
                           
                        </button> </div>
                </section>             
            </div>
            <div class="news__pagination">
                <button class="date_btn pagination_padding">
                    <p class="date_btn_img date_text pagination_center ">01</p>
                </button> 
                <button class="date_btn">
                    <p class="date_btn_img date_text pagination_center">02</p>
                </button> 
                <button class="date_btn">
                    <p class="date_btn_img date_text pagination_center">03</p>
                </button> 
                <button class="date_btn">
                    <img class="date_btn_img" src="../assets/img/arrow.svg">
                    
                </button> 
            </div>
        </article>
    </main>




 
 
   </template>
   
   <script>
   export default {
     name: 'MainComponent', 
     data(){
      return{
      cards: [
        {
          id: 1,
          src: "../assets/img/blog1.png",
          title: "Let’s Get Solution For Building Construction Work",
          date: "26 December,2022 ",
          buttonText: "Kitchan Design",
        },
        {
          id: 2,
          src: "../assets/img/blog2.png",
          title: "Low Cost Latest Invented Interior Designing Ideas.",
          date: "22 December,2022 ",
          buttonText: "Living Design",
        },
        {
          id: 3,
          src: "../assets/img/blog3.png",
          title: "Best For Any Office & Business Interior Solution",
          date: "25 December,2022 ",
          buttonText: "Interior Design",
        },
        {
          id: 4,
          src: "../assets/img/blog4.png",
          title: "Let’s Get Solution For Building Construction Work",
          date: "26 December,2022 ",
          buttonText: "Kitchan Design",
        },
        {
          id: 5,
          src: "../assets/img/blog5.png",
          title: "Low Cost Latest Invented Interior Designing Ideas.",
          date: "22 December,2022 ",
          buttonText: "Living Design",
        },
        {
          id: 6,
          src: "../assets/img/blog6.png",
          title: "Best For Any Office & Business Interior Solution",
          date: "25 December,2022 ",
          buttonText: "Interior Design",
        },
      ]
      }
    }}
   
   </script>
   
   
   <style scoped >
  * {
  margin: 0;
  padding: 0;
}

.center {
  padding-left: calc(50% - 600px);
  padding-right: calc(50% - 600px);
}

li {
  list-style-type: none;
}

a {
  text-decoration: none;
  color: inherit;
}

.date_text {
  color: #4D5053;
  font-family: Jost;
  font-size: 16px;
  font-style: normal;
  font-weight: 400;
  line-height: 150%;
  letter-spacing: 0.16px;
  text-transform: capitalize;
}

.date_btn {
  border-radius: 180px;
  border: 0;
}

.date_btn_img {
  width: 52px;
  height: 52px;
}

.big_title {
  color: #292F36;
  text-align: center;
  font-family: DM Serif Display;
  font-size: 50px;
  font-style: normal;
  font-weight: 400;
  line-height: 125%;
  letter-spacing: 1px;
}

.text {
  color: #4D5053;
  text-align: center;
  font-family: Jost;
  font-size: 22px;
  font-style: normal;
  font-weight: 400;
  line-height: 150%;
  letter-spacing: 0.22px;
}

.little_title {
  color: #292F36;
  font-family: DM Serif Display;
  font-size: 25px;
  font-style: normal;
  font-weight: 400;
  line-height: 125%;
  letter-spacing: 0.5px;
}

.news__info {
  display: flex;
  flex-direction: column;
  align-items: center;
}
.news__info_text {
  max-width: 737px;
  margin-top: 12px;
}
.news__info_content {
  display: grid;
  grid-template-columns: 1fr 1fr 1fr;
  margin-top: 30px;
  gap: 30px;
}

.info__content_picture {
  min-height: 300px;
  max-width: 340px;
  border-radius: 62px 62px 0 0;
  position: relative;
}
.info__content_item {
  border-radius: 62px;
  border: 1px solid #E7E7E7;
  box-shadow: 0px 10px 30px 0px rgba(255, 255, 255, 0.25);
  padding: 21px;
  display: block;
  justify-content: center;
  align-items: flex-start;
  max-width: 382px;
}
.info__content_title {
  display: flex;
  justify-content: center;
  max-width: 340px;
  margin-top: 21px;
}
.info__content_date {
  display: flex;
  align-items: center;
  justify-content: space-between;
  margin-top: 30px;
}

.info_picture_btn {
  position: absolute;
  margin-top: 250px;
  margin-left: -330px;
  border-radius: 8px 8px 8px 0px;
  background: #FFF;
  padding: 4px 5px 8px 11px;
  border: 0;
}

.info__content_date {
  max-width: 340px;
}


.news {
  margin-top: 50px;
}
.news__banner {
  background: url("../assets/img/banner.jpg") no-repeat;
  background-position: center center;
  display: flex;
  justify-content: center;
  align-items: flex-end;
  min-height: 350px;
  margin-bottom: 200px;
}
.news__banner_info {
  display: flex;
  flex-direction: column;
  align-items: center;
  border-radius: 37px 37px 0px 0px;
  background: #FFF;
}
.news__banner_title {
  padding: 41px 78px 0;
}
.news__banner_text {
  padding: 0 78px 41px;
}
.news__post {
  display: flex;
  flex-direction: column;
  align-items: start;
  gap: 27px;
}
.news__post_content {
  display: flex;
  border-radius: 62px;
  border: 1px solid #E7E7E7;
  box-shadow: 0px 10px 30px 0px rgba(255, 255, 255, 0.25);
  padding: 22px;
}
.news .post__content_img {
  border-radius: 37px;
}
.news .post__content_info {
  padding: 50px;
  display: flex;
  flex-direction: column;
  gap: 25px;
}
.news .post__content_date {
  display: flex;
  gap: 215px;
  margin-top: 40px;
}
.news .post__content_text {
  text-align: start;
}
.news__news {
  margin-top: 150px;
}
.news .news_title {
  align-items: start;
}
.news__pagination {
  margin-top: 51px;
  display: flex;
  gap: 20px;
  justify-content: center;
  margin-bottom: 200px;
}
.news .pagination_center {
  display: flex;
  align-items: center;
  justify-content: center;
}
</style>