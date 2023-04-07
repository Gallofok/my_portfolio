Skip to content
Search or jump to…
Pulls
Issues
Codespaces
Marketplace
Explore
 
@Gallofok 
Gallofok
/
my_portfolio
Public
Cannot fork because you own this repository and are not a member of any organizations.
Code
Issues
Pull requests
Actions
Projects
Wiki
Security
Insights
Settings
my_portfolio/index.html
@Gallofok
Gallofok Add files via upload
Latest commit 68bb6be 20 minutes ago
 History
 1 contributor
191 lines (169 sloc)  6.44 KB
 

<!DOCTYPE html>
<html>
  <head>
    <title>Jane Doe - Portfolio</title>
    <link rel="stylesheet" href="./style.css"/>
    <script src="./script.js"></script>
  </head>
  <body>
    <!-- Navigation Bar -->
    <nav>
      <div id="home">
        <div class="profile_name">
          Jane Doe
          <div class="contact_info">
            <img src="html_finalprojimages/envelope.png" alt="https://icons8.com/icon/124377/circled-envelope"/>
          jdoe@jeemail.com
        </div>
        <div style="clear:both;"></div>
        <div class="contact_info">
          <img src="html_finalprojimages/phone.png" alt="https://icons8.com/icon/124377/circled-envelope"/>
          +13456764598

        </div>
        </div>
        <div class="topdiv">
          <a class="topmenu" href="#about-me">About Me</a>
          <!-- Add the links for Skills, Projects and Recommendation here -->

        </div>
      </div>    
    </nav>

    <!-- About Me -->
    <section id="about-me" class="container">
      <div>
        <img src="https://miro.medium.com/max/1400/1*qdAW1TjCN57h1lbuuzvchg.gif" class="profile_image"/>
      </div>

      <div>
          <h1>
            Hi, I'm Jane Doe! <img src="https://twemoji.maxcdn.com/2/72x72/1f44b.png" width="60px"/>
          </h1>
          <p>
            I am a full stack developer with 2 years of experience in both application and presentation layers.
            I have worked on applications and microservices deployed on IBM Cloud. 
            I am an avid user of IBM Watson Services and have worked on Watson Assistant, NLU, Sentiment analyzer to name a few.
          </p>
      </div>
    </section>
              
    <!-- Skills -->
    <section id="skills">
      <h2>Skills</h2>
      <div style="clear:both;"></div>

      <div class="all_skills">
        <div class="skill">
          <img src="html_finalprojimages/html5.png"/>
          <h6>HTML</h6>
          <p>2 years experience</p>
        </div>  

        <div class="skill">
          <img src="html_finalprojimages/js.jpeg"/>
          <h6>JavaScript</h6>
          <p>3 years experience</p>
        </div>  

        <div class="skill">
            <img src="html_finalprojimages/java.png"/>
            <h6>JavaScript</h6>
            <p>.5 years experience</p>
        </div>

        <div class="skill">
            <img src="html_finalprojimages/react.png"/>
            <h6>JavaScript</h6>
            <p>1 year experience</p>
        </div>         
        
        <div class="skill">
            <img src="html_finalprojimages/node.png"/>
            <h6>JavaScript</h6>
            <p>1 year experience</p>
        </div>    
        <!-- Add more skills here -->


      </div>
    </section>
          
    <!-- Projects -->
    <section class="projects" id="projects">
      <h2>
        Projects
      </h2>
      <div style="clear:both;"></div>

        <div id="projects-container" class="projects-container">
          <div class="project-card">
            <h3>Chatbot</h3>
            <ul>
              <li>Developed a secure website integrated with chatbot for an automobile client using HTML, CSS, JavaScript and IBM Watson Assistant</li>
            </ul>
          </div>
          <hr>
          <div class="project-card">
            <h3>Sentiment Analyzer</h3>
            <ul>
              <li>Developed and deployed a sentiment analyzer for the box reviews section of an eCommerce platform using IBM NLU</li>
            </ul>
          </div>
          <hr>
          <div class="project-card">
            <h3>Fashion Website</h3>
            <ul>
              <li>Created a styled multi-page website for a new player in the fashion industry and integrated it with a shopping cart, using stripe for payment gateway</li>
            </ul>
          </div>
    </div>
    </section>
    <div style="clear:both;"></div>

    <!-- Recommendations -->
    <section id="recommendations">
      <h2>Recommendations</h2>
      <div style="clear:both;"></div>
      <div class="all_recommendations" id="all_recommendations">
        <div class="recommendation">
          <span>&#8220;</span>
          Jane is a very quick learner and quickly grasps key concepts of Web development. 
          She got a great attitude & she is an excellent team player. 
          She has a curious mind and asks the right question. 
          She takes initiative within a team and has potentials to lead the team.
          <span>&#8221;</span>
        </div>
        <div class="recommendation">
          <span>&#8220;</span>
          Working with Jane has been an awesome experience. 
          She is highly knowledgable and always goes the extra step to make sure everything is right. 
          For any future projects that need her expertise I would definitely want to work with her again.
          <span>&#8221;</span>
        </div>
        <div class="recommendation">
          <span>&#8220;</span>
          I had worked along with Jane during the initial phase of our venture which needed Web development. 
          She is a committed resource who has in depth knowledge about the domain. 
          She will be an asset for any organisation! 
          <span>&#8221;</span> 
        </div>
        <div class="recommendation">
            <span>&#8220;</span>
            Jan is a good girl
            <span>&#8221;</span> 
          </div>

      </div>
    </section>

    <!-- Recommendation Form -->
    <section id="contact">
      <div class="flex_center">
        <fieldset>
          <legend class="introduction">Leave a Recommendation</legend>          
          <input type="text" placeholder="Name (Optional)"> <br/>
          <textarea id="new_recommendation" cols="500" rows="10" placeholder="Message"></textarea>
          <div class="flex_center">
            <button id="recommend_btn" onclick="addRecommendation()">Submit</button>
          </div>
        </fieldset>
      </div>
    </section>

    <div class="iconbutton">
      <a href="#home">
        <svg xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 24 24" stroke-width="1.5" stroke="white" width="63px">
            <path stroke-linecap="round" stroke-linejoin="round" d="M15 11.25l-3-3m0 0l-3 3m3-3v7.5M21 12a9 9 0 11-18 0 9 9 0 0118 0z" />
          </svg>
      </a>
    </div>


    <div class="popup" id="popup" class="flex_center">
      <img src="html_finalprojimages/checkmark--outline.svg"/>
      <h3>Thank you for submitting your recommendation!</h3>
      <button onclick="showPopup(false)">Ok</button>
    </div>


  </body>
</html>
Footer
© 2023 GitHub, Inc.
Footer navigation
Terms
Privacy
Security
Status
Docs
Contact GitHub
Pricing
API
Training
Blog
About
my_portfolio/index.html at main · Gallofok/my_portfolio
