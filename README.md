# Confluence Pipeline Steps Plugin (formerly "jenfluence")
Jenkins (workflow) plugin that is able to publish information on Atlassian Confluence pages.

Currently, the only feature is to create or retrieve a page via the Confluence REST API.

Our future plans are to extend the plugin so that only certain areas on a page can be updated or information can be inserted at specified markers. The deletion of pages and the publishing of other plugin data such as checkstyle, findbugs, javadoc or jacoco mark further milestones.

Legal notice:
All published trademarks and product names are property of their respective owners and may be claimed by a third party and are subject to the terms of use of the respective trademark laws and the ownership rights of the possessing party. Simply because they are named here, it cannot be concluded that trademarks are not protected through rights of a third party.
We fully respect these laws and these companies and acknowledge that prodct, company and service names may be published within our code and documents without further designation.


## How to deploy on Jenkins
### Method 1 (Jenkins UI)
1. Clone this project: `git clone https://github.com/Sprengnetter-Immobilienbewertung/jenfluence.git`
2. Execute `mvn clean package` to build the HPI file
3. Navigate **Manage Jenkins** &rarr; **Manage Plugins** &rarr; **Advanced** &rarr; **Upload Plugin**
4. Select the generated HPI file located in **jenfluence/target/confluence-pipeline-steps.hpi**
5. Click **Upload** to deploy the HPI file

### Method 2
1. Clone this project: `git clone https://github.com/Sprengnetter-Immobilienbewertung/jenfluence.git`
2. Execute `mvn clean package` to build the HPI file
3. Stop Jenkins
4. Copy the generated HPI file located in **jenfluence/target/confluence-pipeline-steps.hpi** to **$JENKINS_HOME$/plugins**
5. Start Jenkins
