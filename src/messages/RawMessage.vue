<template>
  <div class="sc-message--file">
    <div class="sc-message--file-text">
      <p><span v-html="data.text"></span></p>
    </div>
  </div>
</template>

<script>
export default {
  props: {
    data: {
      type: Object,
      required: true
    }
  }
}
</script>

<style scoped>
.sc-message--file {
  border-radius: 6px;
  font-weight: 300;
  font-size: 14px;
  line-height: 1.4;
  /* white-space: pre-wrap; */
  -webkit-font-smoothing: subpixel-antialiased;
}
.sc-message--content.sent .sc-message--file {
  word-wrap: break-word;
}
.sc-message--file-icon {
  text-align: center;
  margin-left: auto;
  margin-right: auto;
  margin-top: 15px;
  margin-bottom: 0px;
}
.sc-image {
  max-width: 100%;
  min-width: 100%;
}
.sc-message--file-text {
  padding: 10px 10px;
  border-radius: 6px;
  font-weight: 300;
  font-size: 14px;
  line-height: 1.4;
  white-space: pre-wrap;
  -webkit-font-smoothing: subpixel-antialiased;
}
.sc-message--file-name {
  color: white;
  padding-left: 15px;
  padding-right: 15px;
  padding-top: 0;
  font-size: x-small;
  text-align: center;
}
.sc-message--file-name a {
  text-decoration: none;
  color: #ece7e7;
}
.sc-message--file-name a:hover {
  color: white;
}
.sc-message--content.sent .sc-message--file-text {
  color: white;
  background-color: #365ca7;
  word-wrap: break-word;
}
.sc-message--content.received .sc-message--file {
  color: #365ca7;
  background-color: white;
  margin-right: 10px;
}
.sc-message--content.received .sc-message--file-name {
  color: #000;
}
.sc-message--content.received .sc-message--file a {
  color: rgba(43, 40, 40, 0.7);
}
.sc-message--content.received .sc-message--file a:hover {
  color: #0c0c0c;
}
</style>