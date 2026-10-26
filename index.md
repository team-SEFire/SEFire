---
layout: default
title: Home
---
<div class="page-title">
    <h1>Welcome to SEFire</h1>
    <div class="title-line">
        <span></span>
        <div class="title-diamond"></div>
        <span></span>
    </div>
    <p>Making shared household expenses easier to manage.</p>
</div>

<div class="presentation-container">

    <!-- Presentation Tabs For Landing Page-->
    <div class="presentation-tabs">
        <button class="tab active"
                onclick="switchTab(0)">
            Elevator Pitch
        </button>

        <button class="tab"
                onclick="switchTab(1)">
            Problem Description
        </button>

        <button class="tab"
                onclick="switchTab(2)">
            Customers and End Users
        </button>

        <button class="tab"
                onclick="switchTab(3)">
            Solution Statement
        </button>
    </div>

    <!-- Presentation Content -->
    <div class="presentation-window">
        <div class="presentation-slider">

            <!-- Elevator Pitch -->

            <section class="presentation-panel">
                <div class="document-card">

                    <h2>Elevator Pitch</h2>
                    <p> SEFire is a shared expense tracker designed for roommates, 
                        couples, and households. It allows users to record shared expenses, 
                        customize how costs are split, track outstanding balances, and record 
                        payments in one place. SEFire helps users better understand their 
                        finances by providing budgeting guidance, financial vocabulary tooltips 
                        and access to custom variable expenses. These features help make managing 
                        shared household expenses more organized and easier to for everyone.
                    </p>
                </div>
            </section>

            <!-- Problem Description -->

            <section class="presentation-panel">
                <div class="document-card">

                    <h2>Problem Description</h2>
                    <p> Managing financial responsibilities in shared households can be 
                        difficult. Tracking who pays for rent, utilities, groceries, and 
                        other shared expenses can be confusing and may lead to missed 
                        payments or disagreements.
                    </p>

                </div>
            </section>

            <!-- Customers and End Users -->

            <section class="presentation-panel">
                <div class="document-card">

                    <h2>Customers and End Users</h2>
                    <p> People who live in shared households and need to manage financial 
                        responsibilities together. This includes:
                            - roommates 
                            - couples 
                            - families
                    </p>
                </div>
            </section>

            <!-- Solution Statement -->

            <section class="presentation-panel">
                <div class="document-card">

                    <h2>Solution Statement</h2>
                    <p> SEFire is a mobile friendly application that help roomates record shared expenses, 
                        calculate each members shared expenses and track outstanding balances. The application 
                        also informs its members of the importance of budgeting and explaining financial 
                        vocabulary using helpful tooltips.
                    </p>
                </div>
            </section>
            
        </div>
    </div>

Welcome to Team Sapphire's SEFire project website! This website contains information about our team, our project, and our project documentation. Please use the navigation bar at the top of the page to explore the site.

<script>
function switchTab(index) {
    const slider = document.querySelector(".presentation-slider");
    const tabs = document.querySelectorAll(".presentation-tabs .tab");

    slider.style.transform = `translateX(-${index * 100}%)`;

    tabs.forEach((tab, i) => {
        tab.classList.toggle("active", i === index);
    });
}
</script>