<template>
	<v-app>
		<v-app-bar app dark class="grey darken-4" height="150" >
			<div class="d-flex align-center">
				<v-img
				alt="Norden Logo"
				class="shrink mr-2"
				contain
				src="https://nordenpet.com.ar/wp-content/uploads/2021/07/logoneg-1024x482.png"
				transition="scale-transition"
				width="150"
				/>
			</div>
			<v-container >
				<v-col cols="12" id="search-bar">
					<v-text-field
						light
						solo
						class="font-italic"
						label="Buscar productos ..."
						clearable="true"
					></v-text-field>  
				</v-col>
				<v-row>
					<ul id="categories">
						<li v-for="categorie in categories" :key="categorie">
						{{ categorie }}
						</li>
					</ul>
				</v-row>
			</v-container>
		</v-app-bar>
	</v-app>
</template>
        
<script>
	export default {
		name: "topbar",
		data: () => ({
			categories: ['OFERTAS','Perro', 'Gato', 'Alimentos Humedos', 'Alimentos terapeuticos', 'Accesorios']
		}),
	};
</script>