<template>
       <footer class="footer center">
        <section class="footer__info">
            <div class="footer__info_logo">
                <img class="logo" src="../assets/img/Logo.svg">
                <h3 class="logo_brend">Interno</h3>
            </div>
            <p class="footer__info_text text">
                It is a long established fact that a reader will be distracted lookings.
            </p>
            <div class="footer__info_social">
                <a href="#">
                    <img src="../assets/img/twitter.svg" alt="twitter"> </a>
                    <a href="#">  
                <img src="../assets/img/in.svg" alt="insta"> </a>
            </div>
        </section>
        <section class="footer__pages">
            <nav class="footer__pages_title little_title">Pages
                <ul class="footer__pages_list">
                    <li class="footer__pages_item text">
                        <a href="#">Home</a>
                    </li>
                    <li class="footer__pages_item text">
                        <a href="#">Project</a>
                    </li>
                    <li class="footer__pages_item text">
                        <a href="#">Blog</a>
                    </li>
                </ul>
            </nav>
        </section>
        <section class=" footer__contacts ">
            <h4 class="footer__contacts_title little_title">
                Contact
            </h4>
            <p class="footer__contacts_text text">
            55 East Birchwood Ave. Brooklyn, New York 11201
            </p>
            <p class="footer__contacts_text text">
            contact@interno.com
            </p>
            <p class="footer__contacts_text text">
            (123) 456 - 7890
            </p>
        </section>
    </footer>


 
   </template>
   
   <script>
   export default {
     name: 'FooterComponent',
     props: {
       
     }
   }
   </script>
   
   
   <style scoped >
.footer {
  display: flex;
  justify-content: space-between;
  margin-top: 96px;
  margin-bottom: 200px;
}
.footer__info_logo {
  display: flex;
  align-items: center;
}
.footer__info_text {
  margin-top: 18px;
  max-width: 393px;
  text-align: start;
}
.footer__info_social {
  margin-top: 31px;
  display: flex;
  gap: 51px;
}
.footer__pages_list {
  display: flex;
  flex-direction: column;
  gap: 30px;
  margin-top: 30px;
}
.footer__contacts {
  display: flex;
  flex-direction: column;
  gap: 21px;
  max-width: 258px;
  align-items: start;
  text-align: start ;
}
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
.text {
  color: #4D5053;  
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

.logo {
  width: 33.998px;
  height: 34px;
  margin-right: 5px;
}
.logo_brend {
  color: #292F36;
  font-family: DM Serif Display;
  font-size: 40px;
  font-style: normal;
  font-weight: 400;
  line-height: 125%;
}

   </style>
   