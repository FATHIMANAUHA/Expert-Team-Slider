# Expert-Team-Slider
Moves the slider left or right based on the arrow clicked.This feature allows users to toggle between a short and full description for each team member.the full description.Hides the short descriptn.Changes the button text to "Read Less".Clicking "Read Less" Hides the full description.Shows the short description again.
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Team Section</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            margin: 0;
            padding:0;
            box-sizing: border-box;
        }

        .team-section {
            display: flex;
            justify-content: center;
            overflow: hidden;
            padding: 20px;
            max-width: 950px;
            margin: auto;
            position: relative;
            width: 100%;
        }

        .slider-wrapper {
            display: flex;
            transition: transform 0.5s ease-in-out;
            will-change: transform;
            flex-wrap: nowrap;
        }

        .team-card {
            flex: 0 0 300px;
            max-width: 400px;
            background: white;
            border: 1px solid #ddd;
            border-radius: 10px;
            text-align: center;
            box-shadow: 0 4px 6px rgba(0, 0, 0, 0.1);
            padding: 15px;
            margin-right: 15px;
        
        }

        .team-card img {
    width: 100px; /* Adjust the size as needed */
    height: 100px; /* Adjust the size as needed */
    border-radius: 50%; /* Makes the image circular */
    object-fit: cover; /* Ensures the image covers the area without distortion */
    margin-bottom: 10px; /* Adds space between the image and the text */
}

        
     


        .team-card h3 {
            font-size: 18px;
            font-weight: bold;
            margin: 10px 0;
        }

        .team-card .description {
            font-size: 14px;
            color: #555;
            margin: 10px 0;
        }

        .team-card .full-desc {
            display: none;
        }

        .team-card a {
            display: inline-block;
            margin-top: 10px;
            font-size: 14px;
            color: #0066cc;
            text-decoration: none;
            cursor: pointer;
        }

        .team-card a:hover {
            text-decoration: underline;
        }

        /* Arrow buttons */
        .slider-arrow {
            position: absolute;
            top: 50%;
            transform: translateY(-50%);
            background-color: rgba(0, 0, 0, 0.5);
            color: white;
            padding: 10px;
            cursor: pointer;
            border-radius: 50%;
            z-index: 10;
        }

        .slider-arrow.left {
            left: 10px;
        }

        .slider-arrow.right {
            right: 10px;
        }
        
    </style>
