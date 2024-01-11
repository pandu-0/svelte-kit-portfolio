<script>
    import Step from "./Step.svelte";

    let steps = [
        {
            name: "Damaged Car Parts Image Recognition ML model",
            // Icons are from https://fontawesome.com/
            icon: "fa-solid fa-car-burst fa-shake",
            style: "--fa-animation-duration: 3s;",
            description: "None",
            href: "https://github.com/pandu-0/Damaged-Car-Parts-Recognition-ML-Model",
        },
        {
            name: "Car Resale Price Prediction",
            icon: "fa-solid fa-money-check-dollar fa-bounce",
            style: "--fa-animation-duration: 3s; --fa-bounce-height: -20px;",
            description: "INSERT1",
            href: "https://www.kaggle.com/code/pandu0/car-resale-price-prediction-scikit-learn",
        },
        {
            name: "Coming Soon...",
            icon: "fa-solid fa-question fa-spin",
            style: "--fa-animation-duration: 3s;",
            description: "None",
            href: "#",
        },
    ];

    let benefits = [
        {
            before_name: "A",
            name: " Self Taught ",
            after_name: "Programmer",
            description:
                "In addition to knowledge I've gained from my college classes, I've taken the initiative to " +
                "independently learn and master new programming and Machine Learning concepts. This self-directed " +
                "learning has enabled me to deepen my understanding of concepts and broaden my skill set. " +
                "I've successfully learned Python, Scikit-Learn, and Markdown! This continuous learning process " +
                "underscores my commitment to stay updated and adaptable in the ever-evolving field of Data Science.",
        },
        {
            before_name: "A",
            name: " Machine Learning ",
            after_name: "Enthusiast",
            description:
                "I've always loved trying to predict little things in life. After taking CS 131 that " + 
                "covered a bit of Machine Learning, I developed a passion to learn and understand ML concepts. " +
                "I made my first successful model with the help of a Google Lab which is capable of recognizing damaged car parts. " +
                "In turn, it pushed me to work on more project ideas to predict more things!",
        },
        {
            before_name: "An",
            name: " Excellent ",
            after_name: "Communicator",
            description:
                "I firmly believe in the importance of clear and open communication. I think it's crucial to " +
                "maintain transparency and engage in meaningful conversations. This approach not only helps me " +
                "establish profound connections, but also enhances my efficiency " +
                "and productivity in any team.",
        },
    ];
</script>

<main class="flex flex-col flex-1 p-4">
    <meta charset="UTF-8"/>
    <section
        id="introPage"
        class="grid grid-cols-1 lg:grid-cols-2 gap-10 py-8 sm:py-14">

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
            <a style="box-shadow: 2px 2px 3px grey; text-shadow: 3px 3px 3px lightgrey;" 
            class="blueShadow mx-auto lg:mr-auto text-base 
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
                    <i class="fa-brands fa-github fa-2xl"></i>
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
                My <span class="poppins text-violet-400">Coding</span> Odyssey!
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
                <p class="text-left">
                    I developed a <strong class="text-violet-400">specialized machine learning model</strong> 
                    that can identify damaged sections of a car from an image. This model was trained 
                    using the <strong class="text-violet-400">Vertex AI AutoML Vision on the Google Cloud Platform</strong>. 
                    It can <strong class="text-violet-400">accurately categorize</strong> 
                    damage into various parts such as the Bumper, Engine compartment, Hood, Lateral, and Windshield with a 
                    precision of 73% and a recall rate of 50%.
                </p>
            </Step>

            <!-- PROJECT 2 -->
            <Step step={steps[1]}>

                <p class="text-left">
                    This is my first ML model that I coded! I used <strong class="text-violet-400">Scikit-learn</strong> 
                    in Python to create two predictive Regression models using <strong class="text-violet-400">K-Nearest Neighbors</strong> 
                    and <strong class="text-violet-400">Random Forest</strong> algorithms. I also learned Pandas, Matplotlib, 
                    and Seaborn for comprehensive <strong class="text-violet-400">data cleaning</strong>, 
                    <strong class="text-violet-400">analysis</strong>, and <strong class="text-violet-400">visualization</strong>  
                    to gain insights and for informed model development. In addition, I applied GridSearch for 
                    <strong class="text-violet-400">hyperparameter tuning</strong> to optimize the performance of the ML models.
                </p>

            </Step>

            <!-- PROJECT 3 -->
            <Step step={steps[2]}>
                <p class="text-center">
                    In theaters only 🎬 ;)
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
                    <!-- Number next to the Header -->
                    <p
                        class="poppins text-4xl sm:text-5xl md:text-6xl text-slate-500 font-semibold">
                        0{index + 1}
                    </p>
                    <!-- Header -->
                    <div class="flex flex-col gap-6 sm:gap-8">
                        <h3 class="text-2xl sm:text-3xl md:text-5xl">
                            <span>{benefit.before_name}</span>
                            <span class="text-violet-400">{benefit.name}</span>
                            <span>{benefit.after_name}</span>

                        </h3>
                        <!-- Paragraph -->
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

        <!-- Table -->
            <table class="bg-white text-slate-700 rounded text-center">
                <thead class={"border-b border-solid border-slate-200"}>
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