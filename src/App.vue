<template>
  <div>
    <NavBar/>
    <section class="home" id="home">
      <div class="content">
        <div class="text">
          <h2>Hi, I'm Ahmad Fadil</h2>
          <p>I enjoy designing websites and coding beautiful simple things</p>
        </div>
        <div class="image">
          <img src="img/ahmadfadil2.jpg" alt="Profile Image">
        </div>
      </div>
    </section>

    <section class="Biodata" id="Biodata">
      <h2 class="heading">Biodata</h2>
      <div class="Biodata_content">
        <div class="personal_info">
          <h2>Data Diri</h2>
          <p>Nama: Ahmad Fadil
          </p>
          <p>Tempat, Tanggal Lahir: Pekanbaru, 18-Desember-2003</p>
          <p>No.hp: 082287423625 </p>
          <p>Email: af0669924@gmail.com </p>
        </div>
        <div class="education">
          <h2>Pendidikan</h2>
          <ul>
            <li>SD 009 kabun</li>
            <li>SMP N 1 kabun</li>
            <li>SMA N 1 kabun</li>
            <li>Universitas Islam Riau</li>
          </ul>
        </div>
        <div class="hobbies">
          <h2>Hobi</h2>
          <ul>
            <li>Futsal</li>
            <li>Billiard</li>
          </ul>
        </div>
      </div>
    </section>

    <section class="Skill" id="Skill">
      <h2 class="heading">Skill</h2>
      <div class="Skill_content">
        <div class="Skill_item">
          <a target="_blank" href="#"><img src="img/ahmadfadil6.jpg" alt="Projek 1"> </a>     
          <h2>Si Darling</h2>
        </div>
       

        <!-- kalau mau nambah ganti yang disini -->
        <!-- <div class="Skill_item2">
          <a target="_blank" href="#"><img src="img/Projek1.jpg" alt="Projek 1"> </a>     
          <h2>Marut</h2>
        </div>
        <div class="Skill_item3">
          <a target="_blank" href="#"><img src="img/Projek1.jpg" alt="Projek 1"> </a>     
          <h2>Marut</h2>
        </div> -->
       
      </div>
    </section>
   
    <section class="Pengalaman" id="Pengalaman">
      <h2 class="heading">Pengalaman</h2>
      <div class="Pengalaman_item">
          <a target="_blank2" href="#"><img src="img/ahmadfadil1.jpg" alt="Projek 1"> </a>     
          <h2>Serifikat ASEAN Cyber Security Programme</h2>
        </div>
    </section>
  </div>
</template>

<script>

import NavBar from './components/NavBar.vue'

export default {
  name: 'App',
  components: {
    NavBar
  }
}
</script>

<style>

#app {
  
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antiapased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #967259; /* Light gray text color */
  background-color: #ece0d1; /* Dark blue background color */
  margin-top: 60px;
}

/* Styles for Home section */
.home {
  min-height: 100vh;
  background-color: #ece0d1; /* Dark blue background color */
  padding: 50px 0;
  display: flex;
  justify-content: center; /* Center content horizontally */
  align-items: center; /* Center content vertically */
}


.home .content {
  display: flex;
  justify-content: center; /* Center content horizontally */
  align-items: center; /* Center content vertically */
  text-align: center; /* Center text horizontally */
}


.home .image img {
  margin-left: 10px; /* Add space between text and image */
  border-left: 4px solid #38220f; /* Dark border to create a line */
  padding-left: 10px; /* Add padding to separate the line from text */
  width: 250px;
  height: 250px;
}

/* Styles for Biodata section */
.Biodata {
  min-height: 100vh;
  background-color: #967259; /* Dark blue background color */
  padding: 50px 0;
  width: 100%; /* Set width to cover full screen */
}

.Biodata h2.heading {
  color: #ece0d1; /* Light gray text color */
  font-size: 32px;
  margin-bottom: 30px;
}

.Biodata_content {
  display: flex;
  flex-wrap: wrap; /* Allow flex items to wrap */
  justify-content: space-around;
}

.personal_info,
.education,
.hobbies {
  flex: 1;
  margin: 0 20px; /* Add margin between sections */
  background-color: #dbc1ac; /* Dark gray background color */
  border-radius: 10px;
  box-shadow: 0 2px 5px rgba(0, 0, 0, 0.1); /* Add shadow */
  padding: 20px;
  transition: transform 0.3s ease; /* Add transition for hover effect */
}

