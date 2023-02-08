<template>
  <div class="select mr-4 ml-6">
    <div class="inner">
    <div></div>
      <select id="languages" name="languages">
        <option value="en">English</option>
        <option value="af">Afrikaans</option>
        <option value="ar">Arabic</option>
        <option value="ast">Asturian</option>
        <option value="ca">Catalan</option>
        <option value="zh">Chinese</option>
        <option value="zh-CN">Chinese</option>
        <option value="da">Danish</option>
        <option value="nl">Dutch</option>
        <option value="en-GB">English (UK)</option>
        <option value="en-US">English (US)</option>
        <option value="eo">Esperanto</option>
        <option value="fr">French</option>
        <option value="de-DE">German</option>
        <option value="ha">Hausa</option>
        <option value="it">Italian</option>
        <option value="ja">Japanese</option>
        <option value="la">Latin</option>
        <option value="pt">Portuguese</option>
        <option value="es">Spanish</option>
        <option value="sw">Swahili</option>
        <option value="yo">Yoruba</option>
      </select>
      <v-icon start color="#3E96ED" size="large" icon="mdi-menu-down"></v-icon>
    </div>
  </div>
</template>

<style scoped>
select {
  appearance: none;
  background-color: transparent;
  border: none;
  margin: 0;
  font-family: inherit;
  font-size: inherit;
  cursor: inherit;
  line-height: inherit;
  z-index: 1;
  position: absolute;
  width: 100%;
  height: 100%;
  padding: 10px 32px 10px 10px;
  top: 0;
  left: 0;
}

select::-ms-expand {
  display: none;
}

select:focus {
  outline: none;
  border: 2px solid #3E96ED;
  border-radius: inherit;
}

.select {
  max-width: 120px;
  display: flex;
  align-items: center;
  margin: 0;
  padding: 0;
}

.inner {
  width: 120px;
  position: relative;
  border: 1px solid rgb(242, 242, 242, 0.2);
  border-radius: 10px;
  font-size: 1.05rem;
  cursor: pointer;
  line-height: 1;
  background-color: rgb(0, 0, 0, 0.05);
  display: flex;
  align-items: center;
  justify-content: space-between;
  padding: 10px 6px;
}
option{
  background-color: rgb(0, 0, 0, 0.05);
  color: #000;
}
</style>