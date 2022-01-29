<template>
	<div id="nav">
		<router-link to="/">Dashboard</router-link> |
		<router-link to="/about">About</router-link>
	</div>
	<router-view />
</template>

<style lang="scss">
@import url("https://rsms.me/inter/inter.css");

:root {
	--primary: rgb(62, 123, 250);
	--background: rgb(28, 28, 40);
	--light-background: rgb(40, 41, 61);
}

* {
	margin: 0;
	padding: 0;
	border: 0;
}

#app {
	font-family: Avenir, Helvetica, Arial, sans-serif;
	-webkit-font-smoothing: antialiased;
	-moz-osx-font-smoothing: grayscale;

	height: 100vh;
	background-color: var(--background);

	font-family: "Inter";
	text-align: center;
	color: white;
}

h2 {
	padding-left: 1em;
	border-left: 3px solid var(--primary);
}

.box {
	display: flex;
	flex-direction: column;

	padding: 5px;
	margin: 10px;

	background-color: var(--light-background);

	border-radius: 15px;

	opacity: 0;
	animation: drop 1s ease forwards;
	animation-delay: calc(var(--order) * 200ms);
}

.title {
	color: #8f90a6;
}

.code {
	font-family: "Consolas", "Courier New", Courier, monospace;
}

.bar {
	display: flex;
	justify-content: space-between;
	align-items: center;

	padding: 10px;

	.right {
		display: flex;
		justify-content: flex-end;
	}
}

.group {
	display: flex;
	padding: 10px;
	p {
		padding: 5px;
	}
}

@keyframes drop {
	from {
		opacity: 0;
		transform: translateX(-5%);
	}
	to {
		opacity: 1;
		transform: translateX(0);
	}
}

// #nav {
// 	padding: 30px;

// 	a {
// 		font-weight: bold;
// 		color: #2c3e50;

// 		&.router-link-exact-active {
// 			color: #42b983;
// 		}
// 	}
// }
</style>
