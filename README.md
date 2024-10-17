# **Build and Automation Tools:**
## Maven

### Maven Labs

1. **Introduction to Maven Basics**
   - **Objective**: Understand the basics of Maven and how it manages dependencies and builds.
   - **Tasks**:
     - Install Maven on your system.
     - Create a basic Maven project using the `mvn archetype:generate` command.
     - Explore the generated `pom.xml` and understand its structure (dependencies, plugins, etc.).
     - Build the project using `mvn compile` and `mvn package` commands.

2. **Managing Dependencies in Maven**
   - **Objective**: Learn how to manage project dependencies using Maven's `pom.xml`.
   - **Tasks**:
     - Add a third-party library (e.g., JUnit) to your Maven project by modifying the `pom.xml`.
     - Resolve transitive dependencies and check the dependency tree using the `mvn dependency:tree` command.
     - Remove and re-add dependencies to see how Maven handles version conflicts.

3. **Building and Packaging a Java Application**
   - **Objective**: Use Maven to build and package a Java application into a `.jar` file.
   - **Tasks**:
     - Create a simple Java application that prints "Hello Maven!".
     - Modify the `pom.xml` to package the application into a runnable `.jar` file using the Maven `jar` plugin.
     - Execute the built `.jar` using `java -jar`.

4. **Using Maven Plugins for Automation**
   - **Objective**: Automate common tasks using Maven plugins.
   - **Tasks**:
     - Add plugins to the `pom.xml` for tasks like:
       - Code formatting (`maven-checkstyle-plugin`).
       - Running tests automatically (`maven-surefire-plugin`).
       - Deploying the project to a Maven repository (`maven-deploy-plugin`).
     - Run the configured plugins using the `mvn` commands (e.g., `mvn checkstyle:check`).

5. **Multi-Module Maven Project**
   - **Objective**: Understand how to manage multi-module projects with Maven.
   - **Tasks**:
     - Create a parent Maven project with two child modules (e.g., a library module and an application module).
     - Set up the `pom.xml` to include dependencies between the modules.
     - Build all modules together and ensure they interact correctly.

6. **Custom Maven Build Profiles**
   - **Objective**: Learn how to set up custom build profiles in Maven for different environments.
   - **Tasks**:
     - Modify the `pom.xml` to create different build profiles (e.g., `dev`, `test`, and `prod`).
     - Adjust the build settings and dependencies in each profile.
     - Build the project using different profiles (`mvn package -P dev`, etc.).

7. **Continuous Integration with Maven**
   - **Objective**: Automate builds and deployments using a CI tool (e.g., Jenkins or GitLab CI/CD) and Maven.
   - **Tasks**:
     - Set up a CI pipeline that automatically triggers a Maven build and test on code push.
     - Configure Maven to upload artifacts to a Maven repository or deploy them to an application server as part of the pipeline.

