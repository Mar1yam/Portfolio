<script>
export default {
  data() {
    return {
      activeTab: 1,
      items: [
        {
          id: 1,
          name: 'Personal Portfolio',
          imageUrl: 'https://i.imgur.com/0238VSz.png',
          status: 'My personal website, I created this website to display my profile, skills and projects.',
          tech: 'VueJS 3, Tailwind, Bootstrap, npm, HTML, CSS, JavaScript',
          github: '',
          demo: ''
        },
        {
          id: 2,
          name: 'Animated Flower',
          imageUrl: 'https://i.imgur.com/G0X0zSS.png',
          status: 'Created this project on an animated flower inspired by a viral TikTok trend, created using HTML, CSS, JavaScript, Node.js, and Nodemon!',
          tech: 'Node.JS, Nodemon, HTML, CSS, JavaScript',
          github: 'https://github.com/Mar1yam/flower-animation?tab=readme-ov-file',
          demo: 'https://flower-animation.onrender.com/'
        },
        {
          id: 3,
          name: 'Flappy Bird',
          imageUrl: 'https://i.imgur.com/c6FAacH.png',
          status: 'Created a Flappy Bird game using Unity and C#, featuring scoring, high scores, and cloud integration for enhanced gameplay.',
          tech: 'Unity, C#',
          github: 'https://github.com/Mar1yam/Flappy-Bird',
          demo: 'null'
        },
        {
          id: 4,
          name: 'To-Do-List Website',
          imageUrl: 'https://i.imgur.com/WE752Mf.png',
          status: 'A dynamic to-do list website that lets users manage tasks with features like authentication, real-time updates, and responsive design using HTML, CSS, JavaScript, Angular, and Node.js.',
          tech: 'Node.JS, Bootstap, Angular, HTML, CSS, JavaScript',
          github: 'null',
          demo: 'null'
        },
        {
          id: 5,
          name: 'EV Charging Station',
          imageUrl: 'https://i.imgur.com/9S2tY5i.png',
          status: 'The EV Charging Station Route Optimization app enhances convenience by analyzing distances and recommending efficient routes within a 23-node network.',
          tech: 'Python, NetworkX',
          github: 'https://github.com/Sabrina-OT/AlgorithmsFinal',
          demo: 'null'
        },
        {
          id: 6,
          name: 'Encryption Game',
          imageUrl: 'https://i.imgur.com/BnGK1bs.png',
          status: 'Created an encryption game using Python implementing OOP principles with various algorithms including Substitution, Playfair, Caesar, Transposition, Product, and RSA ciphers.',
          tech: 'Python, OOP',
          github: 'null',
          demo: 'null'
        },
        {
          id: 7,
          name: 'Case Study | INFR 1421U',
          imageUrl: 'https://media.licdn.com/dms/image/v2/D562DAQFNDJDJCyq14w/profile-treasury-image-shrink_800_800/profile-treasury-image-shrink_800_800/0/1690758696124?e=1725411600&v=beta&t=eE4EZF_kS86f5ggmJV0t8UT_8eVOot4uf-_NbpH8MKM',
          status: 'Designed and implemented a pilot network for CryptoMine using Cisco Packet Tracer, connecting branches across North America with BGP, OSPF, and VLANs. Showcased skills in network configuration, secure remote access, and inter-VLAN routing.',
          tech: 'Cisco Packet Tracer',
          github: 'null',
          demo: 'null'
        },
        {
          id: 8,
          name: 'Case Study | INFR 2421U',
          imageUrl: 'https://media.licdn.com/dms/image/v2/D4E2DAQHJOo7xHYw2tg/profile-treasury-image-shrink_800_800/profile-treasury-image-shrink_800_800/0/1719367279945?e=1725411600&v=beta&t=YiFkzxuBsuWiXaLTUIvYQ54koLKx4FksC3s3wT1MU1w',
          status: 'Designed and deployed LAN and WAN infrastructure for Ontario Tech University, using MPLS, DMVPN, VLANs, and HSRP for resilience and secure connectivity.',
          tech: 'TCL scripting, Traceroute, SecureCRT',
          github: 'null',
          demo: 'null'
        },
      ]
    };
  }
}
</script>
<template>
  <div class="px-5 py-5 md:px-12 md:py-10 text-left text-amber-50 mx-3">
    <article data-page="about">
      <header>
        <div
          class="text-2xl font-bold text-white mb-10 fadein-bot title-section flex items-center justify-center flex-col">
          <!-- <div class="h-[1px] w-10 bg-amber-200 md:w-20 aos-init aos-animate"></div> -->
          <h4>Past Project Experience</h4>
          <h4 class="text-base font-normal text-transparent bg-clip-text bg-gradient-to-r from-slate-100 to-amber-300">
            Explore the projects I've worked on so far</h4>
        </div>
      </header>
      <section>
        <div>
          <div class="grid grid-cols-1 gap-4 pb-32 md:grid-cols-3 md:gap-3 xl:grid-cols-3 xl:gap-3 2xl:gap-5 fade-zoom-in">
            <div v-for="item in items" :key="item.id">
              <div
                class="item-card flex flex-col items-center gap-2 rounded bg-[#1e1e1f] hover:bg-[#282828] border border-[#383838] rounded-xl text-amber-50 md:gap-3 px-5 py-5 lg:px-5 ">
                <div class="flex h-12 w-12 items-center justify-center p-0 h-full w-full lg:p-0 zoom-in">
                  <img alt="HTML" loading="lazy" decoding="async" data-nimg="1" class="drop-shadow-xl rounded rounded-xl"
                    :src="item.imageUrl">
                </div>
                <div class="w-full flex flex-col gap-2 items-center text-sm md:text-base lg:text-lg">
                  <div class="title-text font-medium text-secondary">{{ item.name }}
                  </div>
                  <div class="w-full text-left text-[10px] text-[#c1c1c1] md:text-xs lg:text-sm">
                    {{ item.status }}</div>
                  <div class="w-full mt-4 text-normal text-sm text-left text-amber-200">
                    {{ item.tech }}
                  </div>
                  <div class="w-full flex justify-end">
                    <div class="flex cursor-pointer items-end gap-2 text-primary">
                      <a v-if="item.github !== 'null'"
                        :href="item.github" target="_blank" rel="noreferrer"
                        title="View github repository" class="transition-all hover:text-accent">
                        <svg stroke="currentColor"
                          fill="none" stroke-width="2" viewBox="0 0 24 24" stroke-linecap="round" stroke-linejoin="round"
                          height="16" width="16" xmlns="http://www.w3.org/2000/svg">
                          <path
                            d="M9 19c-5 1.5-5-2.5-7-3m14 6v-3.87a3.37 3.37 0 0 0-.94-2.61c3.14-.35 6.44-1.54 6.44-7A5.44 5.44 0 0 0 20 4.77 5.07 5.07 0 0 0 19.91 1S18.73.65 16 2.48a13.38 13.38 0 0 0-7 0C6.27.65 5.09 1 5.09 1A5.07 5.07 0 0 0 5 4.77a5.44 5.44 0 0 0-1.5 3.78c0 5.42 3.3 6.61 6.44 7A3.37 3.37 0 0 0 9 18.13V22">
                          </path>
                        </svg></a>
                        <a v-if="item.demo !== 'null'" :href="item.demo" target="_blank" rel="noreferrer"
                        title="View finished project" class="transition-all hover:text-accent">
                        <svg stroke="currentColor"
                          fill="none" stroke-width="2" viewBox="0 0 24 24" stroke-linecap="round" stroke-linejoin="round"
                          height="18" width="18" xmlns="http://www.w3.org/2000/svg">
                          <path d="M18 13v6a2 2 0 0 1-2 2H5a2 2 0 0 1-2-2V8a2 2 0 0 1 2-2h6"></path>
                          <polyline points="15 3 21 3 21 9"></polyline>
                        <line x1="10" y1="14" x2="21" y2="3"></line>
                      </svg></a></div>
                </div>
              </div>
            </div>
          </div>
        </div>
      </div>
    </section>
  </article>
</div></template>

<style>
.item-card:hover {
  transition: transform 0.3s ease;
  transform: translateY(-8px);
}
svg:hover{
  stroke: #ffdb70;
}
@keyframes fadeZoomIn {
  0% {
    opacity: 0;
    transform: scale(0.5);
  }
  100% {
    opacity: 1;
    transform: scale(1);
  }
}

/* Menggunakan animasi pada elemen yang diinginkan */
.fade-zoom-in {
  animation: fadeZoomIn 1s ease-in-out;
}
</style>