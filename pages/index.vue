<template lang="pug">
.root
  .topnav.container
    a.active(href='#home') Home
    a(href='#news') Tentang
    a(href='#contact') Struktur Organisasi
    a(href='#about') Program Kerja
  img.blur(src='/img/blur-tagline-section.svg')

  .tagline-section.container
    img.logo(src='/img/logo.svg')
    .tagline SELAMAT DATANG DI HIMATETA IPB
    .tagline-2  Himpunan Mahasiswa Teknik Pertanian dan Biosistem IPB University
  .garis
  
  b-container.mt-4
    b-row
      b-col.box(md="8" offset-md="2")
        .kotak-kuning
          h3 HIMATETA
        p.Penjelasan-himateta
          | Himateta merupakan sebuah organisasi
          | mahasiswa keprofesian yang bergerak dalam
          | bidang keilmuan Teknik Pertanian dan
          | Biosistem, yang meliputi: Teknik Mesin dan Otomasi, Teknik Biosistem, Teknik Energi
          | Terbarukan dan Teknik Bioinformatika
          | Pertanian.
    b-row
      b-col.box(md="4" offset-md="2")
        .kotak-kuning
          h3 Visi
        p.Penjelasan-visi
          | Menjadikan Himateta menjadi himpunan
          | yang berlandaskan teknik pertanian yang
          | bersifat professional dan peduli terhadap
          | lingkungan sekitar.
      b-col.box(md="4")
        .kotak-kuning
          h3 Misi
        ol
          li Meningkatkan kualitas SDM di bidang Teknik Pertanian
          li
            | Berkontribusi dalam pengembangan
            | pertanian Indonesia
          li
            | Menjadikan regenerasi berikutnya
            | menjadi lebih berkualitas
  footer.footer.pt-3
    .kunjungi
      h4.judul Visit Us
      p.isi
        | Depatermen Teknik Pertanian dan Biosistem, Fakultas Teknologi Pertanian IPB University, Jl. Lingkar Akademik, Babakan, Kec. Dramaga, Kabupaten Bogor, Jawa Barat 16680
    .kontak
      h4.judul Contact
      a.isi(href='mailto:himateta.ipb.lk@gmail.com') Email Himateta IPB
      span Dhikma Yogi
      a.isi(href='https://wa.me/083114875030') (083114875030)
    .sosmed
      h4.judul Social Media
      .icon-sosmed
        a(href='https://www.youtube.com/channel/UCNx7SLJvD_6S35kBab5IKVg')
          img.icon-yt(src='/img/youtube.svg')
        a(href='https://open.spotify.com/show/2sijHFTao3QmhfwxPcEVee')
          img(src='/img/spotify.svg')
        a(href='https://www.instagram.com/himatetalk')
          img(src='/img/instagram.svg')
        a(href='https://www.linkedin.com/company/himpunan-mahasiswa-teknik-pertanian-himateta-ipb/about/')
          img(src='/img/linkdin.svg')
  img.blur-4(src='/img/blur-hero-section.svg')

</template>

<script>
import Vue from 'vue'

export default Vue.extend({
  name: 'IndexPage'
})
</script>

<style>
body {
  width:100%;
  position: relative;
}

.container {
    max-width: 1440px;
    width: 100%;
    padding: 0 15px;
    margin: 0 auto;
}

.topnav {
  position: relative;
  top: 0;
}

/* Style the links inside the navigation bar */
.topnav a {
  display: inline-block;
  color: #000000;
  text-align: center;
  padding: 20px 20px;
  left: 0;
  text-decoration: none;
  font-size: 30px;

  font-family: 'IBM Plex Sans';
  font-style: normal;
}

/* Change the color of links on hover */
.topnav a:hover {
  background-color: #ddd;
  color: black;
}

/* Add a color to the active/current link */
.topnav a.active {
  color: #000000;
}

.tagline-section {
  position: relative;
  height: 65vh;
  width: 100%;
  padding: 0 40px;
  margin: 0 auto;
  left: 40px;
}

.logo {
  position: absolute;
  width: 592.39px;
  height: 500px;
  right: 0px;
  top: 35%;
  transform: translateY(-50%);
  z-index: 3;
}

.blur {
  position: absolute;
  height: 50%;
  right:0px;
  top: 0px;
  z-index: 1;
}

.tagline {
  position: relative;
  width: 600px;
  height: 288px;
  padding-top: 40px;

  font-family: 'IBM Plex Sans';
  font-style: normal;
  font-weight: 500;
  font-size: 75px;
  line-height: 80px;

  color: #000000; 
}

