## Java (Programming Language)
Java is a high-level, class-based, object-oriented programming language that facilitates cross-platform application development through its write-once, run-anywhere approach. Known for its use in backend development, enterprise solutions, and Android app creation, Java's functionality stems from its conversion of code into bytecode for the Java Virtual Machine, and it was used to create the [best selling game of all time](https://en.wikipedia.org/wiki/Minecraft).

## Static Typing
Static typing in programming languages means that variable types are explicitly declared and determined at compile time, contrasting with dynamic typing where types are understood at runtime. This feature in Java enhances error detection during build and contributes to code reliability and efficiency.

## Tip #1: Prefer Static Typing
Embrace static typing in languages, including JavaScript (i.e. use Typescript), to mitigate a wide range of errors, leading to more robust and maintainable code.

*Choosing dynamic typing for a quick speed boost is like sprinting in flip-flops. It might feel fast at first, but you'll likely trip up in the long run!*

## Build Once, Run Anywhere
This Java principle signifies the ability to compile Java code, often into JAR files, which can be run on any device equipped with a Java Virtual Machine, regardless of the underlying architecture.

## Java Virtual Machine (JVM)
JVM is an engine that provides a runtime environment to execute Java bytecode. It is not limited to Java alone but also supports other languages compiled to Java bytecode, such as Kotlin and Scala.

## Java Ecosystem
Java's ecosystem is a significant selling point, comprising a vast array of tools, frameworks, and libraries, facilitating solutions for virtually any programming requirement.

## Java Runtime Environment (JRE)
JRE is a set of software tools used specifically for running Java applications.

## Java Development Kit (JDK)
JDK is a comprehensive suite for developing, compiling, and running Java applications, encompassing the JRE along with additional development tools.

## Kotlin
Kotlin is an advanced, more concise version of Java, offering true null safety. It is the preferred language for Android app development, promoting cleaner code and modern programming features.

## Tip #2: Prefer Kotlin for JVM-based Development
For new projects on the JVM, particularly in mobile development, Kotlin is the recommended choice due to its modern features and ease of use. 

## Tip #3: Use ChatGPT for Java Development Assistance
Utilize ChatGPT, especially the Plus/4.0 version, for guidance in Java coding, understanding best practices, and initial project setup. For JavaScript developers, ask for help in translating JavaScript functionalities into Java.

## JavaScript and Java Comparison
Despite their similar syntax, JavaScript and Java differ significantly; Java is statically typed with access modifiers, while JavaScript is dynamically typed.

## Java Integrated Development Environments (IDEs)

When it comes to Java IDEs, the landscape is dominated by tools like IntelliJ IDEA, Visual Studio Code, and Eclipse. IntelliJ IDEA, particularly its Community Edition, is a favorite among many Java developers for its strong capabilities and no-cost availability. It's widely regarded as the most powerful and efficient IDE for Java development.

Visual Studio Code, with the right extensions, can serve as a lightweight IDE for Java. Eclipse, another major player, is known for its extensive plugin system.

Choosing the right IDE is all about what works best for you. And if you're still coding Java in Vi or Emacs, that's a *bold* choice. 

## Tip #4: Use Homebrew for Installing Java on Mac
Homebrew, a package manager for Mac, simplifies the installation of software like the JDK, offering an efficient way to manage software installations and updates on macOS.

---

# Task One: Java HelloWorld Application
- Install JDK using Homebrew on macOS.
- Develop a HelloWorld program in Java that, when run, outputs "HelloWorld" to the console and then closes.
- Compile and run the program using `javac` and `java` commands.
- Verify the installed JDK version by running `java -version` and `javac -version` in the terminal.

## Tip #5: Java Version Compatibility
Be aware that Java code compiled with a newer JDK version cannot run on an older JRE. Always ensure compatibility between the development and runtime environments.

## Spring Boot
Spring Boot is a framework for building stand-alone, production-grade Spring-based applications with minimal effort. It simplifies the bootstrapping and development of new Spring applications.

