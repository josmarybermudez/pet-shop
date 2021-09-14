<template>
	<v-app>
		<topbar></topbar>
	</v-app>
</template>

<script>
import "./styles/main.scss";
import topbar from "./components/topbar";

export default {
  name: "App",

  data: () => ({
    //
  }),
  components: {
    topbar,
  },
};

</script>
