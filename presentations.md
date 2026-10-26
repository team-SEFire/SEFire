<div class="page-title">
    <h1>Presentations</h1>
    <div class="title-line">
        <span></span>
        <div class="title-diamond"></div>
        <span></span>
    </div>
    <p>This page contains Team Sapphire's Presentations.</p>
</div>

<div class="presentation-container">

    <!-- Presentation Tabs -->
    <div class="presentation-tabs">
        <button class="tab active"
                onclick="switchTab(0)">
            Feasibility
         </button>

         <button class="tab"
                onclick="switchTab(1)">
            Design
         </button>
     </div>

         <!-- Presentation Content -->
         <div class="presentation-window">
             <div class="presentation-slider">

                <!-- Feasibility Presentations -->
                <section class="presentation-panel">
                    <div class="document-card">

                        <h2>Final Feasibility Presentation</h2>
                        <p>Team Sapphire's final feasibility presentation.</p>
                        <iframe src="https://docs.google.com/presentation/d/e/2PACX-1vQYIuJS-Ri-nYnyNarmIV49zhRbGxLVk6GiArFXhJMYgQ3H0W3uWdGdfBXekT8Tms9-vj7ANxSLTzaT/pubembed?start=false&loop=false&delayms=3000" 
                            frameborder="0" 
                            width="960" 
                            height="569" 
                            allowfullscreen="true" 
                            mozallowfullscreen="true" 
                            webkitallowfullscreen="true">
                        </iframe>
                    </div>
                        
                    <div class="document-card">

                        <h2>Feasibility Presentation 3</h2>
                        <p>Team Sapphire's working draft feasibility iteration 3.</p>
                        <iframe src="https://docs.google.com/presentation/d/e/2PACX-1vQklsyOx9RuTppmtaKkMpXTguSAu4nU1TwbRy6ofYTq7O-6J9yrmq0jucHLArKJ2vZidWjXRaX0d6t6/pubembed?start=false&loop=false&delayms=3000" 
                            frameborder="0" 
                            width="960" 
                            height="569" 
                            allowfullscreen="true" 
                            mozallowfullscreen="true" 
                            webkitallowfullscreen="true">
                        </iframe>
                    </div>

                    <div class="document-card">

                        <h2>Feasibility Presentation 2</h2>
                        <p>Team Sapphire's working draft feasibility iteration 2.</p>
                        <iframe src="https://docs.google.com/presentation/d/e/2PACX-1vRz1CJ4ZdMb8yzcfDdlZxdm0K7qmG7ZQXqDICrENKkcbK4rSAc7V0mogVhBWWbBIJ39kApZq_I0GlnK/pubembed?start=false&loop=false&delayms=3000"
                            frameborder="0" 
                            width="960" 
                            height="569" 
                            allowfullscreen="true" 
                            mozallowfullscreen="true" 
                            webkitallowfullscreen="true">
                        </iframe>
                    </div>

                    <div class="document-card">

                        <h2>Feasibility Presentation 1</h2>
                        <p>Team Sapphire's working draft feasibility iteration 1.</p>
                        <iframe src="https://docs.google.com/presentation/d/e/2PACX-1vRVMr8o50jrLw9AzkrDNUNNSzoZ4EqYR5OUdjNUkeVRYzkFVE2eNKx6VYiVJ-NAZGZamcCdNBGYVjlB/pubembed?start=false&loop=false&delayms=3000"
                            frameborder="0" 
                            width="960" 
                            height="569" 
                            allowfullscreen="true" 
                            mozallowfullscreen="true" 
                            webkitallowfullscreen="true">
                        </iframe>
                    </div>
                </section> 

                <!-- Design Presentation -->
 
                <section class="presentation-panel">
                    <div class="document-card">
                        
                        <h2>Working Draft Design Presentation</h2>
                        <p> Team Sapphire's Working Draft Design Presentation. </p>
                        <iframe src="https://docs.google.com/presentation/d/e/2PACX-1vRbRb7tXpGGjHMfbRmB8P2mzGus0K_hJB7g8VyalzEM-G_p1xlP8Q-n1OcdycBSomLCXyvSREcXkAld/pubembed?start=false&loop=false&delayms=3000" 
                            frameborder="0" 
                            width="960" 
                            height="569" 
                            allowfullscreen="true" 
                            mozallowfullscreen="true" 
                            webkitallowfullscreen="true">
                        </iframe>
                    </div>
                </section>
            </div>
        </div>
    </div>                
</div>



<script>
function switchTab(index) {
    const slider = document.querySelector(".presentation-slider");
    const tabs = document.querySelectorAll(".presentation-tabs .tab");
    const panels = document.querySelectorAll(".presentation-panel");
    const windowElement = document.querySelector(".presentation-window");

    if (!slider || !windowElement || !panels[index]) return;

    slider.style.transform = `translateX(-${index * 100}%)`;

    tabs.forEach((tab, i) => {
        tab.classList.toggle("active", i === index);
    });

    windowElement.style.height = `${panels[index].offsetHeight}px`;
}

window.addEventListener("load", () => {
    switchTab(0);
});

window.addEventListener("resize", () => {
    const activeTab = document.querySelector(".presentation-tabs .tab.active");
    const tabs = [...document.querySelectorAll(".presentation-tabs .tab")];

    if (activeTab) {
        switchTab(tabs.indexOf(activeTab));
    }
});
</script>