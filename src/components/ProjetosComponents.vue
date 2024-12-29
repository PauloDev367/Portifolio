<template>
  <div class="area-data">
    <template v-for="(data, index) in projetos" :key="index">
      <div
        class="card-project"
        data-toggle="modal"
        :data-target="`#modalProjeto${index}`"
      >
        <img
          :src="require(`../assets/images/projetos/${data.caminho_img}/1.png`)"
          alt="Foto capa"
        />
        <div class="infos">
          <h3>{{ data.titulo }}</h3>
        </div>
      </div>
    </template>
  </div>

  <template v-for="(data, index) in projetos" :key="index">
    <div
      class="modal modal-projeto fade"
      :id="`modalProjeto${index}`"
      tabindex="-1"
      role="dialog"
      :aria-labelledby="`modalProjeto${index}Label`"
      aria-hidden="true"
    >
      <div class="modal-dialog modal-dialog-centered modal-lg" role="document">
        <div class="modal-content">
          <div class="modal-header">
            <h5 class="modal-title" :id="`modalProjeto${index}Label`">
              {{ data.titulo }}
            </h5>
            <button
              type="button"
              class="close"
              data-dismiss="modal"
              aria-label="Close"
            >
              <span aria-hidden="true">&times;</span>
            </button>
          </div>
          <div class="modal-body">
            <div
              :id="`carouselprojeto${index}`"
              class="carousel slide"
              data-ride="carousel"
            >
              <div class="carousel-inner">
                <div
                  class="carousel-item"
                  v-for="img in data.total_img"
                  :key="img"
                  :class="img == 1 ? 'active' : ''"
                >
                  {{ img }}
                  <img
                    class="d-block w-100"
                    :src="
                      require(`../assets/images/projetos/${data.caminho_img}/${img}.png`)
                    "
                    alt="First slide"
                  />
                </div>
              </div>
              <a
                class="carousel-control-prev"
                :href="`#carouselprojeto${index}`"
                role="button"
                data-slide="prev"
              >
                <span
                  class="carousel-control-prev-icon"
                  aria-hidden="true"
                ></span>
                <span class="sr-only">Previous</span>
              </a>
              <a
                class="carousel-control-next"
                :href="`#carouselprojeto${index}`"
                role="button"
                data-slide="next"
              >
                <span
                  class="carousel-control-next-icon"
                  aria-hidden="true"
                ></span>
                <span class="sr-only">Next</span>
              </a>
            </div>

            <div class="infos">
              <div v-html="data.texto"></div>
            </div>
          </div>
        </div>
      </div>
    </div>
  </template>
</template>

<script setup>
import { ref } from "vue";

