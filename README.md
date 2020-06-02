# PHP Travels
This project covers 3 Testcases.
1.PHP Travels user registration
2.Login and Logout
3.Verify details page

We can trigger the test cases from TestRunner file. Go to this file. File location is: src/test/java/testRunner/TestRunner.java
To trigger: Right click, select Run As -> TestNG Test

To run in different env:
1.Go to end of the pom.file
2.Set the value for activeByDefault key as true in the corresponding env profile
3.Example, For SIT env:

<profile>
<activation>
<activeByDefault>true</activeByDefault>
</activation>
<id>sit</id>
<properties>
<env>sit</env>
</properties>
</profile>

Note: Build the project after updating this in pom file.

To run in different browser:
1.Set the value for browser key as chrome or firefox in the config.properties file
2.Example,
browser=chrome
(or)
browser=firefox
3.File location is: src/main/resources/config.properties