</head>
<body>
    <div class="slider-arrow left" onclick="moveSlide(-1)">&#10094;</div>
    <div class="slider-arrow right" onclick="moveSlide(1)">&#10095;</div>
    <div class="team-section">
        <div class="slider-wrapper">
            <!-- Team Cards (Ensure 6 total cards here) -->
        
            <div class="team-card">
                <img src="https://projects.backb.ca/nmc/wp-content/uploads/2024/12/financial-consultant-planning-home-finances-with-his-client-.jpg" alt="Ritesh Kapoor">
                <h3>Ritesh Kapoor</h3>
                <div class="description">
                    <span class="short-desc">FCA, (Consultant) - Handles statutory compliance matters He is a Qualified Chartered Accountant and commerce graduate from the University ofHe is a Qualified Chartered Accountant and commerce graduate from the University Handles statutory compliance matters He is a Qualified Chartered Accountant and commerce graduate from the University ofHe is a Qualified Chartered Accountant and commerce graduate from the University.</span>
                </div>
                </div>
            <div class="team-card">
                <img src="https://projects.backb.ca/nmc/wp-content/uploads/2024/12/financial-consultant-planning-home-finances-with-his-client-.jpg" alt="Ritesh Kapoor">
                <h3>Ritesh Kapoor</h3>
                <div class="description">
                    <span class="short-desc">FCA, (Consultant) - Handles statutory compliance matters He is a Qualified Chartered Accountant and commerce graduate from the University of Delhi. Ritesh Kapoor handles statutory compliance matters related to the Mumbai office.</span>
                </div>
              
            </div>
            <div class="team-card">
                <img src="https://projects.backb.ca/nmc/wp-content/uploads/2024/12/financial-consultant-planning-home-finances-with-his-client-.jpg" alt="Ritesh Kapoor">
                <h3>Ritesh Kapoor</h3>
                <div class="description">
                    <span class="short-desc">FCA, (Consultant) - Handles statutory compliance matters.</span>
                    <span class="full-desc"> He is a Qualified Chartered Accountant and commerce graduate from the University of Delhi. Ritesh Kapoor handles statutory compliance matters related to the Mumbai office.</span>
                </div>
                
            </div>
            <div class="team-card">
                <img src="https://projects.backb.ca/nmc/wp-content/uploads/2024/12/financial-consultant-planning-home-finances-with-his-client-.jpg" alt="Ritesh Kapoor">
                <h3>Ritesh Kapoor</h3>
                <div class="description">
                    <span class="short-desc">FCA, (Consultant) - Handles statutory compliance matters ied Chartered Accountant and commerce graduate from the University ofied Chartered Accountant and commerce graduate from the University of.</span>
                </div>
                
            </div>
            <div class="team-card">
                <img src="https://projects.backb.ca/nmc/wp-content/uploads/2024/12/financial-consultant-planning-home-finances-with-his-client-.jpg" alt="Ritesh Kapoor">
                <h3>Ritesh Kapoor</h3>
                <div class="description">
                    <span class="short-desc">FCA, (Consultant) - Handles statutory compliance matters  He is a Qualified Chartered Accountant and commerce graduate from the University of Delhi He is a Qualified Chartered Accountant and commerce graduate from the University of Delhi.</span>
                </div>
                
            </div>
            <div class="team-card">
                <img src="https://projects.backb.ca/nmc/wp-content/uploads/2024/12/financial-consultant-planning-home-finances-with-his-client-.jpg" alt="Ritesh Kapoor">
                <h3>Ritesh Kapoor</h3>
                <div class="description">
                    <span class="short-desc">FCA, (Consultant) - Handles statutory compliance matters He is a Qualified Chartered Accountant and commerce graduate from the UniversityHe is a Qualified Chartered Accountant and commerce graduate from the University.</span>
                </div>
                
            </div>
            <div class="team-card">
                <img src="https://projects.backb.ca/nmc/wp-content/uploads/2024/12/financial-consultant-planning-home-finances-with-his-client-.jpg" alt="Ritesh Kapoor">
                <h3>Ritesh Kapoor</h3>
                <div class="description">
                    <span class="short-desc">FCA, (Consultant) - Handles statutory compliance matters  He is a Qualified Chartered Accountant and commerce graduate from the University  He is a Qualified Chartered Accountant and commerce graduate from the University  He is a Qualified Chartered Accountant and commerce graduate from the University .</span>
                </div>
                
            </div>
            <!-- Add more team cards here as needed -->
            <!-- Total of 6 cards to showcase -->
        </div>
        <!-- Arrow Buttons -->       
    </div>
    <script>
        const sliderWrapper = document.querySelector('.slider-wrapper');
        const teamCards = Array.from(sliderWrapper.children); // Get all the team cards
        const cardWidth = 300; // Width of each card
        const gap = 15; // Margin between cards
        const visibleCards = 3; // How many cards should be visible at once
        const slideWidth = (cardWidth + gap) * visibleCards; // Total width of the visible area
        let currentIndex = 0;

        // Set the total width of the slider to accommodate all the cards
        sliderWrapper.style.width = `${(cardWidth + gap) * teamCards.length - gap}px`;

        // Move slides with left or right arrows
        function moveSlide(direction) {
            const newIndex = currentIndex + direction;

            // Check if we are within bounds for the cards remaining
            if (newIndex <= teamCards.length - visibleCards && newIndex >= 0) {
                currentIndex = newIndex;
            }

            // Move the wrapper to show the new slide
            sliderWrapper.style.transition = 'transform 0.5s ease-in-out';
            sliderWrapper.style.transform = `translateX(${-currentIndex * (cardWidth + gap)}px)`;
        }

        // Make sure we never go beyond the last set of 3 cards
        const updateSliderPosition = () => {
            if (currentIndex >= teamCards.length - visibleCards) {
                currentIndex = teamCards.length - visibleCards; // Stop at last set of cards
            }
            sliderWrapper.style.transform = `translateX(${-currentIndex * (cardWidth + gap)}px)`;
        }
        window.addEventListener('resize', updateSliderPosition);
    </script>
</body>
</html>
