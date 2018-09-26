# my-maven-archetypes
Source code of the custom archetypes for creating different seeds, like Springboot, spring boot JAXRS, Spring boot with JAX-RS and Spring-JPA etc..

# 1. Clone this git repository using the command 
`git clone git@github.com:rkiranchowdhary/my-maven-archetypes.git`

# 2. Build and update archetype to your local repository using the commands
`cd my-maven-archetypes/springbootrest-hello-archetype`

`mvn install archetype:update-local-catalog`

# 3. Run the crawl command to update the catalog
`mvn archetype:crawl`

# 4. You can use this architype to create your maven project using below command
`cd ../../ `

`mvn archetype:generate -DarchetypeCatalog=local -DinteractiveMode=false -DarchetypeGroupId=com.myarchetype -DarchetypeArtifactId=springbootrest-hello-archetype -DarchetypeVersion=0.9 -DgroupId=<your-group-id> -DartifactId=<your-project-id>`
