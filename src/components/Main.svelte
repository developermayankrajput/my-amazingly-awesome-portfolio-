<script>
    import Step from "./Step.svelte";
    let steps = [
        { name: "Upai", icon: "fa-solid fa-comment",link:"https://github.com/mayank0rajput/Chat-Messenger" },
        { name: "Saksham Digital", icon: "fa-solid fa-graduation-cap" ,link:"" },
        { name: "ApplePie", icon: "fa-cloud" },
    ];
    let benefits = [
        {
            name: "a problem solver",
            description:
                "Solved over 50 problems on data strictures and algoritms on various platforms like LeetCode, Hackerrank and Coding Ninjas.",
        },
        {
            name: "self taught programmer",
            description:
                "Learned the skills of LEARNING before Android Development in Kotlin with Firebase Database and REST API.",
        },
        {
            name: "passionate developer",
            description:
                "Loves to create something and work on projects for hours",
        },
    ];
</script>

<main class="flex flex-col flex-1 p-4">
    <section
        id="introPage"
        class="grid grid-cols-1 lg:grid-cols-2 gap-5 py-8 sm:py-14 "
    >
        <div
            class="flex flex-col lg:justify-center text-left lg:ml-5 gap-6 md:gap-8 lg:gap-10"
        >
            <h2 class="font-semibold text-4xl sm:text-5xl md:text-6xl">
                Hi! I'm <span class="poppins text-cyan-400">Mayank</span>
                Rajput <br />Software Engineer
                <span class="poppins text-cyan-400"> Intern</span>
            </h2>
            <p class="text-base sm:text-lg md:text-xl">
                My <span class="text-cyan-400">favorite tech </span> includes Kotlin, Java, Flutter and C++, Firebase, MySQL.
            </p>
            <a
                class="blueShadow mx-auto lg:mr-auto lg:ml-0 text-base sm:text-lg md:text-xl poppins relative overflow-hidden px-6 py-3 group rounded-full bg-white text-slate-950 cursor-pointer"
                href="#getintouch"

            >
                <div
                    class="absolute top-0 right-full w-full h-full bg-cyan-400 opacity-20 group-hover:translate-x-full z-0 duration-200"
                />
                <h4 class="relative z-9">Get in touch &rarr;</h4>
            </a>
        </div>

        <div class="relative grid place-items-center  lg:float-right ">
            <img
                src={"images/pfp.png"}
                alt="Profile Picture"
                class="object-cover z-[2] max-h-[70vh] lg:float-right "
            />
        </div>
    </section>


    <section id="introduction" class="py-20 lg:py-32 flex flex-col gap-24">
        <div class="flex flex-col gap-2 text-center">
            <h4 class="text-sky-300 font-semibold text-3xl sm:text-4xl md:text-5xl">
                Introduction
            </h4><br>
            <h6><p class="text-xl sm:text-lg md:text-xl">
                My name is Mayank Rajput. I am pre final year undergrad student at Oriental Institute of Science & Technology persuing Bachelors in Technology in Information Technology Branch.
            </p> 
            <div class="flex justify-center text-xl sm:text-lg md:text-xl">
                <table class="border border-gray-300 rounded-md shadow-md p-4 m-4">
                  <tr>
                    <td class="font-semibold p-2">Programming Languages:</td>
                    <td>
                      <ul class="flex">
                        <li>C++, Java, Kotlin, Python</li>
                      </ul>
                    </td>
                  </tr>
                  <tr>
                    <td class="font-semibold p-2" >Database:</td>
                    <td>
                      <ul class="flex">
                        <li>SQLite (default Android database),MySQL,PostgreSQL</li>
                      </ul>
                    </td>
                  </tr>
                  <tr>
                    <td class="font-semibold p-2">Cloud Services:</td>
                    <td>
                      <ul class="flex">
                        <li>Firebase Cloud (Realtime Database, Firestore, Cloud Functions, etc.)</li>
                      </ul>
                    </td>
                  </tr>
                  <tr>
                    <td class="font-semibold p-2">Skills:</td>
                    <td>
                      <ul class="flex">
                        <li>Data Structures, Object Oriented Programming , Android Development </li>
                      </ul>
                    </td>
                  </tr>
                </table>
              </div>
            </h6>
        </div>
    </section>

    <section id="projects" class="py-20 lg:py-32 flex flex-col gap-24">
        <div class="flex flex-col gap-2 text-center">
            <h6 class="text-lg sm:text-xl md:text-2xl">
                A few of my creative endeavors.
            </h6>
            <h3 class="font-semibold text-3xl sm:text-4xl md:text-5xl">
                Curious to <span class="poppins text-cyan-400">see</span> my work?
            </h3>
        </div>
        <a
            href="https://gsap.com/docs/v3/Installation/guides/Club%20GSAP%20&%20Vercel"
            target="_blank"
            class="mx-auto px-4 py-2 rounded-md border-solid border-white flex items-center gap-2 -mb-4 sm:-mb-0 -mt-10 duration-200"
        >
            <i class="fa-regular fa-circle-play" />
            <p>Watch the video</p>
        </a>
        <div class="grid grid-cols-1 lg:grid-cols-3 gap-12 lg:gap-10 ">
            <Step step={steps[0]}>
                <p>
                    This project is an <strong
                    class="text-cyan-400"> AI-ChatBot Android App </strong> which on trained on custom data and GPT AI Model . It used <strong
                    class="text-cyan-400">Firebase Cloud</strong>, MeetCody.ai , REST APIs and Kotlin. 
                </p>
                <img src={"/images/upai.png"} />
            </Step>
            <Step step={steps[1]}>
                <p>An <strong
                    class="text-cyan-400"> E-Learn Android App </strong> which provided students recorded lectures to study remotely. This application used FireBase Cloud Database and <strong
                        class="text-cyan-400">Youtube API</strong
                    > to play videos.
                </p>
                <img src={"/images/saksham.png"} />
            </Step>
            <Step step={steps[2]}>
                <p>
                    ApplePie is an E-Commerce Android App which which is used to order grocery.  We will use <strong class="text-cyan-400"> Apache Kafka , WebRTC </strong
                    >and Kotlin here. This project is currently under development.
                </p>
            </Step>
        </div>
    </section>
    <section
        id="about"
        class="py-20 pt-10 lg:pt-16 lg:py-32 flex flex-col gap-16 sm:gap-20 md:gap-24 relative"
    >
        <div
            class="flex flex-col gap-2 text-center relative before:absolute before:top-0 before:left-0 before:w-2/3 before:h-1.5 before:bg-stone-500 after:absolute after:bottom-0 after:right-0 after:w-2/3 after:h-1.5 after:bg-stone-500 py-4"
        >
            <h6 class="text-lg sm:text-xl md:text-2xl">Want to know more?</h6>
            <h3 class="font-semibold text-3xl sm:text-4xl md:text-5xl">
                A bit <span class="poppins text-cyan-400">about</span>
            </h3>
        </div>
        <p class="mx-auto poppins font-semibold text-lg sm:text-xl md:text-2xl">
            I am . . .
        </p>
        <div class="flex flex-col gap-20 w-full mx-auto max-w-[800px]">
            {#each benefits as benefit, index}
                <div class="flex gap-6 sm:gap-8">
                    <p
                        class="poppins text-4xl sm:text-5xl md:text-6xl text-zinc-500 font-semibold"
                    >
                        0{index + 1}
                    </p>
                    <div class="flex flex-col gap-6 sm:gap-8">
                        <h3 class="text-2xl sm:text-3xl md:text-5xl">
                            {benefit.name}
                        </h3>
                        <p>{benefit.description}</p>
                    </div>
                </div>
            {/each}
        </div>
    </section>
</main>
