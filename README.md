# Guarantee Vault Platform Automation Tests
- execute test with a specific profile(ex: Chrome):
``mvn clean install -Pchrome
``

- execute tests based on specific tags(ex. @regression) and parallel running on 3 threads
  ``mvn clean install -Dtags=@Regression -DparallelCount=3
  ``
- execute multiple test based on different tags and 3 threads with headless profile:
``mvn clean install -Dtags=@E2E,@Regression -DparallelCount=3 -Pheadless``

- execute multiple test based on different tags and 3 threads with headless profile:
  ``mvn clean install -Dtags=@Regression1 -DparallelCount=8``


- generate allure report:
``allure serve /c/Work_Projects/e2e-ui-tests/target/allure-results``




OBSOLETE:

``mvn clean install  -Dcucumber.options="--plugin io.qameta.allure.cucumber4jvm.AllureCucumber4Jvm --tags @Regression"
``