const projetos = ref([
  {
    titulo: "Development of an Online Store with ERP Integration",
    texto: `
        <p>I developed an online store for Araújo Pneus, a well-established company in the tire and automotive accessories segment in northern Brazil, using the ISet platform. The project included the implementation of essential features such as:</p>

        <ul>
        <li>Secure and diverse payment methods.</li>
        <li>Delivery configuration with multiple options to cater to different locations.</li>
        <li>Order registration and management system.</li>
        <li>Organization and display of products in categories, optimizing the user experience.</li>
        <li>Additionally, I implemented a Backend for Frontend (BFF) to integrate the client’s ERP system with the online store. This component automates the synchronization of critical data such as inventory and prices through a cronjob executed every 10 minutes. During this process, data is validated and updated efficiently, ensuring the consistency and accuracy of the information displayed on the e-commerce platform.</li>
        </ul>

        <p>This solution provided a smoother and more integrated operation, reducing manual efforts and optimizing the management of the online store.</p>
    `,
    total_img: 7,
    caminho_img: "araujoecom",
  },
  {
    titulo: "Development of a Platform for Managing Pre-Owned Vehicles and CRM",
    texto: `
        <p>I developed a customized platform for Brenner Veículos, a well-known company in the automotive sector in Rio Grande do Sul. The project was built using Laravel and Blade technologies, with a focus on providing an elegant, functional, and efficient solution to meet the client’s specific needs.</p>
        <p>The main features of the platform include:</p>

        <ul>
        <li>Pre-Owned Vehicle Management: An intuitive interface that allows the client to easily register, update, and manage their portfolio of vehicles.</li>
        <li>SEO Best Practices Page: Created to optimize visibility on search engines, enhancing organic reach and attracting more qualified visitors.</li>
        <li>Integrated CRM: A compact contact management system with:</li>
        <li>Interactive Dashboard: Providing an overview of interactions and key metrics.</li>
        <li>Detailed Contact Listing: A dedicated area to organize and view potential customer information in a structured and efficient way.</li>
        </ul>

        <p>This solution not only enhanced Brenner Veículos' digital presence but also facilitated internal management and customer service, aligning technology with the company’s growth strategies.</p>
    `,
    total_img: 11,
    caminho_img: "brennerseminovos",
  },
  {
    titulo: "Ticket Management Platform with Support Integration",
    texto: `
        <p>I developed a robust platform using Laravel (for the API) and Vue.js (for the frontend), designed to meet the needs of ticket management and technical support.</p>
        <p>The main features of the system include:</p>

        <ul>
        <li>
        Ticket Registration: Allows customers to register multiple tickets for support requests, ensuring efficient communication with the responsible team.
        </li>

        <li>
        Asynchronous Email Notifications: Implemented with Laravel queues, ensuring that notification emails are sent without impacting the user experience when creating a ticket.
        </li>
  
        <li>
        Chat for Ticket Interactions:
        <li>While not real-time (suitable for tickets requiring longer response times), the chat offers a practical way for communication between the customer and support.</li>
        <li>Interactions are dynamically updated on the interface, providing a clear and organized tracking of the ticket history.</li>
        </li>
        </ul>
        
        <p>This solution was designed to combine functionality and performance, offering a smooth experience for customers while facilitating organization and support team efficiency.</p>
    `,
    total_img: 12,
    caminho_img: "chamados",
  },
  {
    titulo: "Complete Inventory and Financial Management System",
    texto: `
        <p>I developed an integrated management system using .NET 6.0 for the backend and Vue.js for the frontend, designed to meet the needs of companies looking to control their operations efficiently and centrally.</p>
        <p>The main features of the system include:</p>

        <ul>
        <li>
            Inventory Management:
            <li>Easy and detailed registration and management of products.</li>
            <li>Full control over stock movements to streamline organization and replenishment.</li>
        </li>
        
        <li>
            Financial Management:
            <li>Modules to record and track the purchase and sale of products and services.</li>
            <li>Control of accounts payable and receivable, providing a clear view of the financial flow.</li>
        </li>
        
        <li>People Management: Organization of customer, supplier, and employee information in a unified database.</li>
        <li>Email Notifications: Automation of notifications for relevant updates, ensuring quicker communication.</li>
        </ul>
        
        <p>This solution stands out for combining advanced tools for operational and financial management, delivering an integrated, reliable, and efficient experience for users.</p>
    `,
    total_img: 15,
    caminho_img: "controleestoque",
  },
  {
    titulo: "Complete CRM System for Managing Clients and Leads",
    texto: `
        <p>I developed a comprehensive CRM system using Laravel for the backend and Vue.js for the frontend, designed to optimize the management of clients and leads, offering an all-encompassing view and integrated features.</p>
        <p>Key Features:</p>

        <ul>
            <li>
                Interactive Dashboard:
                Provides an overview of a selected client’s information, with the ability to easily switch between clients using a selectpicker.
            </li>
            
            <li>
                Lead Summary:
                A dedicated page that displays a consolidated overview of all registered leads, segmented by:
                Google campaigns.
                Phone leads (Leadfone).
                Meta campaigns (Facebook/Instagram).
                These data are collected and integrated through APIs I developed, which extract information from third parties and update the system in real time.
            </li>
            
            <li>
                Detailed Lead Management:
                A specific screen to view all leads, presenting detailed information for each one.
                Leads can be downloaded and exported to spreadsheets, making it easier for external analysis and data sharing.
            </li>
            
            <li>
                User Management:
                Full administration of users (clients and administrators), with control over permissions and access.
            </li>
        </ul>
        
        
        <p>This solution combines a modern and functional interface with powerful data integrations, providing the company with an essential tool to manage clients and leads efficiently and strategically.</p>
    `,
    total_img: 6,
    caminho_img: "crmluma",
  },
  {
    titulo: "Contact Management System for the São Paulo Forum",
    texto: `
        <p>I developed a customized system for the IBM team, in partnership with the São Paulo Forum, using Laravel and Blade. The system was designed to manage contacts from the website, providing a practical and secure solution for handling leads and optimizing decision-making.</p>
        <p>Key Features:</p>

        <ul>
        <li>
            Lead Management:
            <li>Ability to accept or reject registered clients directly within the system.</li>
            <li>Record of personalized comments for each lead, making follow-ups easier and improving the evaluation process.</li>
        </li>

        <li>Action History: Detailed logging of who accepted or rejected each client, ensuring transparency and traceability of actions taken.</li>
        <li>Lead Reevaluation: A feature that allows rejected leads to be retrieved, offering the opportunity for reevaluation and potential conversion into clients.</li>

        </ul>
        <p>This solution was developed with special attention to security and privacy, reflected, for example, in hiding forms in screenshots. The system stands out by providing the team with an organized and efficient way to manage and analyze leads, ensuring greater control over the contacts received.</p>
    `,
    total_img: 10,
    caminho_img: "ibmcf2forum",
  },
  {
    titulo: "Registration and Payment Management System for a Business Event",
    texto: `
        <p>I developed a customized system for the Meta and Integrare teams, designed to manage registrations and payments for a business event held in São Paulo. Using Laravel and Blade, the solution combines advanced features with an elegant and intuitive interface.</p>
        <p>Key Features:</p>

        <ul>


        <li>
            Custom Landing Page:
            <li>Created for promoting and registering clients interested in the event.</li>
            <li>Refined and functional design to attract and engage visitors.</li>
        </li>

        <li>
            Integration with Mercado Pago:
            <li>Configuration of the payment method to generate and send the payment link directly to the client's email after approval in the system, as requested by the client.</li>
        </li>
        
        <li>
            Registration Management:
            <li>Ability to accept or reject registered clients based on specific criteria.</li>
            <li>Robust filtering system by CNPJ and email, ensuring accuracy in categorizing and distributing clients by sector and category.</li>
        </li>
        
        <li>
            Overview and Registration Analysis:
            <li>A detailed listing showing the total number of registrations in each category, segmented into accepted, rejected, and pending analysis.</li>
        </li>
        
        <li>
            Discount Coupon Creation:
            <li>A tool to generate promotional coupons, facilitating customized payment conditions and encouraging greater participation in the event.</li>
        </li>
        </ul>
        
        <p>This system was developed to provide an optimized experience for both organizers and participants, integrating technology and efficiency in a strategic business environment.</p>
    `,
    total_img: 10,
    caminho_img: "mcmmeta",
  },
  {
    titulo: "Development of Interactive Minigames for BASF Event",
    texto: `
        <p>I developed two interactive minigames for a BASF event using Laravel and Blade. The games, Memory Game and Puzzle, were created to provide a fun and engaging experience for participants, with an interface adapted for various devices.</p>
        <p>Key Features:</p>

        <ul>
        <li>Interactive Games: Memory Game and Puzzle with drag-and-drop functionality for desktop devices.</li>
        <li>Full support for touch devices, such as those used at the event, with touch events for smooth and intuitive interaction, perfect for touchscreen TVs.</li>
        <li>Challenge Timer: Each minigame features a timer that adds excitement and competitiveness, encouraging players to complete challenges within the allotted time.</li>
        <li>If time runs out, the game resolves automatically, ending the challenge fairly.</li>
        <li>Display of Final Time: At the end of each minigame, the time taken to complete the game is shown, providing players with immediate feedback on their performance.</li>
        </ul>
        
        <p>This system was designed to ensure a dynamic and engaging experience, leveraging interactive technologies to meet the BASF event's requirements, where direct screen interaction and the excitement of a time-limited challenge created a thrilling and memorable gaming environment.</p>
    `,
    total_img: 6,
    caminho_img: "minigamesmcm",
  },
  {
    titulo: "Mini Real Estate Portal for RE/MAX Franchises",
    texto: `
        <p>I developed a mini real estate portal using Laravel and Blade, focused on the sale and management of properties for RE/MAX franchises. The system combines an elegant interface with intuitive features to simplify navigation and the process of purchasing and managing properties.</p>
        <p>Key Features:</p>

        <ul>
        <li>Homepage with Featured Properties: The homepage showcases a selection of featured properties with an attractive design that grabs users' attention.</li>
        <li>A preview of other available properties is also displayed, making navigation easier and helping users make their choice.</li>
        <li>Property Details: Each property has a dedicated page with detailed information, including photos and full descriptions, providing a clear and comprehensive view for potential buyers.</li>
        <li>Property Registration and Management: Enables the registration and management of new properties directly on the platform, making it easy to input and update information.</li>
        <li>Properties can be organized into categories, offering an efficient filter for users to find properties based on their preferences.</li>
        </ul>

        <p>This portal was designed to provide a visually appealing and functional experience, allowing RE/MAX franchises to manage their properties effectively and enabling customers to easily find what they are looking for.</p>
    `,
    total_img: 10,
    caminho_img: "miniportal",
  },
  {
    titulo: "Phone Leads Management System (Leadfones)",
    texto: `
        <p>I developed a Leadfones management system using Laravel for the backend and Vue.js for the frontend. This system was designed to facilitate the management of phone leads from a third-party provider, offering an intuitive and efficient platform for administrators and clients.</p>
        <p>Key Features:</p>

        <ul>
        <li>Leadfones Viewing: Users can view all the registered Leadfones of a specific client in a clear and organized manner, providing easy access to information.</li>
        <li>CSV Export: It is possible to download the registered Leadfones in a .csv file, making it easier to analyze externally or share data.</li>
        <li>User Management: The system allows the registration and management of users, with the ability to create admins and clients, ensuring access control based on the user's profile.</li>
        </ul>

        <p>This solution provides a simple and efficient way to manage phone leads, with an intuitive design and practical features, ensuring that Leadfone data is easily accessible and manipulable for the responsible team.</p>
    `,
    total_img: 2,
    caminho_img: "painelleadfone",
  },
  {
    titulo: "Custom Photo Editing System for Pipefy Event",
    texto: `
        <p>I developed a system using CodeIgniter 3 for the Pipefy team, created for an internal company event. The platform was designed to allow employees to customize their photos in a simple and fun way, with the option to add customized Pipefy backgrounds and icons, promoting team interaction and engagement.</p>
        <p>Key Features:</p>

        <ul>
        <li>Photo Registration and Editing: Employees can register on the platform and edit their photos, personalizing them with Pipefy's exclusive backgrounds and icons. The interface was developed to be intuitive and easy to use, allowing everyone to participate without difficulty.</li>
        <li>Save and View Edits: All edits made by users can be saved, allowing employees to access their personalized photos at any time.</li>
        <li>Photo Wall: The platform displays a wall with all the photos created by the team, allowing everyone to view the edits made by colleagues.</li>
        <li>Image Download: Each image can be downloaded individually, making it easy to share the photos with others outside the platform.</li>
        </ul>
        
        <p>This system was created to foster fun and interaction among Pipefy employees while providing an easy way to personalize and share images within the team. The solution was fully adapted to the event, offering a seamless and personalized experience for the users.</p>
    `,
    total_img: 5,
    caminho_img: "pipefy",
  },
  {
    titulo: "Report Sending System for Clients - Singel Engenharia",
    texto: `
        <p>I developed a comprehensive system using Laravel and Blade for Singel Engenharia, focused on sending reports to clients in an organized and efficient manner. The platform offers an intuitive folder management system and a robust structure for sending and receiving large files, ensuring a smooth experience for both administrators and clients.</p>
        <p>Key Features:</p>

        <ul>
        <li>Report Management with Folders: The system allows administrators to organize reports into folders, similar to Google Drive, ensuring easy navigation and organization of documents.</li>
        <li>Folder Administration: Administrators can view all registered clients and their respective reports, as well as reorder folders as needed, ensuring efficient organization.</li>
        <li>Sending Reports and Notifications: The system utilizes chunk upload for sending large files, ensuring that reports are sent securely and without interruptions.</li>
        <li>Jobs and queues are used to send notifications at scale, both to users and administrators, ensuring communications are efficient and do not overload the system.</li>
        <li>Client Access: Clients can access their created folders, view the reports sent, and download the files as needed. The interface was designed to be simple and intuitive, allowing clients to quickly find the documents they need.</li>
        </ul>

        <p>This system was developed to provide an efficient and scalable solution for Singel Engenharia, ensuring that reports are sent and accessed quickly and organized, with an intuitive interface for both administrators and clients.</p>
    `,
    total_img: 13,
    caminho_img: "singelrelatorios",
  },
  {
    titulo: "Feedback Collection System for Businesses",
    texto: `
        <p>I developed a feedback collection system using Laravel on the backend and Vue.js on the frontend. The platform was designed to facilitate the collection of customer reviews about specific companies or employees, providing an efficient way to gather and manage customer feedback.</p>
        <p>Key Features:</p>

        <ul>
        <li>Sending Reviews: The system features a simple and intuitive interface where customers can easily submit reviews, either about the company as a whole or about a specific employee, offering flexibility for collecting more detailed feedback.</li>
        <li>Review Management: Administrators can view, manage, and analyze all received reviews, enabling efficient management of customer feedback.</li>
        <li>Reviews can be exported in spreadsheet format (e.g., .csv), making it easy to analyze and process the collected data.</li>
        <li>User Management: The system provides complete user management, allowing administrators to register, remove, update, and list all employees and admins registered on the platform.</li>
        </ul>
        <p>This system offers a robust and easy-to-use solution for businesses that want to collect and manage customer feedback while ensuring efficient administration of system users. The user-friendly interface and ability to export data make the platform a powerful tool for enhancing the customer experience and optimizing internal management.</p>
    `,
    total_img: 9,
    caminho_img: "sistemadefeedbacks",
  },
  {
    titulo:
      "Freelancer System for the Scientific Initiation Congress - FEPI 2024",
    texto: `
        <p>I developed a system for freelancers using .NET 8 on the backend and Vue.js on the frontend as part of the Scientific Initiation Congress at the FEPI University of Higher Education in Itajubá in 2024. The platform was built with a robust hexagonal architecture, aimed at providing scalability and lower cost per request, when compared to a microservices architecture.</p>
        <p>Key Features:</p>

        <ul>
        <li>Service Registration and Management: Clients can register new services, manage existing ones, and send proposals directly to service providers, streamlining communication and interaction between both parties.</li>
        <li>Service Provider Registration: Service providers can register on the platform, manage proposals they've sent, and submit new proposals directly to clients, ensuring efficient and agile communication and negotiation.</li>
        <li>Hexagonal Architecture: The use of hexagonal architecture ensures the system is easily scalable, maintaining an efficient and cost-effective structure. This contributes to ongoing maintenance and evolution as the system grows.</li>
        </ul>        
        
        <p>This system was developed to facilitate the connection between clients and freelancers, optimizing the service registration and proposal negotiation process. The chosen architecture provides high performance and flexibility, making the platform ready to handle the growing demand of users, whether in managing services or exchanging proposals between clients and service providers.</p>
    `,
    total_img: 18,
    caminho_img: "sistemadefreelancers",
  },
  {
    titulo: "Personal Finance Management System - .NET 8.0 and Vue.js",
    texto: `
        <p>I developed a personal finance management system using .NET 8.0 for the backend and Vue.js for the frontend. The goal of this system is to allow users to manage their personal finances effectively, by recording expenses and income from one or more bank accounts, providing complete control over spending and earnings.</p>
        <p>Main Features:</p>

        <ul>
        <li>Bank Account Registration: The system allows users to register multiple bank accounts, making it easier to track finances from different sources of income or expenses. Users can switch between accounts to view specific information.</li>
        <li>Expense and Income Entries: Users can quickly and easily enter their expenses and income, enabling efficient daily financial tracking. The platform includes categories to help organize transactions.</li>
        <li>Bank Account Overview: On the home page, users can view an overview of the spending for a specific bank account, with graphs and details about the balance and the financial trend over time.</li>
        <li>Entry Registration and Listing: Users can register and view expenses and income for specific months and years tied to a specific account. Entries can be filtered by category, date, and type of transaction (expense or income).</li>
        <li>Mini Dashboard: A mini dashboard provides a quick overview of monthly entries, allowing users to see totals for expenses and income and track their financial balance. Graphs and summaries assist in visualizing the data.</li>
        <li>Mobile-Focused: The platform is optimized for mobile devices, ensuring an intuitive and responsive interface. This allows users to manage their finances smoothly on smartphones or tablets, providing flexibility in managing their finances anywhere.</li>
        </ul>
        
        <p>This system offers users complete control over their personal finances with a simple and clear interface for managing their expenses and income. The quick data visualization and mini dashboard features make the platform a valuable tool for organizing finances in a practical and efficient way.</p>
    `,
    total_img: 11,
    caminho_img: "sistemadegestaofinanceira",
  },
  {
    titulo: "Ticket Sales System - Laravel and Vue.js",
    texto: `
        <p>I developed a ticket sales system using Laravel for the backend and Vue.js for the frontend. The purpose of this system is to provide a simple and efficient platform for selling tickets to concerts, allowing registered customers to purchase tickets via credit card or PIX (a popular Brazilian instant payment method).</p>

        <p>Main Features:</p>

        <ul>
        <li>Ticket Purchase: Registered customers can purchase tickets for concerts quickly and easily, with payment options available through credit card or PIX.</li>
        <li>Show Registration and Management:Administrators can register and manage shows, including details such as event date, time, location, and ticket prices, ensuring all event information is kept up to date.</li>
        <li>Admin Dashboard: The admin dashboard provides an overview of ticket sales, with insights into tickets sold, shows listed, and other relevant data. It enables administrators to manage events and track sales efficiently.</li>
        <li>Sales History: The system includes a comprehensive list of all ticket sales, displaying transaction details such as customer information, number of tickets purchased, and the payment method used.</li>
        <li>Ticket Management: Administrators can view a list of all tickets, with the ability to filter between active and inactive tickets. This makes it easier to manage and control available tickets for events.</li>
        <li>Responsive Interface: The platform offers a smooth and intuitive experience with an interface that adapts to both desktop and mobile devices, enabling customers to purchase tickets from anywhere.</li>
        </ul>
        
        <p>This system provides full control over ticket sales, allowing administrators to manage shows and sales effectively, while customers can securely and conveniently purchase tickets. The detailed sales tracking and ticket management features make the platform ideal for event companies and concert organizers.</p>
    `,
    total_img: 14,
    caminho_img: "sistemadeingressos",
  },
  {
    titulo: "Real-Time Voting System - .NET 8.0 and Vue.js with SignalR",
    texto: `
        <p>I developed a real-time voting system using .NET 8.0 for the backend, Vue.js for the frontend, and SignalR for real-time communication. The system allows instant interaction between clients and administrators, making the voting process dynamic and efficient.</p>
        <p>Main Features:</p>
        <ul>
        <li>Real-Time Voting Submission: Clients can cast their votes for candidates and see the progress of the voting in real time, without needing to refresh the page. SignalR ensures that all participants see the updates instantly.</li>
        <li>
            Administrator Voting Management: Administrators have complete control over the voting process, including the ability to:
            <ul>
                <li>Pause or reopen the voting at any time.</li>
                <li>Reset the votes to restart the process if needed.</li>
                <li>Announce the winner as soon as the voting ends.</li>
        
            </ul>
        </li>
        <li>View online users and votes registered up to that point, ensuring transparency in the process.</li>
        
        <li> Real-Time View: The system dynamically updates vote statuses and partial results, allowing all participants to monitor the vote count and progress in real time.</li>
        <li> Interactive and Intuitive Interface: Developed with Vue.js, the system features a modern and user-friendly interface that delivers real-time updates, ensuring a smooth experience for both users and administrators.</li>
        <li> Vote Tracking: The system offers a detailed view of who has voted and who is online, with the vote count being updated as participants cast their votes, all in real time.</li>
        </ul>
        <p>Additional Features:</p>
        <ul>

        <li>Scalability: The use of SignalR ensures that the system can handle large numbers of users voting simultaneously without sacrificing performance.</li>
        <li>Security and Reliability: The platform guarantees the accuracy and security of votes, with session management to prevent fraud and ensure integrity.</li>

        </ul>

        <p>This real-time voting system is ideal for events, internal elections, and interactive processes that require immediate feedback from participants. It combines cutting-edge technology with user experience to ensure a fair, transparent, and efficient voting process.</p>
    `,
    total_img: 11,
    caminho_img: "sistemadevotos",
  },
  {
    titulo: "Online Raffle Sales System - Laravel and Blade",
    texto: `
    <p>
      This online raffle sales system was developed using Laravel and Blade, combining a modern and robust architecture with optimized features for lottery and ticket sales.
    </p>

    <h3>Key Features:</h3>
    <h5>Administrator Raffle Management:</h5>
    <ul>
      <li>
        <strong>Raffle Registration:</strong>
       
      <ul>
        <li>
            Configure new raffles with details such as:
            <li>Draw date.</li>
            <li>Price per ticket.</li>
            <li>Cover photo to enhance appeal.</li>
            <li>Prizes available for winners.</li>
            <li>Automatic purchase buttons for user convenience.</li>
          </li>
      </ul>
      </li>
    </ul>
    
    <ul>
      <li>
        <strong>Raffle Ticket Generation and Management:</strong>
        <ul>
        <li>Support for up to 1 million numbered tickets generated in a sequence of six pairs.</li>
        <li>Use of Jobs and Queues for efficient ticket generation and processing, ensuring data integrity and scalability.</li>
        </ul>
      </li>
    </ul>
    
    <ul>
      <li>
        <strong>Purchase Processing and Notifications:</strong>
        <li>
          Automated Email Notifications:
          <ul>
          <li>Emails sent automatically for:</li>
          <li>Successful purchase confirmation.</li>
          <li>Winner announcements after the draw.</li>
          </ul>
        </li>
      </li>
    </ul>
    
    <ul>
      <li>
        <strong>Postgres Database:</strong>
        <li>
          Chosen for its:
          <ul>
          <li>Robustness in handling large data volumes (e.g., numbered tickets).</li>
          <li>Security to protect financial and user information.</li>
          </ul>
        </li>
      </li>
    </ul>
    
    <ul>
      <li>
        <strong>Dockerized Development Environment:</strong>
        <li>
          The system is configured to run in Docker containers, ensuring:
          <ul>
          <li>A standardized development environment.</li>
          <li>Ease of deployment and testing.</li>
          </ul>
        </li>
      </li>
    </ul>
    
    <h3>System Benefits:</h3>
      <ul>
        <li>
          Scalability:
          <ul>
          <li>Designed to handle large volumes of raffles and users while maintaining high performance.</li>
          </ul>
        </li>
      </ul>
      
      <ul>
        <li>
          <strong>Security and Reliability</strong>
          <ul>
          <li>PostgreSQL ensures data integrity.</li>
          <li>Jobs and Queues prevent failures during intensive task processing.</li>
          </ul>
        </li>
      </ul>
    
      <ul>
        <li>
          <strong>User Experience:</strong>
          <ul>
          <li>Elegant and intuitive interface for both administrators and participants.</li>
          <li>Automated notifications keep users informed at every stage.</li>
          </ul>
        </li>  
      </ul>
    
      <ul>
        <li>
          <strong>Flexibility:</strong>
          <ul>
          <li>Easy raffle and ticket management with customization options for different events.</li>
          </ul>
        </li>
      
      </ul>
    
    <p>
      This online raffle system is an ideal solution for administrators seeking to organize lotteries efficiently, offering secure processing and an enjoyable experience for both participants and organizers.
    </p>
    `,
    total_img: 23,
    caminho_img: "rifas",
  },
]);
</script>