.tagline-2 {
  position: relative;
  width: 692px;
  height: 68px;

  font-family: 'Alice';
  font-style: normal;
  font-weight: 400;
  font-size: 30px;
  line-height: 34px;
  text-align: justify;

  color: #000000;
}

.garis {
  position:relative;
  height: 0px;
  left: 0px;
  border-bottom: 2px solid #000000;
}

.hero-section {
  position: relative;
  width: 100%;
  text-align: center;
  padding: 0 15px;
  margin: 20px auto;
}

.hero-section img {
  position: absolute;
  height: 100%;
  z-index: 1;
}


.kotak-kuning {
  width: 100%;
  background: #FFFBE4;
}
.kotak-tentang {
  position: relative;
  width: 244.02px;
  height: 95px;
  left: 30px;

  background: #FFFBE4;
  box-shadow: 0px 4px 4px rgba(0, 0, 0, 0.25);
  border-radius: 50px;
}

.kotak-tentang p {
  position: relative;
  top: 25px;
  left: 25px;
  width:100%;

  font-family: 'IBM Plex Sans';
  font-style: normal;
  font-weight: 600;
  font-size: 40px;
  line-height: 52px;
  display: flex;
  align-items: center;
  text-align: center;

  color: #000000;
}

.box {
  background: rgba(243, 233, 233, 0.2);
}

.box h3 {
  position: relative;

  font-family: 'Alice';
  font-style: normal;
  font-weight: 400;
  font-size: 40px;
  line-height: 46px;
  align-items: center;
  text-align: center;
  margin: 0 auto;
  color: #000000;
}

.box p {
  font-family: 'PT Serif Caption';
  font-style: normal;
  font-weight: 400;
  font-size: 26px;
  line-height: 45px;
  /* or 136% */

  display: flex;
  align-items: center;
  text-align: justify;

  color: #000000;
}


.box li {
  position: relative;
  font-family: 'PT Serif Caption';
  font-style: normal;
  text-align: justify;
  font-weight: 400;
  font-size: 26px;
  line-height: 50px;

  color: #000000;
}

footer {
  position: relative;
  display: flex;
  width: 100%;
  height: 249px;
  justify-content: center;
  background: #000000;
  z-index: 3;
}

.blur-4 {
  position: absolute;
  height: 38%;
  /* left: -316px;
  top: 2093px; */
  z-index: 1;
  bottom: 0;
  left: 0;
}

.kunjungi {
  width: 347px;
  margin-right: 40px;
}

.kunjungi h4 {
  position: relative;
  width: 113px;
  height: 31px;
  font-family: 'Alice';
  font-style: normal;
  font-weight: 400;
  font-size: 24px;
  line-height: 27px;

  color: #FFFAFA;
}

.kunjungi p {
  position:relative;
  width: 347px;
  height: 157px;

  font-family: 'PT Serif Caption';
  font-style: normal;
  font-weight: 400;
  font-size: 20px;
  line-height: 27px;
  /* or 135% */
  text-align: justify;
  color: #FFFBFB;
}

.kontak {
  margin-right: 40px;
}

.kontak h4 {
  position: relative;
  width: 100px;
  height: 25px;
  

  font-family: 'Alice';
  font-style: normal;
  font-weight: 400;
  font-size: 24px;
  line-height: 27px;

  color: #FFFBFB;
}

.kontak a {
  position: relative;
  width: 100px;
  margin: 0 0;

  font-family: 'PT Serif Caption';
  font-style: normal;
  font-weight: 400;
  font-size: 20px;
  line-height: 25px;
  text-decoration: none;
  /* or 125% */
  color: #FFFBFB;
}

.kontak span {
  position: relative;
  width: 100%;
  margin: 0 0;

  display: flex;
  font-family: 'PT Serif Caption';
  font-style: normal;
  font-weight: 400;
  font-size: 20px;
  line-height: 25px;
  /* or 125% */
  color: #FFFBFB;
}

.icon-sosmed {
  display: flex;
  justify-content: flex-start;
}

.sosmed h4 {
  position: relative;
  width: 180px;
  height: 34px;

  font-family: 'Alice';
  font-style: normal;
  font-weight: 400;
  font-size: 24px;
  line-height: 27px;

  color: #FFFEFE;
}

.sosmed a {
  text-decoration: none;
  padding: 0 5px;
}

.icon-sosmed.icon-yt {
  margin-bottom: 10px;
}

.icon-sosmed img {
  vertical-align: middle;
}

</style>
