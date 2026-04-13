# Modernization

* Understand
    * Functionality
    * Architecture - ARCHITECTURE.md
    * Versions in detail - ARCHITECTURE.md
    * Evolution of the Java ecosystem
* Identify modernization opportunities and create a prioritized plan - MODERNIZATION.md
    * Update the plan with branching
    * Update the plan with more detail if necessary.
    * Create Github issues for each item in the plan
    
* Start executing the modernization plan
    * Implement an issue or two, update GitHub issues
    * Run compilations
* Summarize where we are
    * Create ppt with status from GitHub

## What does this app do?

Ask mode 

```
What's the purpose of the @refarch-jee-customerorder/ application and who are the users? Read subdirectories and files in the application. Summarize in under 200 words.
```

## Whats the architecture and design?

Advanced mode - for write access.

```
Explain the architecture of @/refarch-jee-customerorder/ like I just joined the team. Start with a mermaid diagram of component dependencies with components grouped into layers of the app. Show external dependencies - anything that would execute outside of the app server. Include an ER diagram for the database and brief descriptions of the key tables. Write findings to ARCHITECTURE.md and keep it brief - not more than 300 lines.
```

## Detailed analysis of versions used

```
Analyze all .pom files in @refarch-jee-customerorder/ and report on Java and Java EE versions. Add a table of findings to ARCHITECTURE.md with each (eg. CustomerOrderServices), javaee dependency version and scope (eg provided), and target versions for the maven-compiler-plugin. 
```

## How has the Java language and ecosystem evolved since this app was written? 

Advanced mode

```
Generate a mermaid timeline diagram with major Java releases from Java 8 to Java 26 grouped by year. State release month and LTS status together with a summary of 3 JEPS / JSRs with significant new functionality for each release. Save the diagram as a .png file.
```

```
Add the Java EE releases and descriptions of added functionality to the timeline and regenerate the png. Start with Java EE 7.
```

## Identify modernization opportunities

Plan mode

```
Analyze the codebase in @/refarch-jee-customerorder/ and identify modernization opportunities for upgrading to Java 21 and moving to Quarkus 3.3 on OpenShift. Divide the analysis into 2 sections:

Section 1: Framework and architecture modernization for the target Quarkus runtime. Examples:

- Application server or vendor specific extensions used and suggestions for replacing them
- Replacing JNDI lookups with CDI
- Panache / Hibernate replacing of EJBs

Section 2: Language level modernization and mechanical changes. Opportunities to introduce Java language features introduced after JDK8. Limit to:

- Records instead of POJOs
- Text blocks to simplify string concatenation
- Switch expressions 

Create a analysis report in markdown format MODERNIZATION.md - be brief and assume that an experienced Java developer is the target audience. The report should contain a list of all identified modernization opportunities and a prioritized plan for how to address them. Important: limit the analysis to 300 lines. Clearly call out anything that requires manual review.
```

```
Update the plan, I want to start with upgrading to Java 21 in the current codebase across all POMs, then I want to convert the @Address class to be a record.
```

```
Create github issues for the steps so we can keep track of progress. Use the github mcp and create them in the original repo.
```

```
Implement issue # - assign it to me first
```

```
Use the Github MCP server to list all repo issues (also closed ones) and summarize the work sofar in a powerpoint file - use the powerpoint skill.
```

# Closing

Across the SDLC, Bob makes you faster, while you stay in control.