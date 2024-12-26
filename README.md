# VivvoybyVivoPressMMXXIIII

## SUMMARY

www.vivvoy.fr © VivoPress July MMXXIIII

Vivre & voyager en France 
Living & traveling in France

Votre site d’informations touristiques, patrimoniales et culturelles, édité par vous pour vous.

Your site of tourism, heritage and cultural information, edited by you for you.


Parlez-nous de vous, il n’y a que cela qui nous intéresse.
Tell us about you, there is only what interests us.            

Vivvoy est une publication de VivoPress 2.0, l’éditeur de vos passions. 
Pour plus de renseignements, consultez-nous. 

Vivvoy is a publication of VivoPress 2.0, the publisher of your passions. 
For more information, contact us.

contact@vivvopress.fr


©  VivoPress 07.2024     


1 & 2 //



V I V V O Y  by  VivoPress 2.0 
Philippe Marclay (Team’s member)

 THE DIGITAL TOOLS
 SERVING THE PROJECT VIVVOY 

3 // TECHNOLOGIES

Python and many technologies allow me to create my website of tourist and heritage information, due to its versatility and popularity.

Here are some ways in which Python can be useful in this context.

1. Web development with Flask or Django

Flask and Django are popular web frameworks in Python. They simplify the web development process by providing an organized structure for creating web applications. Flask can be used for simpler projects and Django for more complex ones.

2. Data processing with Pandas

Python has a rich library of data processing tools, which can be useful for organizing and presenting tourist information. Pandas is particularly powerful for working with tabular data.

3. Mapping with Folium or Geopandas
If your tourist information site includes interactive maps, libraries like Folium (which integrates with Leaflet) or Geopandas can allow you to add mapping features.

4. Web scraping for information gathering

I can use libraries like BeautifulSoup or Scrapy to extract information from other websites, for example, to update data on tourist attractions.

5. Database with SQLAlchemy or Django ORM

To store and manage data efficiently, I can use a database. SQLAlchemy is a popular library for this, which is built in if I use Django, its ORM (Object-Relational Mapping).

6. Integration with APIs
I can integrate third-party APIs to enrich my site. For example, weather APIs to provide local weather information, translation APIs for international visitors, etc.


7. Fast development with libraries and modules
Python has a wide range of libraries that can speed up development. For example, I can use graphic libraries like Matplotlib to generate graphics or images.

8. User and Security Management
Django includes user management, authentication and authorization features that may be essential for my site.

9. Easy to deploy
Python facilitates the deployment of web applications. Services such as Heroku, AWS, or DigitalOcean can be used to host my Python application.
IN SUMMARY, Python offers a combination of powerful tools, libraries and frameworks that can simplify the development of my tourism and heritage information site, covering aspects such as web development, data management, mapping and more.

4 // CHALLENGE STATEMENT

The objective of this project is to provide tourism and heritage information that is sourced, up-to-date and dynamic. It meets the growing needs of national and international audiences visiting and living in France. It also aims to provide digital tools for all stakeholders in the sectors concerned. VIVVOY is a technical and human interface, serving the greatest number of people.

5 // RISKS

1. - Risk 1: - Single points of failure (SPOF) and Potential impact.
If a critical component such as the web server, application server or database fails, the entire site may become unavailable resulting in lost revenue and user dissatisfaction.
  - Backup/Alternatives: Implement redundancy by adding failover systems (e.g., load balancing in Active-Active, database replication). Use clusters to ensure high availability.

2. Risk 2: Traffic overload:
  - Potential impact: A peak traffic (due to high season) could overload servers, resulting in slow performance or site unavailability.
  - Backup/Alternatives: Use a load balancer (e.g., HAProxy) to distribute incoming traffic across multiple servers. Set up automatic scaling (autoscaling) in the cloud to add servers in case of traffic peaks.

3. Risk 3: Security breaches (no firewall and HTTPS):
  - Potential impact: Without a firewall or encrypted (HTTPS) communication, the site is vulnerable to malicious attacks such as DDoS attacks, sensitive data interception or SQL injections. This could compromise the security of users and the site.
  - Backup/Alternatives: Install a web application firewall (WAF) to filter malicious traffic. Enforce the use of HTTPS to secure all communications and protect user data.
