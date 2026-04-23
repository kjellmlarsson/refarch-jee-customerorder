# Understand

Ask mode 

```
What's the purpose of the @refarch-jee-customerorder/ application and who are the users? Read subdirectories and files in the application. Summarize briefly.
```

## Whats the architecture and design?

Advanced mode

```
Explain the architecture of @/refarch-jee-customerorder/. Start with a mermaid diagram of component dependencies with components grouped into layers of the app.
Write findings to ARCHITECTURE.md and keep it brief, assume that the reader is an experienced Java developer
```

```
Add an ER diagram for the database and brief descriptions of the key tables.
```

```
Are there any unit tests we can run?
```

## Detailed analysis of versions used

```
Analyze all .pom files in @refarch-jee-customerorder/ and report on Java and Java EE versions. Add a table of findings to ARCHITECTURE.md with each (eg. CustomerOrderServices), javaee dependency version and scope (eg provided), and target versions for the maven-compiler-plugin. 
```

# Identify modernization opportunities and create plan

Plan mode

```
Analyze the codebase in @/refarch-jee-customerorder/ and identify modernization opportunities for upgrading to Java 21 and moving to Quarkus 3.3 on OpenShift. Divide the analysis into 2 sections:

Section 1: Framework and architecture modernization for the target Quarkus runtime. Examples:

- Application server or vendor specific extensions used and suggestions for replacing them
- Moving to from javax to jakarta namespaces
- Replacing JNDI lookups with CDI
- Panache / Hibernate replacing of EJBs

Section 2: Language level modernization and mechanical changes. Opportunities to introduce Java language features introduced after JDK8. Limit to:

- Records instead of POJOs
- Text blocks to simplify string concatenation
- Switch expressions 

Create a analysis report in markdown format MODERNIZATION.md - be brief and assume that an experienced Java developer is the target audience. The report should contain a list of all identified modernization opportunities and a prioritized plan for how to address them.
```

```
Update the plan, I want to start with upgrading to Java 21 in the current codebase across all POMs, then I want to convert the @Address class to be a record.
```

# Start executing the modernization plan

```
Execute the first step of the modernization plan. 
```