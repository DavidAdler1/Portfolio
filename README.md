# David's Grand Shop - Capstone Project Portfolio

## The Mission
My project started with a simple idea: online shopping should be easy, safe, and fair. I noticed that many current e-commerce sites are either too complicated, not secure enough, or don’t always put users first. So, I set out to build an online store that anyone can use without hassle, where security and ethical practices come first.​

I wanted to create a website where signing up, logging in, browsing products, managing your cart, and checking out is straightforward and enjoyable. At the same time, I made sure to protect user data with secure coding practices and careful handling of information.​

My design is simple and organized. By separating the data, the look of the site, and user interactions, I made the website easy to maintain and improve over time. This approach not only meets my current needs but also sets me and my project up for future growth.​

In short, my mission is to build a reliable and ethically driven online store that makes shopping easy and secure, while staying true to the values of fairness and responsibility. 

---

## Project Navigation

[Application Demo](Demo.md)

[Project Approach](Approach.md)

[Setup & Installation Guide](Setup.md)

[Key Code Snippets & Implementation](Code_Snippets.md)

[Project Diagrams & Architecture](diagrams.md)


---


### High-level Functional Requirements

User Registration & Login

- Users can create an account and log in securely.

- Session-based authentication ensures that only logged-in users can access the website

Product Browsing & Search

- Users can view all products and search by name or keyword.

Shopping Cart Functionality

- Users can add, remove, and update products in their cart.

- Cart data persists between sessions using cookies.

Checkout & Order Processing

- Logged-in users can place an order.

- Product inventory is updated in the database after checkout.

Order History & User Profiles

- Users can view their order history and update personal information.

Admin Controls

- Admin users can view, edit, or delete products.

- Admins can view, edit, or delete the list of all registered users.

---

### High-Level Non-Functional Requirements
Security

- Uses secure sessions for authentication.

- Admin access is protected by the isAdmin flag.

- Data validation and SQL injection protection via parameterized queries.

Performance

- Lightweight ADO.NET access means fast, direct SQL communication.

- Optimized queries minimize server load and improve responsiveness.

Scalability

- Clean MVC architecture with service layers allows easy scaling of features.

- Modular codebase allows new services and views to be added independently.

Maintainability

- Follows good principles with the separation of concerns between controllers, services, models, and views.

- Business logic is encapsulated in services, making the system easy to update or debug.

Usability

- Clean and easy-to-use user interface for both customers and admins.

Reliability

- SQL transactions prevent data inconsistency during checkout.

- ILogger helps detect and resolve issues fast.

---

### Technologies Chosen

