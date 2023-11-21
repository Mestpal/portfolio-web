<script>
	import Step from "./Step.svelte";

    let steps = [
        {name: 'project 1', icon: 'fa-solid fa-list-check'},
        {name: 'project 2', icon: 'fa-solid fa-list-check'},
        {name: 'project 3', icon: 'fa-solid fa-list-check'},
    ]
</script>

<main class="flex flex-col flex-1 p-4">
    <section 
        id="introPage"
        class="grid grid-cols-1 lg:grid-cols-2 gap-10 py-8 sm:py-14"
    >
        <div class="flex flex-col lg:justify-center text-center lg:text-left gap-6 md:gap-8 lg:gap-18">
            <h2 class="font-semibold text-4xl sm:text-5xl md:text-6xl">
                Hi! I'm <span class="text-violet-400">Manuel</span> Estevez Palencia<br>
                A Full Stak <span class="poppins text-violet-400">Developer</span>
            </h2>
            <p class="text-base sm:text-lg md:text-xl">
                My favourite technologies stock includes: JavaScript, frameworks like VUE or Nuxt, <br>
                component libraries like Vuetify, or style librarieslike Bulma
            </p>
            <a 
                class="blue-shadow mx-auto lg:mr-auto text-base sm:text-lg md:text-xl poppins 
                relative overflow-hidden px-4 py-3 group rounded-full bg-white text-slate-950
                cursor-pointer"
                href="#"
                target="_blank" 
            >
                <div 
                    class="absolute top-0 right-full w-full h-full bg-violet-400 opacity-20 group-hover:translate-x-full z-0 duration-200"
                />
                <h4 class="relative z-9">Get in touch &rArr;</h4>
            </a>
        </div>
        <div class="relative shadow-2xl grid place-item center">
            <img
                src={"images/profile.jpg"}
                alt="Profile Image"
                class="object-cover z-[2] max-h-[70vh]"
            >
        </div>
    </section>

    <section id="projects" class="py-20 lg:py-32 flex flex-col gap-24">
        <div class="flex flex-col gap-24 text-center">
            <h6 class="text-lg sm:text-xl md:text-2xl">
                Some of my recent projects
            </h6>
            <h3 class="font-semibolt text-3xl sm:text-4xl md:text-5xl">
                Are you curious to <span class="poppins text-violet-400">see</span> my work?
            </h3>
            <a href="https://youtube.com/shorts/EZkiplhQiMs?feature=shared"
            target="_blank" class="mx-auto px-4 py-2 rounded-md border border-solid border-white 
            flex items-center gap-2 -mb-4 sm:-mb-0 -mt-10 hover:border-violet-700 duration-200"
            >
                <i class="fa-regular fa-circle-play"></i>
                <p>Watch the video</p>
            </a>
            <div class="grid grid-cols-1 lg:grid-cols-3 gap-12 lg:gap-10">
                <Step step={steps[0]}>
                    Project Description 1
                </Step>
                <Step step={steps[1]}>
                    Project Description 2
                </Step>
                <Step step={steps[2]}>
                    Project Description 3
                </Step>                                
            </div>
        </div>
    </section>

    <section id="about">

    </section>
</main>