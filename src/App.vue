<template>
  <!-- component -->
  <!-- This is an example component -->
  <div class="max-w-7xl mx-auto flex flex-col relative">

    <nav class="max-w-7xl px-5 md:fixed top-0 z-[98] w-screen backdrop-blur-md bg-[#121212] bg-opacity-80">
      <div class="container mx-auto flex flex-wrap items-center justify-between">
        <button @click="redirectToHome" class="flex">
          <span class="self-center text-lg text-[#ffdb70] font-semibold whitespace-nowrap fadein-bot hover:text-amber-100">0_0mairy</span>
        </button>
        <div class="flex md:order-2 fadein-bot space-x-4">
          <a href="https://github.com/Mar1yam" target="_blank" rel="noopener noreferrer"><img class="w-9 rounded-full" src="https://seeklogo.com/images/G/github-logo-2E3852456C-seeklogo.com.png" alt="github"></a>
          <a href="https://www.linkedin.com/in/mariyam-m-3989a4224/" target="_blank" rel="noopener noreferrer"><img class="w-9 rounded-full" src="https://img.icons8.com/?size=100&id=447&format=png&color=FFFFFF" alt="linkdin"></a>
          <a href="https://doc-00-38-prod-02-apps-viewer.googleusercontent.com/viewer2/prod-02/pdf/hhta9ep5svcqecccbrhrm1e1jubdnure/e57opcm7e5lotvno0dp0r72pg2pq2eej/1725061725000/3/100614821988288310807/APznzaZ7jNCkOchPInlJLAUs4_RCom5d_b3rOMB-t8uc7YYlyKrCzxQ8dHXgRe-pXVVQZ3GAN0XOSiCZVHx-yLP8nN6g2TANCZEZaVYA0iErEs0SR8vH6JCM7JaJjbpaHuGvtmoiF5RmywgvkuntF1ZmJf8SKh8ZFXMplY0LBMJBfhmSk8aQidyak9zPfc5TvWAcFjjnGRm9B1IOBtKEVKCj6b5U-UY8KzfiMI-ojMRH89CMGP2aYPcbsMQMhIZ7T_e-72sHldOEployOpVTAJlRUipMBI5ANLxWsdniGr7SAJrZaAumW1k-kAwheLNFpOigARO5wbeDsv4jLW61JJi14Us6YGsdmo4msU4IyW2_K-0mrcZxTu3pr9J9Ho2zetd34M-2d1e_o8AbjAq6KzA3f_KIzUkYHQ==?authuser=0&nonce=0sfqu2okjbv0e&user=100614821988288310807&hash=9ibu61uj0ge5v7kt6cjgbdc0ueht040v" target="_blank" rel="noopener noreferrer"><img class="w-9 rounded-full" src="https://img.icons8.com/?size=100&id=121320&format=png&color=FFFFFF" alt="Resume"></a>
        </div>
        <div class="hidden md:flex justify-between items-center w-full md:w-auto md:order-1" id="mobile-menu-3">
          <ul class="flex-col md:flex-row flex md:space-x-8 mt-4 md:mt-0 md:text-sm md:font-medium">
            <li>
              <router-link to="/"
                class="fadein-bot text-gray-700 hover:bg-gray-50 border-b border-gray-100 md:hover:bg-transparent md:border-0 block pl-3 pr-4 py-2 md:hover:text-gray-500 md:p-0"
                aria-current="page">Home</router-link>
            </li>
            <li>
              <router-link to="/about"
                class="fadein-bot fadein-1 text-gray-700 hover:bg-gray-50 border-b border-gray-100 md:hover:bg-transparent md:border-0 block pl-3 pr-4 py-2 md:hover:text-gray-500 md:p-0">About</router-link>
            </li>
            <li>
              <router-link to="/project"
                class="fadein-bot fadein-2 text-gray-700 hover:bg-gray-50 border-b border-gray-100 md:hover:bg-transparent md:border-0 block pl-3 pr-4 py-2 md:hover:text-gray-500 md:p-0">Projects</router-link>
            </li>
            <li>
              <router-link to="/contact"
                class="fadein-bot fadein-3 text-gray-700 hover:bg-gray-50 border-b border-gray-100 md:hover:bg-transparent md:border-0 block pl-3 pr-4 py-2 md:hover:text-gray-500 md:p-0 blog">Contact</router-link>
            </li>
          </ul>
        </div>
      </div>
    </nav>

    <div class="md:mt-[100px]">
      <router-view />
    </div>
  </div>
  <footer class="block md:hidden fixed bottom-0 left-0 right-0 rounded-t-3xl border border-[#383838] bg-[#121212] bg-opacity-80 backdrop-blur-md backdrop-opacity-90">
  <nav class="flex justify-around py-4 text-xs">
    <router-link to="/" class="text-gray-300 hover:text-white">Home</router-link>
    <router-link to="/about" class="text-gray-300 hover:text-white">About</router-link>
    <router-link to="/project" class="text-gray-300 hover:text-white">Projects</router-link>
    <router-link to="/contact" class="text-gray-300 hover:text-white">Contact</router-link>
  </nav>
</footer>
</template>

<script>
export default {
  methods: {
    redirectToHome() {
      this.$router.push('/')
    }
  },
}
</script>

<style>
*,
*::before,
*::after {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}

::-webkit-scrollbar {
  width: 5px; /* for vertical scrollbar */
  height: 5px; /* for horizontal scrollbar */
}

::-webkit-scrollbar-track {
  background: hsl(240, 1%, 17%);
  border-radius: 5px;
}

::-webkit-scrollbar-thumb {
  background: #ffdb70;
  border-radius: 5px;
}

::-webkit-scrollbar-button { width: 20px; }

body {
  font-family: 'Poppins', sans-serif;
  background: hsl(0, 0%, 7%);
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  height: 100vh;
}

nav {
  padding: 30px;
}

nav a {
  font-weight: bold;
  color: #2c3e50;
  transition: color 0.3s;
}

nav a.router-link-exact-active {
  display: inline-flex;
  flex-direction: column;
  color: white;
  transition: color 0.3s;
}

nav a.router-link-exact-active::after {
  display: inline-block;
  content: "";
  margin-top: 0.08em;
  width: 100%;
  height: 4px;
  border-radius: 2px;
  background-color: #ffdb70;
}

nav a.router-link-exact-active:hover {
  color: white;
}


@keyframes fadeInLeft {
  0% {
    opacity: 0;
    transform: translateX(-100%);
  }
  100% {
    opacity: 1;
    transform: translateX(0);
  }
}

</style>
