Mutation testing example using
* JUnit 5
* piTest 1.2.2
* Maven

To generate mutation report from the command line:

`mvn test-compile org.pitest:pitest-maven:mutationCoverage`

Output will appear in target/pit-reports
View the report by opening the index.html 

Also confirmed working with the PIT Mutation Testing plugin in IntelliJ
https://plugins.jetbrains.com/plugin/7119-pit-mutation-testing

With the plugin you need to 
- Edit Configurations and add a PIT Runner config
- Edit that configuration to point target classes at `com.rocketnine.*`

Run the plugin via the Run button and the output link appears in a Mutation Report window.
Output location for the plugin appears in target/report