- ASP.NET MVC (C#) – For its clear structure and separation of concerns using the Model-View-Controller pattern. It made my app more organized and maintainable.

- SQL Server – To store all user, product, and order data. It’s secure, reliable, and works well with .NET.

- ADO.NET – For direct communication with the database using SQL queries. It gave me full control over how I handled data.

- HTML, CSS, and Razor – For building clean and dynamic views. Razor let me combine C# and HTML easily for interactive pages.

- IHttpContextAccessor – For managing user sessions like login state, admin roles, and the shopping cart. I chose this to be able to use user data.

- ILogger – For tracking user activity, especially logins, and handling any errors for debugging.

---

### Industry Best Practices
- Separation of Concerns – I followed the MVC architecture to separate the user interface, business logic, and data access, making the code easier to manage and scale.

- Security Practices – I used session-based authentication and added user roles to control access to admin features.

- Service Layer Architecture – I created service classes like CartService, OrderService, and SecurityService to handle business logic separately from the controllers.

- Input Validation and Error Handling – I added checks during checkout, such as filtering out products with zero quantity, and used TempData for user-friendly error messages.

- Code Reusability and Modularity – Reusable methods and structured models made it easier to maintain and extend the project later.

- Secure Cookie Handling – I used HttpOnly, Secure, and SameSite cookie options when saving cart data to prevent tampering and cross-site attacks.

---
  
### Cloud Deployment
- Yes, my project is deployed to the cloud using Azure.

---
  
### How were DevOps principles applied?
This Project Followed the full Software Development Life Cycle.​

- Jira was used for sprint planning and management.​

- GitHub was used for code updates and version control.​

- Postman was used for API Testing and development.

---
  
### New Technologies Learned
- Learned about MVC architecture to better organize the project.

- Learned Jira for sprint planning and task tracking.

- Improved skills with Postman for API testing.

- Gained experience with GitHub for version control and collaboration.

- Learned session handling to manage user authentication and state.

---

### Technical Approach
Followed the MVC (Model-View-Controller) design pattern to separate concerns:

- Models for data representation

- Views for the UI

- Controllers for user interaction and routing

- Used Service Classes to handle business logic like cart operations and order processing.

- Implemented Session and Cookie Handling for user authentication and cart persistence.

- Used SQL Server for database storage and interaction via ADO.NET with SqlConnection.

- Applied Form Validation and input sanitization to ensure secure and clean data handling.

---

  
### Diagrams
For a detailed view of all the diagrams, please visit the [Diagrams Page](diagrams.md).

---


### Risks and Challenges
- Challenge: Integrating the front and backend and ensuring smooth data flow.
- Solution: Used the MVC pattern to separate concerns and tested functionality frequently.

- Challenge: Manage user sessions and cart persistence, ensuring the cart remains intact even after the page refreshes.
- Solution: Implemented cookie-based cart management using the CartService and session handling for user authentication.

- Challenge: Managing time constraints while interacting with issues that persist as development continues.
- Solution: Prioritized simple features first. Debugged issues as they came up.
  
- Challenge: Managing time constraints while addressing issues that persisted as development continued.
- Solution: Prioritized simpler features first and debugged issues as they came up to avoid delaying progress.
  
---

### Outstanding Issues
- CI/CD Pipeline issues with GitHub - Azure Web app user doesnt have correct admin status.

---

### Resources Used: 
How do I use cookies to store shopping cart content?. Stack Overflow. (2016, October). https://stackoverflow.com/questions/39860045/how-do-i-use-cookies-to-store-shopping-cart-content 

MozDevNet. (2025, April 11). HTML elements reference - HTML: Hypertext markup language: MDN. MDN Web Docs. https://developer.mozilla.org/en-US/docs/Web/HTML/Reference/Elements 

MozDevNet. (2025a, March 24). CSS reference - CSS: Cascading style sheets: MDN. MDN Web Docs. https://developer.mozilla.org/en-US/docs/Web/CSS/Reference 

Egeo, & egeoegeo                      32333 silver badges2525 bronze badges. (2022, July 5). ASP.NET core identity check isadmin. Stack Overflow. https://stackoverflow.com/questions/72875803/asp-net-core-identity-check-isadmin 

Cephalin. (2022, September 21). Tutorial: ASP.NET APP with Azure SQL database - azure app service. Tutorial: ASP.NET app with Azure SQL Database - Azure App Service | Microsoft Learn. https://learn.microsoft.com/en-us/azure/app-service/app-service-web-tutorial-dotnet-sqldatabase 

Ardalis. (2024a, June 17). Overview of ASP.NET core MVC. Microsoft Learn. https://learn.microsoft.com/en-us/aspnet/core/mvc/overview?view=aspnetcore-9.0&WT.mc_id=dotnet-35129-website 

Rummens, A. (2024, August 20). Azure SQL database: STEP-by-step setup and Management. DataCamp. https://www.datacamp.com/tutorial/azure-sql-database 

Tdykstra. (2024, September 18). Session in ASP.NET Core. Session in ASP.NET Core | Microsoft Learn. https://learn.microsoft.com/en-us/aspnet/core/fundamentals/app-state?view=aspnetcore-9.0 

 

GitHub. (n.d.). Adding a theme to your GitHub Pages site using jekyll. GitHub Docs. https://docs.github.com/en/pages/setting-up-a-github-pages-site-with-jekyll/adding-a-theme-to-your-github-pages-site-using-jekyll 

GitHub Pages. Markdown Guide. (n.d.). https://www.markdownguide.org/tools/github-pages/#:~:text=Just%20create%20a%20new%20repository,the%20Markdown%20support%20is%20excellent 

Jekyll themes. Jekyll Themes. (n.d.). http://jekyllthemes.org/ 

GitHub. (n.d.-b). Quickstart for GitHub Pages. GitHub Docs. https://docs.github.com/en/pages/quickstart 

 

Jamesmontemagno, erjain, Par, J., & Mairaw. (2022, April 12). Logical architecture versus physical architecture - .NET. .NET | Microsoft Learn. https://learn.microsoft.com/en-us/dotnet/architecture/microservices/architect-microservice-container-applications/logical-versus-physical-architecture 

 
SamMonoRT, AndriySvyryd, Anderson, R., bricelam, ajcvickers, smitpatel, roji, seekingtheoptimal, lajones, djcarter85, NikitaKrasnovSW, divega, mairaw, tdykstra, spottedmahn, & rowanmiller. (2024, November 12). Connection strings - EF core. EF Core | Microsoft Learn. https://learn.microsoft.com/en-us/ef/core/miscellaneous/connection-strings?tabs=dotnet-core-cli 

Banach, Z. (2024, December 16). How to prevent CSRF attacks by using anti-CSRF tokens. Invicti. https://www.invicti.com/blog/web-security/protecting-website-using-anti-csrf-token/ 

Rick-Anderson, timdeschryver, guardrex, tdykstra, GitHubPang, serpent5, v-haiboz, tryonelove, damienbod, nschonni, pranavkm, scottaddie, JvandeKraats, gyuwon, isaac2004, v-anpasi, rhires, & danroth27. (2024, October 14). Role-based authorization in ASP.NET Core. Microsoft Learn. https://learn.microsoft.com/en-us/aspnet/core/security/authorization/roles?view=aspnetcore-9.0 

Shah, N. (2025, February 26). Performance optimization techniques for ASP.NET Core Applications. Techcronus Tech Blog & Insights. https://www.techcronus.com/blog/performance-optimization-techniques-for-asp-net-core-applications/  

ions/ 
  

