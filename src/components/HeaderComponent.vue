<template>
   <header class="header center">
        <div class="header__left">
            <img class="logo" src="../assets/img/Logo.svg">       
        <h3 class="logo_brend">Interno</h3>
        </div>
        <nav class="header__right">
            <ul class="header__right_list">
                <li class="header__right_item">
                    <a href="#"> Home </a>
                </li>
                <li class="header__right_item">
                    <a href="#"> Project</a>
                </li>
                <li class="header__right_item">
                    <a href="#"> Blog</a>
                </li>
            </ul>
        </nav>
    </header>   


  </template>
  
  <script>
  export default {
    name: 'HeaderComponent',
    props: {
      
    }
  }
  </script>
  
  
  <style scoped >
 .header {
  margin-top: 51px;
  display: flex;
  align-items: center;
}
.header__left {
  display: flex;
  align-items: center;
}
.header__right {
  padding-left: 780px;
}
.header__right_list {
  display: flex;
  gap: 50px;
}
.header__right_item {
  color: #292F36;
  text-align: center;
  font-family: Jost;
  font-size: 20px;
  font-style: normal;
  font-weight: 400;
  line-height: 125%;
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