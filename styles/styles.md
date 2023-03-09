# Revision Autoprefixer


```css
/*
* Prefixed by https://autoprefixer.github.io
* PostCSS: v8.4.14,
* Autoprefixer: v10.4.7
* Browsers: last 4 version
*/

@import url('https://fonts.googleapis.com/css2?family=Nunito+Sans:ital,wght@0,400;0,600;0,700;1,400;1,700&family=Roboto:ital,wght@0,400;0,700;0,900;1,400;1,500&display=swap');

:root {
  /* espacios */
  /* --padding100: 100px 0; */

  /* básicos */
  --woodsmoke: #131415;
  --white: #ffffff;
  --woodsmoke-025: #13141535;

  /* primarios */
  --tuna: #383c43;
  --silver-sand: #c1c7c7;
    --silver-tree: #64b49d;
    --shuttle-gray: #5c6d80;
    --pine-cone: #725d54;
    --horizon: #5d8aab;
    --apple-blossom: #ab4e42;
    --amazon: #377a60;
    --skin: #FBBEBE;
    --skined: #E2ABAB;

  /* effects */
  --gradient: linear-gradient(#c1c7c7 0%, #383c43 10%, #131415);
  --gradient-tree: linear-gradient(45deg, #64b49d, #377a60);
  --gradient-green: linear-gradient(45deg, #64b49d 25%, #377a60 75%);
  --gradient-tea: linear-gradient(90deg, #ffffff, #FBBEBE 10%, #ab4e42 70%);
  --time-animation: 0.3s;
}
*{
  -webkit-box-sizing: border-box;
          box-sizing: border-box;
  margin: 0;
  padding: 0;
  /* outline: 3px solid limegreen !important; */

}
body{
  font-family: 'Roboto', sans-serif;
  font-family: 'Nunito Sans', sans-serif;
  -webkit-box-sizing: border-box;
          box-sizing: border-box;
  margin: 0;
  color: #c1c7c7;
  display: -webkit-box;
  display: -ms-flexbox;
  display: flex;
  -webkit-box-orient: vertical;
  -webkit-box-direction: normal;
      -ms-flex-direction: column;
          flex-direction: column;
  
}
a{
    text-decoration: none;
    color: var(--white);
 }
 
h1{
  text-shadow: 1px 1px 1px var(--horizon), 3px 3px 2px var(--horizon);
}
.body::-webkit-scrollbar {
  width: 8px;
  background: var(--tuna);
}

.body::-webkit-scrollbar-thumb {
  background: var(--amazon);
  border-radius: 4px;
}

/*-----------MENU DE NAVEGACIÓN------------*/
.header {
  color: var(--white);
  padding: 1rem;
  margin: 0;
  width: 100%;
  display: -webkit-box;
  display: -ms-flexbox;
  display: flex;
  -webkit-box-orient: horizontal;
  -webkit-box-direction: normal;
      -ms-flex-direction: row;
          flex-direction: row;
  -webkit-box-pack: center;
      -ms-flex-pack: center;
          justify-content: center;
  background: var(--tuna);
  position: fixed;
  z-index: 10;
}

.nav__menu{
  width: 95%;
  display: -webkit-box;
  display: -ms-flexbox;
  display: flex;
  -webkit-box-orient: horizontal;
  -webkit-box-direction: normal;
      -ms-flex-direction: row;
          flex-direction: row;
  -webkit-box-pack: end;
      -ms-flex-pack: end;
          justify-content: flex-end;
  -ms-flex-line-pack: end;
      align-content: end;
}

.nav__ul{
  width: 35rem;
  display: -webkit-box;
  display: -ms-flexbox;
  display: flex;
  -webkit-box-pack: space-evenly;
      -ms-flex-pack: space-evenly;
          justify-content: space-evenly;
  -ms-flex-line-pack: center;
      align-content: center;
  -webkit-box-align: baseline;
      -ms-flex-align: baseline;
          align-items: baseline;
}

.nav__list{
  list-style: none;
  color: var(--white);
  padding: 9px 0;
}

.nav__links{
  background: var(--amazon);
  text-decoration: none;
  height: 19px;  
  font-family: 'Nunito Sans';
  font-style: normal;
  font-size: 16px;
  line-height: 19px;
  -webkit-box-align: center;
      -ms-flex-align: center;
          align-items: center;
  padding: 9px 16px;
  border-radius: 8px;
  -webkit-box-shadow: 4px 4px 4px rgba(0, 0, 0, 0.2);
          box-shadow: 4px 4px 4px rgba(0, 0, 0, 0.2);
}

.nav__links:hover {
  background-color: var(--silver-tree);
  border-radius: 8px;
}

.nav__links:focus{
  background: var(--silver-tree);
  border: solid 1px var(--white);
  -webkit-box-shadow: none;
          box-shadow: none;
}

/*----------Menu Lateral-------------*/

.nav__main--lateral{
  font-family: 'Nunito Sans', sans-serif;
  position: fixed;
  background-color: var(--tuna);
  display: -webkit-box;
  display: -ms-flexbox;
  display: flex;
  -webkit-box-orient: vertical;
  -webkit-box-direction: normal;
      -ms-flex-direction: column;
          flex-direction: column;
  -webkit-box-pack: center;
      -ms-flex-pack: center;
          justify-content: center;
  -ms-flex-line-pack: start;
      align-content: flex-start;
  /* padding: 1rem 0; */
  height: 100%;
}

.nav__logo--lateral{
  position: relative;
  padding: 1rem;
  bottom: 0.5rem;
  left: 1rem;
}

.full__link {
  position: relative;
  color: var(--white);
  text-decoration: none;
  font-size: 1.5rem;
  font-weight: 600;
  line-height: 50px;
  padding: 4px 2rem;
  -webkit-transition: -webkit-transform 0.3s ease-out;
  transition: -webkit-transform 0.3s ease-out;
  -o-transition: transform 0.3s ease-out;
  transition: transform 0.3s ease-out;
  transition: transform 0.3s ease-out, -webkit-transform 0.3s ease-out;
}

.full__link::after {
  content: "";
  position: absolute;
  height: 50px;
  left: 0;
  width: 100%;
  background: var(--gradient-tree);
  -webkit-transform: scaleY(0);
      -ms-transform: scaleY(0);
          transform: scaleY(0);
  z-index: -1;
  -webkit-transition: -webkit-transform 0.3s ease-in;
  transition: -webkit-transform 0.3s ease-in;
  -o-transition: transform 0.3s ease-in;
  transition: transform 0.3s ease-in;
  transition: transform 0.3s ease-in, -webkit-transform 0.3s ease-in;
}

.full__link:hover::after {
  -webkit-transform: scaleY(1);
      -ms-transform: scaleY(1);
          transform: scaleY(1);
}

.full__menu--ul {
  position: absolute;
  top: 50%;
  left: 50%;
  -webkit-transform: translate(-50%, -50%);
      -ms-transform: translate(-50%, -50%);
          transform: translate(-50%, -50%);
  list-style: none;
  text-align: center;
}

  .nav__footer{
    padding-top: 20%;
    margin: 0%;
    font-family: 'Nunito Sans', sans-serif;
    font-size: 14px;
  }


/*----------PRESENTACIÓN----------*/
.img{
  min-height: 1061px;
  background-image: url(/media/img/computer.jpg);
  background-position: center center;
  background-size: cover;
  z-index: -20;
}

.container {
  width: 100%;
}

.header__container{
  width: 48%;
  background-color: #383c4370;
  margin-right: 20%;
  margin-left: 25.5%;
  padding-top: 20%;  
  padding-left: 1rem;
  text-align: left;
  color: var(--white);
  z-index: 10;
}

.header__title--hola {
  padding-top: 5rem;
}

.header__title {
  font-size: 4rem;
  letter-spacing: 2px;
  font-family: 'Roboto', sans-serif;
}

.header__button{
  font-family: 'Nunito Sans',sans-serif;
  font-weight: 600;
  font-size: 14px;
  line-height: 19px;
  padding: 9px 16px;
  background: var(--silver-sand);
  border-radius: 8px;
}

/*------------------ACERCA----------------- */

/* -----MARGEN PRINCIPAL------*/
.container__acerca,
.container__estudios,
.container__habilidades,
.container__portfolio,
.container__contactos{
  width: 73%;
  /* background-color: #383c4370; */
  /* margin-right: 15%; */
  margin-left: 23.5%;
  padding-left: 1rem;
  padding-right: 1rem;
  text-align: left;
    color: var(--tuna);
    z-index: 10;
  }
.container__acerca{
  margin-bottom: 2rem;
}
/*-------TERMINA MARGEN-------*/
/*---------SUBTÍTULOS---------*/
.subtitle-acerca__color{
  background-color: var(--horizon);
}
.subtitle-body{
  text-align: left;
  margin-left: 2.5rem;
}

.subtitle-acerca{
  font-family: 'Roboto', sans-serif;
  font-weight: 900;
  font-size: xx-large;
  color: var(--white);
  display:inline-block;
  position: relative;
  top: 1rem;
  margin-bottom: 32px;
  padding: 4px;
  z-index: 200;
  border: 4px solid var(--white);
}

.subtitle-acerca::after, .subtitle-acerca::before{
content: '';
position: absolute;
width: 120px;
height: 4px;
background-color: currentColor;
top: 0.8em;
}

.subtitle-acerca::before{
  left: -126px;
}

.subtitle-acerca::after{
  right: -126px;
}
/*--------TEXTO----------*/

.main__container--acerca,
.main__subtitle--estudios,
.main__subtitle--habilidades,
.main__subtitle--acerca{
  margin: 2rem 0;
  font-family: 'Roboto', sans-serif;

}
.main__acerca,
.estudios__article,
.habilidades__article{
  padding-top: 2rem;
  padding-left: 10%;
  line-height: 1.5rem;
}

/* -------------IMÁGENES------------- */

.body__img{
  display: -webkit-box;
  display: -ms-flexbox;
  display: flex;
  -webkit-box-pack: center;
      -ms-flex-pack: center;
          justify-content: center;
  -webkit-box-align: center;
      -ms-flex-align: center;
          align-items: center;
  background: var(--white);
}

.container__img{
  position: relative;
  width: 100%;
  display: -webkit-box;
  display: -ms-flexbox;
  display: flex;
  -webkit-box-pack: center;
      -ms-flex-pack: center;
          justify-content: center;
  -webkit-box-align: center;
      -ms-flex-align: center;
          align-items: center;
  -ms-flex-wrap: wrap;
      flex-wrap: wrap;
  padding: 1rem;
}

.container__img .card{
  position: relative;
  max-width: 300px;
  height: 215px;
  margin: 30px 10px;
  padding: 20px 1rem;
  display: -webkit-box;
  display: -ms-flexbox;
  display: flex;
  -webkit-box-orient: vertical;
  -webkit-box-direction: normal;
      -ms-flex-direction: column;
          flex-direction: column;
  -webkit-box-sizing: 0.5px 202px #383c4370;
          box-sizing: 0.5px 202px #383c4370;
}

.container__img .card .imgBx{
  position: relative;
  width: 260px;
  height: 260px;
}

.container__img .card .imgBx .svg{
  max-width: 100%;
  border-radius: 8px;
}

/*------------------ÍCONOS----------------- */

.main__icon--intereses{
  padding: 2rem 3.5rem;
  display: -webkit-box;
  display: -ms-flexbox;
  display: flex;
  -webkit-box-orient: horizontal;
  -webkit-box-direction: normal;
      -ms-flex-direction: row;
          flex-direction: row;
  -ms-flex-wrap: wrap;
      flex-wrap: wrap;
  -webkit-box-pack: space-evenly;
      -ms-flex-pack: space-evenly;
          justify-content: space-evenly;
}

/*------------------ESTUDIOS----------------- */
.main__container--estudios{
  font-family: 'Nunito Sans', sans-serif;
  margin-bottom: 2rem;
}
.main__container--estudios .estudios__article .estudios__container p{
  font-style: italic ;
}
.main__container--estudios .estudios__article .estudios__container a{
  color: var(--horizon);
  font-style: italic;
}

.estudios__article{
  display: -webkit-box;
  display: -ms-flexbox;
  display: flex;
  -webkit-box-orient: vertical;
  -webkit-box-direction: normal;
      -ms-flex-direction: column;
          flex-direction: column;

}

.estudios__container{
  display: -webkit-box;
  display: -ms-flexbox;
  display: flex;
  -webkit-box-orient: horizontal;
  -webkit-box-direction: normal;
      -ms-flex-direction: row;
          flex-direction: row;
  -webkit-box-pack: justify;
      -ms-flex-pack: justify;
          justify-content: space-between;
  -webkit-box-align: baseline;
      -ms-flex-align: baseline;
          align-items: baseline;
  padding: 12px 8px;
}

.academia,
.innovaccion,
.utn,
.taller,
.skill,
.soft{
  background-color: var(--horizon);
  color: var(--white);
  display: -webkit-box;
  display: -ms-flexbox;
  display: flex;
  padding: 16px 8px;
}

/*------------------HABILIDADES----------------- */

.habilidades__container{
  padding: 1rem 8px;
}

/*----------------- MÉTRICA---------------*/
.metrics{
  font-family: 'Roboto', sans-serif;
  background-color:var(--white);
  margin: 0%;
  padding: 0%;
  display: -webkit-box;
  display: -ms-flexbox;
  display: flex;
  -webkit-box-orient: horizontal;
  -webkit-box-direction: normal;
      -ms-flex-direction: row;
          flex-direction: row;
  -ms-flex-wrap: wrap;
      flex-wrap: wrap;
  -ms-flex-line-pack: center;
      align-content: center;
  color: var(--white);

}

.metrics__container--profesional, .metrics__container--skills{
  margin-top: 3rem;
  width: 380px;
  background: var(--horizon);
  margin: 150px auto;
  padding: 30px;
  border-radius: 10px;
  -webkit-box-shadow: 2 20px 25px var(--tuna);
          box-shadow: 2 20px 25px var(--tuna);
}

@keyframes load{
  from{
    width: 0%;
  }
}
@-webkit-keyframes load{
  from{
    width: 10%;
  }
}

.metrics__sub{
  text-align: center;
  margin-bottom: 10px;
}

.metrics__box{
  list-style: none;
  margin: 0;
  padding: 0;
}

.metrics__text{
  margin-bottom: 10px;
}

.metrics__bar{
  height: 18px;
  background-color: var(--white);
  margin-bottom: 15px;
  border-radius: 15px;
}

.metrics__bar::before{
  content: " ";
  background: var(--gradient-tea);
  display: inline-block;
  padding: 0.6rem;
  border-radius: inherit;
  animation: load 3s 0s; 
  -webkit-animation: load 3s 0s;
  -moz-animation: load 3s 0s;
  -o-animation: load 3s 0s;
}

.metrics__bar.metrics__bar80::before{
  width: calc(80% - 10px);
}
.metrics__bar.metrics__bar70::before{
  width: calc(70% - 10px);
}
.metrics__bar.metrics__bar90::before{
  width: calc(90% - 10px);
}
.metrics__bar.metrics__bar60::before{
  width: calc(60% - 10px);
}
/*-----------------FIN METERS---------------*/


/**/
/*------------------FORMULARIO----------------- */
/**/
.talk {
  font-style: none;
  font-display: hidden;
}

.formulario{
  position: relative;
  display: -webkit-box;
  display: -ms-flexbox;
  display: flex;
  -webkit-box-pack: center;
      -ms-flex-pack: center;
          justify-content: center;
  -webkit-box-align: center;
      -ms-flex-align: center;
          align-items: center;
  min-height: 100vh;
  background: var(--gradient-green);
  padding: 2rem;
  padding-top: 180px;
  margin-left: 17.5%;
  color: var(--woodsmoke);
  -webkit-box-shadow: 0 15px 35px rgba(0, 0, 0, 0.25);
          box-shadow: 0 15px 35px rgba(0, 0, 0, 0.25);
}

.formulario__sub-color{
  background: var(--tuna);
  padding-left: 19rem;
}

.contact__me{
  font-family: 'Roboto', sans-serif;
  text-align: center;
  padding: 2rem;
  background-color: var(--white);
  border-radius: 16px 16px 0 0;

}

.form__container{
  position: relative;
  padding: 50px;
  background: var(--white);
  display: -webkit-box;
  display: -ms-flexbox;
  display: flex;
  -webkit-box-pack: center;
      -ms-flex-pack: center;
          justify-content: center;
  -webkit-box-align: center;
      -ms-flex-align: center;
          align-items: center;
  /* border-radius: 16px; */
  
}

.form__input--box{
  position: relative;
  width: 350px;
  z-index: 20;
}

.form__text{
  position: relative;
  padding: 8px 10px;
  width: 100%;
  border: none;
  outline: none;
  background: transparent;
  color: var(--white);
  font-size: 1.25em;
  letter-spacing: 0.05em;
  z-index: 30;
}

.form__label{
  font-family: 'Roboto', sans-serif;
  position: absolute;
  left: 0;
  padding: 0 1rem;
  pointer-events: none;
  font-size: 1em;
  -webkit-transition: 0.5s;
  -o-transition: 0.5s;
  transition: 0.5s;
  color: var(--woodsmoke);
  letter-spacing: 0.05em;
}

.form__text:valid ~ .form__label,
.form__text:focus ~ .form__label {
  font-size: 0.85em;
  -webkit-transform: translateY(-2rem);
      -ms-transform: translateY(-2rem);
          transform: translateY(-2rem);

}

.form__base{
  position: absolute;
  bottom: 0;
  left: 0%;
  width: 100%;
  height: 0.25rem;
  background: var(--gradient-green);
  -webkit-transition: 0.5s;
  -o-transition: 0.5s;
  transition: 0.5s;
  z-index: 10;
  border-radius: 4px;
  pointer-events: none;
}

.form__text:valid~.form__base,
.form__text:focus~.form__base{
  height: 100%;
  -webkit-box-shadow: inset 1px 1px 10px var(--woodsmoke-025);
          box-shadow: inset 1px 1px 10px var(--woodsmoke-025);
}

.textarea{
  font-family: 'Roboto', sans-serif;
  width: 350px;
  height: 59px;
  padding: 16px;
  outline: none;
  resize: none;
  font-size: 1em;
  /* z-index: 10; */
}

.textarea:is(:focus, :valid){
  border-color: var(--horizon);
}

.textarea:is(:focus, :valid)::-webkit-input-placeholder{
  font-family: 'Roboto', sans-serif;
  color: var(--white);
}

.textarea:is(:focus, :valid)::-moz-placeholder{
  font-family: 'Roboto', sans-serif;
  color: var(--white);
}

.textarea:is(:focus, :valid):-ms-input-placeholder{
  font-family: 'Roboto', sans-serif;
  color: var(--white);
}

.textarea:is(:focus, :valid)::-ms-input-placeholder{
  font-family: 'Roboto', sans-serif;
  color: var(--white);
}

.textarea:is(:focus, :valid)::placeholder{
  font-family: 'Roboto', sans-serif;
  color: var(--white);
}

.textarea::-webkit-scrollbar{
  width: 0;
}

.form__border1{
  border-top: 16px;
}
.form__border2{
  border-radius: 0 0 16px 16px;

}

.form__btn{
  position: relative;
  display: -webkit-box;
  display: -ms-flexbox;
  display: flex;
  -webkit-box-orient: horizontal;
  -webkit-box-direction: normal;
      -ms-flex-direction: row;
          flex-direction: row;
  -webkit-box-pack: center;
      -ms-flex-pack: center;
          justify-content: center;
  -webkit-box-align: center;
      -ms-flex-align: center;
          align-items: center;
  padding: 0.5rem 1rem;
  background: transparent;
}

.form__btn--send{
  cursor: pointer;
  padding: 9px 1rem;
  background: var(--amazon);
  color: var(--white);
  font-family: 'Nunito Sans', sans-serif;
  border: none;
  border-radius: 8px;
  -webkit-box-shadow: 4px 4px 4px rgba(0, 0, 0, 0.5);
          box-shadow: 4px 4px 4px rgba(0, 0, 0, 0.5);
}

.form__btn--send:hover{
  padding: 9px 1rem;
  background: var(--silver-tree);
  border: none;
  border-radius: 8px;
}

.form__btn--send:focus{
  background: var(--silver-tree);
  border: solid 1px var(--tuna);
  -webkit-box-shadow: none;
          box-shadow: none;
}
/**/
/*------------------FORMULARIO----------------- */
/**/



/*-------------------RESPONSIVE CODE START----------------------*/
/* 
@media screen and (max-width: 1250px){
  .full__wrapper ul{
    max-width: 100%;
    padding: 0 20px;
  }

  .full__link{
    margin-left: 30px;
  }

}


@media screen and (max-width: 900px) {
  .full__wrapper{
    display: block;
    position: fixed;
    bottom: red;
    height: 100%;
    width: 100%;
    top: 70px;
    left: 0%;
    margin-left: 0;
    max-width: 350px;

  }
  
} 
*/
/*------------------------------------------------------------*/




```