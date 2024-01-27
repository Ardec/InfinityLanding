<template>
  <div class="center-container">
    <div class="hero-section">
      <h1 class="hero-header">Zarabiaj jako kierowca taxi we Wrocławiu</h1>
      <p class="hero-text">
        Samochód firmowy <br />
        Pakiet ubezpieczeń <br />
        0 zł na start
      </p>
    </div>
    <div class="slogan">
      <div class="slogan-text">Pensja nawet 7500 zł miesięcznie</div>
    </div>
    <div class="form">
      <div class="form-content">
        <div class="form-header">
          <div class="form-title">Zostań kierowcą</div>
          <div class="form-paragraph">Zacznij zarabiać już za 24 godziny!</div>
          <br>
          <div class="form-phone"><a href="tel:603193888">+48 603 193 888</a></div>
          <div class="form-phone"><a href="tel:669849309">+48 669 849 309</a></div>
          <br>
        </div>
        <a href="tel:+48500300200">
          <div class="form-action">
            <div class="form-button">Zadzwoń</div>
          </div>
        </a>
      </div>
    </div>
    <div class="partners">
      <div class="partners-header">
        <div class="partners-title">Partnerzy</div>
        <div class="partners-paragraph">
          <span class="bold">Infiniti</span>Up jest oficjalnym partnerem największych
          przewozników na Polskim tynku transpowym
        </div>
      </div>
      <div class="partners-body">
        <div class="bolt"></div>
        <div class="uber"></div>
        <div class="free"></div>
      </div>
    </div>
    <div class="points-container">
         <div class="points-section">
         <div class="point-icon"><Icon class="icon" size="36" color="black" name="streamline:insurance-hand" /></div>
      <div class="point-header">Pakiet ubezpieczeń</div>
        <div class="point">Ubezpieczenie zdrowotne</div>
        <div class="point">Ubezpieczenie grupowe</div>
        <div class="point">Ubezpieczenie NNW</div>
    </div>
    <div class="points-section">
      <div class="point-icon"><Icon class="icon" size="36" color="black" name="material-symbols:payments-outline-sharp" /></div>
      <div class="point-header">0 zł opłat</div>
        <div class="point">0 zł za paliwo</div>
        <div class="point">0 zł za samochód</div>
        <div class="point">0 zł za rozliczenie</div>
    </div>
    <div class="points-section">
      <div class="point-icon"><Icon class="icon" size="36" color="black" name="covid:social-distancing-protect-shield-1" /></div>

      <div class="point-header">Pakiet socjalny</div>
        <div class="point">Karta multisport</div>
        <div class="point">Konkursy z nagrodami</div>
    </div>
    <div class="points-section">
        <div class="point-icon"><Icon class="icon" size="36" color="black" name="mdi:help-outline" /></div>
      <div class="point-header">Wsparcie</div>
        <div class="point">Pomoc w uzyskaniu pozwolenia na pracę</div>
        <div class="point">Pomoc z założeniu konta bankowego</div>
        <div class="point">Serwis i Kontakt 24/7</div>
    </div>
    </div>
 

    <div class="contact">
      <div class="partners-header">
        <div class="partners-title">Kontakt</div>
        <div class="partners-paragraph">
          <span class="bold">Infinity</span>Up sp z o.o. z siedzibą we Wrocławiu
        </div>
        <div class="partners-paragraph">53-608 Wrocław</div>
        <div class="partners-paragraph">ul.Robotnicza 40</div>
        <div class="partners-paragraph">NIP 8992935062 </div>
        <div class="partners-paragraph">KRS 0000989396</div>
        <div class="partners-paragraph">
          kontakt.infinityup@gmail.com
        </div>
        <div class="partners-title">
                     <div class=""><a href="tel:603193888">+48 603 193 888</a></div>
        </div>
          <div class="partners-title">
          <div class=""><a href="tel:669849309">+48 669 849 309</a></div>
        </div>
 
      </div>
    </div>
  </div>
</template>