4. Risk 4: Lack of monitoring and surveillance:
  - Potential impact Without monitoring tools, it will be difficult to quickly detect and fix problems (server outages, memory leaks, degraded performance) which could negatively affect the user experience.
  - Backup/Alternatives : Implement monitoring tools such as Prometheus or Grafana to monitor server performance in real time and receive alerts if anomalies occur.

6 // INFRASTRUCTURE

1. ranching and Merging Strategy:
Our team will adopt GitHub Flow for managing our repository. This strategy ensures a smooth and flexible development process while keeping the main branch stable:
1.	Main Branch: The main branch will always contain production-ready code.
2.	Feature Branches: Each new feature or fix will be developed on a separate branch, named descriptively (e.g., feature/map-integration or bugfix/date-format).
3.	Pull Requests (PRs): Once a feature is complete, a PR will be opened to merge the branch into main. Peer reviews ensure code quality before merging.
4.	Merging: After approval, the branch will be merged into main, ensuring it passes all automated tests before deployment.
2. Deployment Strategy:
We’ll use a continuous deployment (CD) approach to keep the tourism website updated with minimal downtime:
1.	Staging Environment: Each change merged into main will first be deployed to a staging environment for final testing in a near-production setting.
2.	Automated Deployment: Once changes pass staging, they will be automatically deployed to production using tools like GitHub Actions or Jenkins.
3.	Rolling Deployments: To avoid downtime, we’ll use rolling deployments, allowing updates to be pushed without disrupting active users.
3. Populating the App with Data:
1.	Data Collection: The initial data, such as landmarks, tourist attractions, and local events, will be collected from publicly available sources, tourism boards, and partnerships with local stakeholders.
2.	Database: This data will be stored in a MySQL database, structured with tables for attractions, locations, events, and user feedback.
3.	Regular Updates: Content management tools will allow the team to manually update or add new entries, while periodic scripts or APIs can fetch and update real-time data (e.g., event schedules).
4. Testing Strategy:
1.	Automated Testing:
○	Unit Testing for individual components, ensuring each function of the site behaves as expected.
○	Integration Testing to verify how different modules (e.g., map integration and event listings) work together.
○	End-to-End Testing using tools like Selenium or Cypress to simulate real user interactions.
2.	Continuous Integration (CI):
○	We’ll use GitHub Actions or CircleCI to run tests automatically after each commit and before merging any branch into main.
3.	Manual Testing:
○	User Acceptance Testing (UAT) in the staging environment will ensure the website performs correctly from a user perspective before final deployment.
 // EXISTING SOLUTIONS

1. Tripadvisor
Similarities: Tripadvisor provides detailed information on tourist destinations, attractions and user reviews. It also provides personalized recommendations, maps and the ability to book tourist services such as hotels or guided tours.
Differences: Our site will focus more on local heritage, with a section dedicated to the history of the places, regional cultural events, and detailed information not only about major attractions but also less well-known sites. In addition, our goal is to create localized and collaborative content, in partnership with local guides and tourist offices.
2. Lonely Planet
Similarities: Lonely Planet offers detailed travel guides for various destinations around the world, including recommendations on places to visit, interactive maps, and practical tips for travelers.
Differences: While Lonely Planet primarily addresses a global audience, our site will focus on more local and regional recommendations, highlighting hidden treasures and heritage experiences specific to a particular region. We will also have a participatory component where users can contribute directly with their own recommendations.
Re-implementation of a proven solution:
We have chosen to reimplement a solution based on recommendations of places and activities, a model commonly used by platforms such as Tripadvisor and Lonely Planet. However, our special specification will be oriented towards a local and community approach, with a collaborative content section where users and local experts can propose unknown sites and events.

Why this reimplementation?
Local focus: Large global platforms often do not cover small destinations or local heritage sites in detail. Our solution fills this gap by providing detailed information on regional cultural and historical aspects.
Community approach: We also want to integrate a participatory dimension, where users can contribute to the enrichment of local data, with editorial control to ensure the quality and veracity of information.
Single user experience: Where other solutions are often focused on booking and quick consumption of information, our platform will focus on learning, in-depth exploration of the regions, and preservation of local cultural treasures.


Edited on 02.05.2024 and corrected on 13.09.2024,
by Philippe Marclay, digital editor, for the VIVVOY project by VivoPress 2.0.
:JUSTUS UT ACER:

____________________________________________________________________________________________________________________________________


