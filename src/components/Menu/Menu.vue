<template>
    <div class="menu">
    <button class="field_button" @click.stop="download">Сохранить</button>
    </div>
</template>

<script>
import style from "./menu.css";
import XML from "xml";


export default {
  data() {
    return {};
  },
  
  methods: {
    download: function() {
      // var example4 = [
      //   {
      //     toys: [
      //       { _attr: { decade: "80s", locale: "US" } },
      //       { toy: "Transformers" },
      //       { toy: "GI Joe" },
      //       { toy: "He-man" }
      //     ]
      //   }
      // ];
      // let xmlData = XML(example4, { indent: true, declaration: true });

      // let link = document.createElement("a");
      // let blob = new Blob([xmlData], { type: "text/plain" });
      // link.href = window.URL.createObjectURL(blob);
      // link.download = "test.txt";
      // link.click();

      this.$emit("save");
    },


  }
};
</script>