## Spring Initializr
This tool is akin to create-react-app for React, but for Spring Boot. It streamlines the creation of new projects by generating a basic project structure with chosen dependencies like Spring Web. It helps avoid common setup errors in Java, making it a practical choice for efficiently initializing Spring Boot applications. It can be run from the commandline (when installed) or from the [website](https://start.spring.io).



## Java Coding Conventions
*Class Names and File Names*: In Java, the name of the public class must match the filename. This convention facilitates the organization and retrieval of code. For example, if your class is named MyClass, the filename should be MyClass.java.
*Package Names and Directories*: Package names should correspond to the directory structure where the files reside. This alignment ensures a coherent file system organization. For instance, a package named com.example.myapp should be found in a directory path /com/example/myapp/.
General Capitalization Standards:
- *Class Names*: Use CamelCase for naming classes, with the first letter of each word capitalized (e.g., MyJavaClass).
- *Method Names*: Method names should start with a lowercase letter and follow camelCase convention (e.g., myMethod()).
- *Variable Names*: Like method names, variable names should also start with a lowercase letter and follow camelCase (e.g., myVariable).
- *Constants*: Constants are typically defined using all uppercase letters with underscores to separate words (e.g., MAX_HEIGHT).

# Task Two: Java Spring Boot HelloWorld Web Server
- Setup an IDE and install Gradle via Homebrew.
- Create a Spring Boot application that displays "Hello World" on the main URL. Consider using the Spring Initializr website to quickly create a project skeleton. Make sure to add the 'Spring Web' dependency to your project.
- Define project dependencies with Gradle.
- Compile the application into a JAR file and run it.
- Verify the web server's functionality and terminate the server.

## Maven and Gradle
Maven and Gradle are build automation tools used in Java projects for dependency management and project compilation. In the NodeJS space, their equivalents are npm and Yarn.

## Tip #6: Prefer Gradle Over Maven
Gradle is almost always a better choice than Maven for JVM build automation, especially in larger projects. A key advantage of Gradle is its speed; it can be up to 10x faster than Maven (which helps a lot for other projects). This is due to features like incremental builds and build caching, which reduce unnecessary work. Gradle's build scripts are also more readable and concise, offering an easier and more efficient development experience.

## Tip #7: Pitch a switch from Maven to Gradle for Legacy JVM projects with slow build times

In situations where Maven builds in legacy projects start to slow down significantly, it's advisable to consider a switch to Gradle. This transition is particularly recommended when build times exceed 5 minutes. Gradle's efficiency in handling larger, more complex builds can substantially improve build times and overall project performance. This recommendation can be an important pitch to clients, highlighting a proactive approach to enhancing development efficiency in existing projects.

## Tip #8: Regularly Update Dependencies
Regularly updating dependencies in your Gradle or Maven project is crucial. Neglecting this can lead to security vulnerabilities, as seen in the [Equifax breach](https://en.wikipedia.org/wiki/2017_Equifax_data_breach).

## OpenAI API
The OpenAI API provides REST-based access to a wide range of AI functionalities, including but not limited to text generation. These capabilities can be seamlessly integrated into various applications.

## Tip #9: Explore with OpenAI API Playground
For hands-on experimentation with the OpenAI API, visit the [OpenAI API Overview](https://platform.openai.com/docs/overview). It's an excellent resource for trying out different prompts and settings before implementing them in your application.

## Tip #10: Verify REST Calls with curl
Familiarize yourself with using `curl` to quickly test REST API calls without writing calls. For example, to call the OpenAI API:
   ```bash
   curl https://api.openai.com/v1/engines/davinci-codex/completions \
     -H "Content-Type: application/json" \
     -H "Authorization: Bearer YOUR_API_KEY" \
     -d '{
       "prompt": "Translate the following English text to French: 'Hello, how are you?'",
       "max_tokens": 60
     }'
   ```

# Task Three: Java Web Application with OpenAI API Integration
- Set up OpenAI API access by visiting [OpenAI API Overview](https://platform.openai.com/docs/overview).
- Generate an OpenAI API key.
- Implement an application using Spring Boot to interact with the OpenAI API.
- Develop a feature allowing user input text to be sent to OpenAI, receiving and displaying the response.
- Ensure API keys are not stored in Java code or source control, but injected via environment variables.
- Add the project to your public GitHub repository, ensuring a comprehensive `README.md` is included, detailing the project setup and functionality.

## Tip #11: Securely Store Keys and Passwords
Never store passwords or API keys in plain source control management (SCM). Such practices can lead to security breaches. 

## Tip #12: Utilize Public GitHub for Code Snippets and Tech Spikes
Storing simple code snippets, examples, and conducting technology spikes on your public GitHub serves multiple purposes. It acts as a versioned backup, aids in self-promotion, and provides a quick reference for future use. Additionally, documenting tech spikes on GitHub showcases your exploratory work with new technologies or approaches, offering insights into your problem-solving process. This practice not only benefits you by creating a tangible record of your learning and experimentation but also demonstrates your proactive engagement with emerging technologies to the wider community.

## Tech Spike Challenge
For each new technology you're exploring, create a public GitHub project. Document your process with a README.md and include a GitHub Action for building the project. This approach not only showcases your exploratory work and findings but also gets you hands-on with CI/CD practices. It’s a great way to share what you’ve learned, practice good DevOps habits, and contribute to your professional growth. Embrace this challenge to continuously expand your tech toolkit in a visible, impactful way.

# Task Four: Adding DevOps Practices to Your Project
## Pre-Step: Create a new Spring Boot Application
- Before diving into DevOps practices, create a Spring Boot application:
- Go to [Spring Initializr](https://start.spring.io).
- Ensure you add the "Spring Web" dependency to your project for web application development.
- After generating the project, import it into IntelliJ IDEA or your preferred IDE and verify that it runs successfully.
- Add and commit this project to your Public GitHub repo. 
## Step 1 - Automated Builds
- Set up GitHub Actions by adding a `.github/workflows/build.yml` script in your repository.
- This script should define steps to run the Gradle wrapper and execute builds on every commit to the master branch.
## Step 2 - Build Failure Notification
- Configure notifications to a Microsoft Teams channel for build failures.
- Use GitHub secrets to securely store the webhook URL for MS Teams.
- Create an incoming webhook in MS Teams and link it to your GitHub Actions.
- Test the setup by committing a change that intentionally breaks the build, like adding gibberish to your Java file.
## Step 3 - GitHub Action Status Badge
- Add a status badge to your `README.md` to display the build status. This badge is automatically updated based on the latest build results.

## GitHub Actions
GitHub Actions offer agentless and containerized build environments, where build scripts are part of the application repository. This approach significantly lowers the entry barrier compared to traditional CI tools like Jenkins.

## Maven/Gradle Wrapper
These wrappers ensure that the correct version of the build script engine is used, regardless of what's installed on the build agent. It simplifies build processes and ensures consistency across environments.

## Pair Programming
Pair Programming is an agile software development technique where two programmers work together at one workstation. One, the driver, writes code while the other, the observer or navigator, reviews each line of code as it is typed in. The two programmers switch roles frequently. It's an alternative to slower pull request processes, facilitating real-time code review and collaboration.

## Tip #13: Incorporating Pair Programming
Incorporate Pair Programming into your development flow to expedite the code review process. If Pair Programming is utilized, you may skip the formal pull request or immediately approve it as part of the Pair Programming session. Make sure to document who you paired with in the story comments or in the pull request itself for transparency.
- *Deciding When to Pair Program*: Standups are an excellent time to decide on pair programming sessions. It's when you can discuss who needs support and align pairs based on the day's tasks.
- *Picking the Right Pair*: If you're struggling with a particular codebase, pair up with the person who wrote it. This direct transfer of knowledge is incredibly efficient.
- *Remote Pairing Options*: Although in-person pairing is ideal for its direct interaction, remote pairing is a viable option with tools like Visual Studio Code Live Share, Zoom, or Tuple. It ensures that geographical distance doesn't hinder the collaborative effort.
- *Focus and Productivity*: Pair programming naturally boosts focus. Each partner keeps the other on task, minimizing distractions and preventing the tendency to drift off into less productive activities.
- *Ego Aside*: Successful pair programming requires setting your ego aside. It's about learning and solving problems together. If someone is resistant to pairing, it could signal they're defensive about their code base, potentially hiding something, or simply unaware of their knowledge gaps due to the Dunning-Kruger effect. Pairing with them becomes even more crucial in these situations. Understanding phenomena like the [Dunning-Kruger effect](https://en.wikipedia.org/wiki/Dunning–Kruger_effect) and [Imposter Syndrome](https://en.wikipedia.org/wiki/Impostor_syndrome) is important for navigating these dynamics, promoting a culture of openness and continuous improvement.
- *A Valuable Tool*: Consider pair programming as a valuable tool in your development toolbox. It's not just about coding together; it's a practice that enhances code quality, team knowledge, and project momentum.

## Pair Programming Challenge
Challenge yourself and your team to try pair programming on your engagements. Set goals to pair program a certain number of times per week and reflect on the benefits and challenges. It's a practice that, when embraced, can significantly improve the development process and team dynamics. Encourage sharing experiences and tips within the team to make the most out of this collaborative approach.

## Incoming Webhook
An incoming webhook is a simple way to post messages from external sources into platforms like Microsoft Teams. It allows applications to send automated messages or updates into a Teams channel.

## Tip #14: Leverage Incoming Webhooks
Utilize incoming webhooks for quick alerts in DevOps processes, such as build failures or updates, in collaboration tools like MS Teams and Slack.

## Webhook Integration Challenge
Identify ways to implement webhooks back at client projects for real-time updates—think JIRA status, CI/CD outcomes, and more. It’s often easier to demonstrate the value of such integrations and ask for forgiveness than to seek permission. Dive in, set up those webhooks, and show how they can streamline project communication and efficiency.

## Tip #15: Monitor Dependencies with Webhooks
Use webhooks to automatically notify relevant teams when there are issues with APIs or dependencies they manage, enhancing cross-team communication and issue resolution.

*Nothing motivates a quick fix quite like a webhook-triggered rage icon popping up in your chat every time an API breaks. It's like a virtual 'fix-it' nudge!*

## Tip #16: Use Gradle/Maven Wrapper for Build Agents
Implement Gradle or Maven wrappers in your projects to ensure build agents don't require specific versions of Gradle or Maven, facilitating smoother builds.

## Tip #17: Incorporate CI/CD from Day One
Integrate Continuous Integration and Continuous Deployment (CI/CD) into your projects, personal or public, from the start. Set up build-on-commit with notifications.

*Setting up CI/CD is like leaving yourself a treasure map. When you return to a project after months, you'll find the 'X' marking 'how to build this thing.'*

## Tip #18: Notifications on New Broken Builds
Set up notifications for new broken builds in team projects. Encourage team members to promptly fix or rollback changes if the issue isn't resolved quickly. This practice fosters a culture of accountability and rapid response.

# Task Five: Tech Spike Pairing 

## MS Teams Bot Using Microsoft Bot Framework
Create a bot that responds with "Hello World" to any message in MS Teams, using C#, Java, Python, or JavaScript. Document the creation process and code on a public GitHub repo.

## Enhance GitHub Actions with OpenAI API
Extend GitHub Actions to analyze build failure messages using the OpenAI API for clearer insights, then forward that refined analysis to an MS Teams channel. Utilize GitHub secrets to safeguard the OpenAI API access key from exposure. Document the integration process and code on a public GitHub repo.

## Incoming Webhook Notification for Pull Requests
Set up an MS Teams alert via incoming webhooks when a new Pull Request is made, including the commit message in the notification. Explore using OpenAI API to review code diffs. Document on GitHub.

## Notifications to SMS Messages
Implement a system to send notifications to SMS using AWS SNS (or Azure equivalent), focusing on build statuses or alerts. Provide a detailed setup guide on GitHub. Test it with a demo of broken builds causing a person to get a text message. 

## Spring Boot Joke Web Application with Azure OpenAPI
Develop a Spring Boot app that returns jokes based on user-submitted topics, utilizing Azure OpenAPI for joke content. Include the project and setup guide on GitHub.

## GitHub Action for Web Project Deployment
Develop a GitHub Action that orchestrates the build and deployment of a web project to a cloud platform, such as Amazon Beanstalk, with the deployment ideally being handled by the build script (Maven or Gradle) itself rather than directly within GitHub Actions. This approach allows for easier local testing. Ensure the project and its deployment steps are well-documented on GitHub.

## Error Notification Integration with MS Teams for Web Applications
Implement MS Teams Incoming Web Notifications for a NodeJS or Java (Spring Boot) web application to alert on unknown, uncaught, or critical errors. Consider adding a button to your website that triggers such an error for testing purposes. Document the process, including how to set up the webhooks and error handling logic, on a public GitHub repo.
- Bonus: Extend the notification feature to catch and alert on browser-side JavaScript errors, offering a comprehensive monitoring solution across both server and client sides.

## Utilizing Microsoft Graph API for Calendar Operations
Explore the Microsoft Graph API to interact with Office 365 Calendar: Start by fetching your own availability for the current day. Then, as an advanced step, determine the first three available time blocks for a meeting between yourself and another person (given their full name, you'll need to resolve their user ID). Finally, implement functionality to book a meeting in the calendar based on availability. Choose your preferred programming language for this task, and document your process and findings on a public GitHub repository, showcasing your ability to integrate with Microsoft services and manage calendar data programmatically.


# Backlog of Topics

- **Product Ideation** (RAVL Toolbox) - insert AI buzzwords here (Lambda function for chunking / processing / summarizing .. large pdfs -- for Katie). 
- **Cloud Deployments and Overview**
  - Including Blue/Green and Zero-Downtime Deployments.
- **Cloud Deployment Styles**: Including Function as a Service (FaaS), Platform as a Service (PaaS), Kubernetes (K8S), Docker, AWS Fargate, and more.
- **Deploy Pipelines**
- **Efficient IDE usage** 
- **Automated Testing** - Unit-Testing, Parametirized Tests, JUnit, Spook, etc 
- **Artifact Versioning** -- include release versioning, hotfixing, cherrypicking, version endpoints, tracking stories with deploys, including GitHash (i.e. solving "what exaclty is deployed, what's in this build ")
- **Trunk based development** -- with WIP and feature toggling (implcit and explicit)
- **Data Stores** -- Cache / CDN / SQL / etc 
- **Exception Handling for Unknown Errors** -- combined with Webhook or Teams notifications or Email notificaitons 
- **Logging (including structured), Metrics, Tracing (trace-id), Alerting, Dashboards**
- **GitHub Platform Usage** -- i.e. using the whole suite 
- **Microsoft Teams Bots and Integration** -- seems like a cool option for RAVL toolcase. 
- **AI-Related Topics** -- because why not -- also how to augment OpenAI API with own data. 
- **Security** -- including authentication
- **Retrospectives:** -- as a tool to drive change at client 
- **Static Code Analysis** -- i.e. Sonar
- **Code Maintainability** -- including refactoring
- **Pair Programming** -- and alternative code peer review styles
- **Cloud-Native Development** -- mainly don't store local state 
- **Spring Boot** -- config, dependecy injection, logging, properties, actuator, etc
- **Anti-Patterns and Code Smells** -- i.e. reinventing the wheel, premature optimization,
- **Best Practices** -- YAGNI, DRY, Boy Scout Rule, etc
- **Agile, Lean, Extreme Programming** - Overview 
- **[Getting Things Done When You're only a Grunt](https://www.joelonsoftware.com/2001/12/25/getting-things-done-when-youre-only-a-grunt/)**
- **To Be Announced (TBA)**
- **Do a Hackathon**