<style lang="scss" scoped>
.point-icon{
  // background-color: $primary;
}
.points-container{
  display:flex;
  flex-direction: row;
  flex-wrap: wrap;
  padding:56px;
  gap:24px;
  justify-content: center;
}
.points-section{
  padding:16px;
  display:flex;
  flex-direction: column;
  color:$primary;
  gap:24px;
  // border:solid $primary 1px;
  // border-radius:12px;

}
.point{
width:300px;
font-size: 20px;
font-style: normal;
font-weight: 400;
line-height: normal; 
}
.point-header{
font-size: 32px;
font-style: normal;
font-weight: 800;
line-height: normal; 
}
.partners-body {
  display: flex;
  padding: 24px 0px;
  flex-direction: column;
  align-items: center;
  gap: 16px;
}
.bolt {
  background: url("/assets/img/boltlogo.png") center / cover no-repeat;
  width: 50px;
  height: 29px;
}
.uber {
  background: url("/assets/img/uberlogo.png") center / cover no-repeat;
  width: 73.864px;
  height: 25px;
}
.free {
  background: url("/assets/img/freelogo.png") center / cover no-repeat;
  width: 163.066px;
  height: 29px;
}
.partners {
  display: flex;
  padding: 24px 16px;
  flex-direction: column;
  align-items: center;
  gap: 10px;
  align-self: stretch;
  border-radius: 12px;
  background: linear-gradient(0deg, rgba(0, 0, 0, 0.5) 0%, rgba(0, 0, 0, 0.8) 100%),
    url("/assets/img/duster.png") center / cover no-repeat;
  color: $text-primary;
}
.contact {
  display: flex;
  padding: 24px 16px;
  flex-direction: column;
  align-items: center;
  gap: 10px;
  align-self: stretch;
  border-radius: 12px;
  background: linear-gradient(0deg, rgba(0, 0, 0, 0.5) 0%, rgba(0, 0, 0, 0.8) 100%),
    url("/assets/img/sky1.png") center / cover no-repeat;
  color: $text-primary;
}
.partners-header {
  width: 100%;
  display: flex;
  flex-direction: column;
  gap: 16px;
}
.partners-title {
  font-size: 32px;
  font-style: normal;
  font-weight: 800;
  line-height: normal;
}
.partners-paragraph {
  font-size: 20px;
  font-style: normal;
  font-weight: 200;
  line-height: normal;
}
.bold {
  font-weight: 700;
}

.form {
  padding: 56px 16px;
  font-family: Inter;
}
.form-action {
  display: flex;
  padding: 16px;
  justify-content: center;
  align-items: center;
  gap: 10px;
  align-self: stretch;
  border-radius: 12px;
  background: $primary;
}
.form-button {
  color: $text-primary;
  text-align: center;
  font-size: 20px;
  font-style: normal;
  font-weight: 800;
  line-height: normal;
}
.form-title {
  color: $primary;
  font-size: 32px;
  font-style: normal;
  font-weight: 800;
  line-height: normal;
}
.form-phone {
  color: $primary;
  font-size: 32px;
  font-style: normal;
  font-weight: 800;
  line-height: normal;
  padding: 8px 0px;
}
.form-paragraph {
  color: $primary;
  font-size: 20px;
  font-style: normal;
  font-weight: 400;
  line-height: normal;
}
.center-container {
  width: 100%;
  color: $text-primary;
}
.slogan {
  display: flex;
  padding: 16px;
  flex-direction: column;
  align-items: left;
  gap: 10px;
  align-self: stretch;
  background: $primary;
}
.slogan-text {
  font-family: Inter;
  font-size: 20px;
  font-style: normal;
  font-weight: 400;
  line-height: normal;
}

.hero-section {
  background: linear-gradient(0deg, rgba(0, 0, 0, 0.5) 0%, rgba(0, 0, 0, 0.5) 100%),
    url("/assets/img/sky1.png") center / cover no-repeat;
  backdrop-filter: blur(50px);
  display: flex;
  width: 100%;
  min-height: 487px;
  padding: 0 16px;
  gap:24px;
  flex-direction: column;
  justify-content: center;
  align-items: flex-start;
  flex-shrink: 0;
}

.hero-header {
  font-family: Inter;
  font-size: 40px;
  font-style: normal;
  font-weight: 800;
  line-height: 2.6rem;
}

.hero-text {
  gap:16px;
  color: $text-primary;
  font-family: Inter;
  font-size: 24px;
  font-weight: 400;
}

@media (min-width: 800px) {
  .hero-section {
    min-height: 800px;
    background-size: cover;
    min-width: 1200px;
    margin-left: auto;
    margin-right: auto;
    width: 100%;
  }
}
</style>