.personal_info:hover,
.education:hover,
.hobbies:hover {
  transform: translateY(-5px); /* Add a slight lift on hover */
}

.personal_info h2,
.education h2,
.hobbies h2 {
  color: #f6f8fa; /* Light gray text color */
  font-size: 24px;
  margin-bottom: 15px;
}

.personal_info p {
  color: #f6f8fa; /* Light gray text color */
  font-size: 18px;
  margin-bottom: 10px;
}

.education ul,
.hobbies ul {
  list-style: none;
  padding: 0;
}

.education ul li,
.hobbies ul li {
  color: #f6f8fa; /* Light gray text color */
  font-size: 18px;
  margin-bottom: 5px;
}

/* Add hover effect to list items */
.hobbies ul li:hover {
  color: #946b2d; /* Dark orange text color on hover */
  font-weight: bold; /* Add bold font on hover */
}

/* Styles for Skill section */
.Skill {
  min-height: 100vh;
  background-color: #dbc1ac; /* Light gray background color */
  padding: 50px 0;
  width: 100%; /* Set width to cover full screen */
}

.Skill h2.heading {
  color: #946b2d; /* Dark orange text color */
  font-size: 32px;
  margin-bottom: 30px; /* Add margin to separate heading from content */
}

.Skill_content {
  display: flex;
  flex-wrap: wrap; /* Allow flex items to wrap */
  justify-content: space-around;
}

.Skill_item,
.Skill_item2,
.Skill_item3 {
  flex: 1;
  margin: 0 20px; /* Add margin between items */
  background-color: #634832; /* Dark gray background color */
  border-radius: 10px; /* Rounded corners */
  box-shadow: 0 2px 5px rgba(0, 0, 0, 0.1); /* Add shadow */
  padding: 20px;
  transition: transform 0.3s ease; /* Add transition for hover effect */
}

.Skill_item:hover,
.Skill_item2:hover,
.Skill_item3:hover {
  
  transform: translateY(-5px); /* Add a slight lift on hover */
}

.Skill_item h2,
.Skill_item2 h2,
.Skill_item3 h2 {
  color: #dbc1ac; /* Light gray text color */
  font-size: 24px;
  margin-bottom: 15px; /* Add margin below heading */
}
.Skill_item img, .Skill_item2 img, .Skill_item3 img{
width: 250px;
height: 250px;
}

/* Add hover effect to images */
.Skill_item img:hover,
.Skill_item2 img:hover,
.Skill_item3 img:hover {
 
  transform: scale(1.1); /* Enlarge image on hover */
}


/* Styles for Pengalaman section */
.Pengalaman {
  min-height: 100vh;
  background-color: #634832; /* Light gray background color */
  padding: 50px 0;
  width: 100%; /* Set width to cover full screen */
}

.Pengalaman h2.heading {
  color: #ece0d1; /* Light red text color */
  font-size: 32px;
}

.Pengalaman p {
  color: #666666; /* Light gray text color */
  font-size: 20px;
}


.Pengalaman_item,
.Pengalaman_item2,
.Pengalaman_item3 {
  flex: 1;
  margin: 0 20px; /* Add margin between items */
  background-color: #ece0d1; /* Dark gray background color */
  border-radius: 10px; /* Rounded corners */
  box-shadow: 0 2px 5px rgba(0, 0, 0, 0.1); /* Add shadow */
  padding: 20px;
  transition: transform 0.3s ease; /* Add transition for hover effect */
}

.Pengalaman_item:hover,
.Pengalaman_item2:hover,
.Pengalaman_item3:hover {
  
  transform: translateY(-5px); /* Add a slight lift on hover */
}

.Pengalaman_item h2,
.Pengalaman_item2 h2,
.Pengalaman_item3 h2 {
  color: #634832; /* Light gray text color */
  font-size: 24px;
  margin-bottom: 15px; /* Add margin below heading */
}
.Pengalaman_item img, .Pengalaman_item2 img, .Pengalaman_item3 img{
width: 250px;
height: 250px;
}

/* Add hover effect to images */
.Pengalaman_item img:hover,
.Pengalaman_item2 img:hover,
.Pengalaman_item3 img:hover {
 
  transform: scale(1.1); /* Enlarge image on hover */
}













</style>
