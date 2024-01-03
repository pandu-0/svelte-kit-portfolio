<script>
    import Step from "./Step.svelte";

let steps = [
    {
        name: "131 Mini Project!",
        // Icons are from https://fontawesome.com/
        icon: "fa-solid fa-terminal fa-beat",
        description:
            "INSERT",
        href: "https://github.com/pandu-0/cs131/tree/master/a5#a5-project-cs131",
    },
    {
        name: "Damaged Car Parts Recognition ML model",
        icon: "fa-solid fa-car-burst fa-shake",
        description:
            "INSERT1",
        href: "https://github.com/pandu-0/Damaged-Car-Parts-Recognition-ML-Model",
    },
    {
        name: "Temp2",
        icon: "fa-solid fa-question fa-spin",
        description:
            "INSERT2",
        href: "#",
        
    },
];

    let benefits = [
        {
            metric: "10x",
            name: "a self taught programmer",
            description:
                "Blank :((",
        },
        {
            name: "a Machine Learning enthusiast",
            description:
                "Blank :((",
        },
        {
            name: "an excellent communicator",
            description:
                "Blank :((",
        },
    ];
</script>

<main class="flex flex-col flex-1 p-4">
    <meta charset="UTF-8"/>
    <section
        id="introPage"
        class="grid grid-cols-1 lg:grid-cols-2 gap-10 py-8 sm:py-14"
    >
        <div
            class="flex flex-col lg:justify-center 
            text-center lg:text-left gap-6 md:gap-8 lg:gap-10"
        >
             <!-- Introduction text -->
            <h2 class="font-semibold text-2xl sm:text-5xl md:text-6xl">
                Hey! I'm <span class="poppins text-violet-400">Manmohanbabu</span> Rupanagudi 
                <br/> Majoring in <span class="poppins text-violet-400">Data Science </span> at SJSU
           
            </h2>

            <!-- Introduction subtext -->
            <p class="text-base sm:text-lg md:text-xl">
                I love <span class="text-violet-400"> Statistics</span> and 
                concepts in <span class="text-violet-400"> Machine Learning</span>.
                Specifically, I'm great at Java, command-line programming and Math!
            </p>

            <!-- GitHub Link -->
            <a class="blueShadow mx-auto lg:mr-auto text-base 
            sm:text-lg md:text-xl poppins relative overflow-hidden px-6 py-3 group 
            rounded-full bg-white text-slate-950 cursor-pointer"
            href="https://github.com/pandu-0"
            target = "_blank">
                <div
                class="absolute top-0 right-full w-full h-full bg-violet-400 
                opacity-20 group-hover:translate-x-full z-0 duration-200"
                />

                <!-- padding is top, right, bottom, left directions.
                    But you can just use 1 number to fill them all -->
                <h4 style="padding: 3px;" class="relative z-9">
                    <span>See my GitHub!</span>
                    <i class="fa-brands fa-github fa-2xl fa-fade"></i>
                </h4>
            </a>
            
            
        </div>

        <!-- Profile image -->
        <div id="pandu" class="relative shadow-2xl grid place-items-center">
            <img
                src={"images/profile.png"}
                alt="Pandu"
                class="object-cover z-[2] max-h-[70vh]"
            />
        </div>
    </section>
    
    <!-- Steps That contain project description -->
    <section class="py-20 lg:py-32 flex flex-col gap-24" id="projects">
        <div class="flex flex-col gap-2 text-center">
            <h6 class="text-large sm:text-xl md:text-2xl">
                My <span class="poppins text-violet-400">Coding</span> Odyssey.
            </h6>
            <h3 class="font-semibold text-3xl sm:text-4xl md:text-5xl">
                Curious to <span class="poppins text-violet-400">see</span> my work?
            </h3>
        </div>

        <!-- Video Button and Link -->
        <!-- <a
            href="https://www.youtube.com/watch?v=wh9QLjk3M2k"
            target="_blank"
            class="mx-auto px-4 py-2 rounded-md border border-solid border-white flex items-center gap-2 -mb-4 sm:-mb-0 -mt-10 hover:border-violet-700 duration-200"
        >
            <i class="fa-regular fa-circle-play" />
            <p>Watch the video</p>
        </a> -->

        <!-- PROJECT DETAILS -->
        <div class="grid grid-cols-1 lg:grid-cols-3 gap-12 lg:gap-10">

            <!-- PROJECT 1 -->
            <Step step={steps[0]}>
                <p>
                    A mini project in my CS131 class where I 
                    <strong class="text-violet-400"> 
                        analyzed
                    </strong> a 2023 anime dataset
                    to see if I can find any interesting
                    <strong class="text-violet-400">
                        insights.
                    </strong> 
                    The project includes statistical information calculated 
                    from command line (awk/sed) and 
                    graphs plotted using
                    <strong class="text-violet-400">gnuplot</strong>.
                </p>
            </Step>

            <!-- PROJECT 2 -->
            <Step step={steps[1]}>
                <p>
                    A custom <strong class="text-violet-400">ML model</strong> I created that automatically 
                    <strong class="text-violet-400">recognizes damaged car parts</strong> given a 
                    image of the damaged car. The model was made using 
                    <strong class="text-violet-400">Google Cloud Platform's Vertex AI AutoML Vision</strong>. 
                    This model is capable of <strong class="text-violet-400">classifying</strong> damaged parts 
                    into Bumper, Engine compartment, Hood, Lateral & Windshield 
                    with 73% precision and 50% recall.
                </p>
            </Step>

            <!-- PROJECT 3 -->
            <Step step={steps[2]}>
                <p>
                    BLANK :((
                </p>
            </Step>
        </div>
    </section>
    
    <section
        id="about"
        class="py-20 pt-10 lg:pt-16 lg:py-32 flex flex-col gap-16 sm:gap-20 md:gap-24 relative"
    >
        <div
            class="flex flex-col gap-2 text-center relative 
            before:absolute before:top-0 before:left-0 before:w-2/3 
            before:h-1.5 before:bg-violet-700 after:absolute after:bottom-0 
            after:right-0 after:w-2/3 after:h-1.5 after:bg-violet-700 py-4"
        >
            <h6 class="text-large sm:text-xl md:text-2xl">
                Want to know more?
            </h6>
            <h3 class="font-semibold text-3xl sm:text-4xl md:text-5xl">
                A bit <span class="poppins text-violet-400">about</span> me.
            </h3>
        </div>
        <p class="mx-auto poppins font-semibold text-lg sm:text-xl md:text-2xl">
            I am . . .
        </p>

        <!-- 3 bullet points -->
        <div class="flex flex-col gap-20 w-full mx-auto max-w-[800px]">
            {#each benefits as benefit, index}
                <div class="flex gap-6 sm:gap-8">
                    <p
                        class="poppins text-4xl sm:text-5xl md:text-6xl text-slate-500 font-semibold"
                    >
                        0{index + 1}
                    </p>
                    <div class="flex flex-col gap-6 sm:gap-8">
                        <h3 class="text-2xl sm:text-3xl md:text-5xl">
                            <span>{benefit.name}</span>
                        </h3>
                        <p>{benefit.description}</p>
                    </div>
                </div>
            {/each}
        </div>
        <h5 class={" text-2xl sm:text-3xl font-semibold text-center poppins "}>
            The <span class="text-violet-400">Complete</span> Package
        </h5>
        <div
            class="flex flex-col overflow-x-scroll gap-10 max-w-[800px] mx-auto w-full"
        >
            <table class="bg-white text-slate-700 rounded text-center">
                <thead class={"border-b border-solid border-slate-200  "}>
                    <tr class="">
                        <th />
                        <th class="whitespace-nowrap p-2 px-4">Candidate #1</th>
                        <th class="whitespace-nowrap p-2 px-4">Candidate #2</th>
                        <th class="whitespace-nowrap p-2 px-4">Candidate #3</th>
                        <th
                            class="bg-violet-700 text-white whitespace-nowrap p-4 px-8"
                            >Me</th
                        >
                    </tr>
                </thead>
                <tbody>
                    <!-- First row -->
                    <tr class="border-b border-solid border-slate-200">
                        <td
                            class="border-r border-solid border-white pl-4 pr-8 py-4 
                            font-semibold text-sm"
                            >Dedication</td
                        >
                        <td><i class="fa-solid fa-check text-slate-500" /></td>
                        <td><i class="fa-solid fa-check text-slate-500" /></td>
                        <td><i class="fa-solid fa-xmark text-slate-500" /></td>
                        
                        <!-- my checkmark -->
                        <td><i class="fa-solid fa-check text-green-500" /></td>
                    </tr>

                    <!-- Second row -->
                    <tr class="border-b border-solid border-slate-200">
                        <td
                            class="border-r border-solid border-white pl-4 pr-8 py-4 
                            font-semibold text-sm"
                            >Critical Thought</td
                        >
                        <td><i class="fa-solid fa-xmark text-slate-500" /></td>
                        <td><i class="fa-solid fa-check text-slate-500" /></td>
                        <td><i class="fa-solid fa-check text-slate-500" /></td>

                        <!-- my checkmark -->
                        <td><i class="fa-solid fa-check text-green-500" /></td>
                    </tr>

                    <!-- Third row -->
                    <tr>
                        <td
                            class="border-r border-solid border-white pl-4 pr-8 py-4 
                            font-semibold text-sm"
                            >Interpersonal Skills</td
                        >
                        <td><i class="fa-solid fa-xmark text-slate-500" /></td>
                        <td><i class="fa-solid fa-xmark text-slate-500" /></td>
                        <td><i class="fa-solid fa-check text-slate-500" /></td>

                        <!-- my checkmark -->
                        <td><i class="fa-solid fa-check text-green-500" /></td>
                    </tr>

                    <!-- Fourth row -->
                    <tr class="border-t border-solid border-slate-200">
                        <td
                            class="border-r border-solid border-white pl-4 pr-8 py-4 
                            font-semibold text-sm"
                            >Progamming Ability</td
                        >
                        <td><i class="fa-solid fa-check text-slate-500" /></td>
                        <td><i class="fa-solid fa-check text-slate-500" /></td>
                        <td><i class="fa-solid fa-xmark text-slate-500" /></td>

                        <!-- my checkmark -->
                        <td><i class="fa-solid fa-check text-green-500" /></td>
                    </tr>
                </tbody>
            </table>
        </div>
        <div class="mx-auto -mt-12 italic sm:hidden opacity-50">
            <p>Scroll to see more &rarr;</p>
        </div>
        <p class="mx-auto">So why not invest?</p>
    </section>
</main>