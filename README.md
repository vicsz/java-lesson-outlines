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

## Tip #12: Utilize Public GitHub for Code Snippets
Storing simple code snippets, examples, and technology spikes on your public GitHub serves three key purposes: it acts as a versioned backup, aids in self-promotion, and provides a quick reference for future use.

# Task Four: Adding DevOps Practices to Your Project
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

## Incoming Webhook
An incoming webhook is a simple way to post messages from external sources into platforms like Microsoft Teams. It allows applications to send automated messages or updates into a Teams channel.

## Tip #13: Leverage Incoming Webhooks
Utilize incoming webhooks for quick alerts in DevOps processes, such as build failures or updates, in collaboration tools like MS Teams and Slack.

## Tip #14: Monitor Dependencies with Webhooks
Use webhooks to automatically notify relevant teams when there are issues with APIs or dependencies they manage, enhancing cross-team communication and issue resolution.

*Nothing motivates a quick fix quite like a webhook-triggered rage icon popping up in your chat every time an API breaks. It's like a virtual 'fix-it' nudge!*

## Tip #15: Use Gradle/Maven Wrapper for Build Agents
Implement Gradle or Maven wrappers in your projects to ensure build agents don't require specific versions of Gradle or Maven, facilitating smoother builds.

## Tip #16: Incorporate CI/CD from Day One
Integrate Continuous Integration and Continuous Deployment (CI/CD) into your projects, personal or public, from the start. Set up build-on-commit with notifications.

*Setting up CI/CD is like leaving yourself a treasure map. When you return to a project after months, you'll find the 'X' marking 'how to build this thing.'*

## Tip #17: Notifications on New Broken Builds
Set up notifications for new broken builds in team projects. Encourage team members to promptly fix or rollback changes if the issue isn't resolved quickly. This practice fosters a culture of accountability and rapid response.

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
- **AI-Related Topics** -- because why not 
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

