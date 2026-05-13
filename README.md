# TestMu AI-Maven-Tunnel — TestMu AI (Formerly LambdaTest)

![TestMu AI Logo](https://www.testmuai.com/resources/images/selenium-parallel-testing-index.png)

---

### Prerequisites

1. Maven is required to be installed:
   https://maven.apache.org/install.html

### Environment Setup

1. Global Dependencies
   - Install [Java8](https://www.oracle.com/technetwork/java/javase/downloads/jdk8-downloads-2133151.html)
2. TestMu AI Credentials

   - Set TestMu AI username and access key in environment variables. It can be obtained from [TestMu AI dashboard](https://automation.lambdatest.com/)  
     example:

   * For linux/mac

   ```
   export LT_USERNAME="YOUR_USERNAME"
   export LT_ACCESS_KEY="YOUR ACCESS KEY"

   ```

   - For Windows

   ```
   set LT_USERNAME="YOUR_USERNAME"
   set LT_ACCESS_KEY="YOUR ACCESS KEY"

   ```

3. Setup
   - Clone [maven-tunnel-sample](https://github.com/LambdaTest/maven-tunnel-sample.git) from GitHub.
   - Navigate to the cloned directory
   - Compile maven dependencies
   ```
   $ mvn compile
   ```

##### Routing traffic through your local machine

- Set tunnel value to `true` in test capabilities
  > OS specific instructions to download and setup tunnel binary can be found at the following links.
  >
  > - [Windows](https://www.testmuai.com/support/docs/display/TD/Local+Testing+For+Windows)
  > - [Mac](https://www.testmuai.com/support/docs/display/TD/Local+Testing+For+MacOS)
  > - [Linux](https://www.testmuai.com/support/docs/display/TD/Local+Testing+For+Linux)

### Important Note:

Some Safari & IE browsers, doesn't support automatic resolution of the URL string "localhost". Therefore if you test on URLs like "http://localhost/" or "http://localhost:8080" etc, you would get an error in these browsers. A possible solution is to use "localhost.lambdatest.com" or replace the string "localhost" with machine IP address. For example if you wanted to test "http://localhost/dashboard" or, and your machine IP is 192.168.2.6 you can instead test on "http://192.168.2.6/dashboard" or "http://localhost.lambdatest.com/dashboard".

### Running Tests

- To Start Test:

  - Navigate to maven-tunnel-sample
  - Run following command

  - To run single test
    `mvn test -DsuiteXmlFile=MavenSingle.xml`

  - To run parallel tests
    `mvn test -DsuiteXmlFile=MavenParallel.xml`

### Note: You can also mention your TestMu AI credentials in env/default.properties file

## 🚀 LambdaTest is Now TestMu AI

👋 Welcome to TestMu AI, the next evolution of LambdaTest. As of January 2026, [LambdaTest is Now TestMu AI](https://www.testmuai.com/lambdatest-is-now-testmuai/) - we have evolved from a cross-browser testing cloud into a unified, AI-native quality engineering platform designed for the modern DevOps era.

Whether you have been part of the LambdaTest community for years or are just discovering TestMu AI, our mission remains the same: to help you ship faster with high-scale test execution, autonomous testing, and deep quality analytics.

**🔄 Our Rebrand Journey**

We chose the name TestMu AI to reflect our shift towards intelligent, autonomous testing. While our identity has changed, our core technology and commitment to the testing community stay the same.

👉 Find [LambdaTest's New Home](https://www.testmuai.com/).

**🔭 Explore TestMu AI**

The same infrastructure LambdaTest customers relied on, now delivered through autonomous AI agents.

- [KaneAI](https://www.testmuai.com/kane-ai/)
- [Agent-to-Agent Testing](https://www.testmuai.com/agent-to-agent-testing/)
- [HyperExecute](https://www.testmuai.com/hyperexecute/)
- [Real Device Cloud](https://www.testmuai.com/real-device-cloud/)
- [Pricing](https://www.testmuai.com/pricing/)
- [Documentation](https://www.testmuai.com/support/docs/)