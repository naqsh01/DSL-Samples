# DSL Templates - Master Components

DSL templates for creating master components for application components that can be deployed and undeployed on application servers such as JBoss, WebLogic, and IIS.

## Prerequisites ##

  1. The required application server plugin should be installed on the **ElectricFlow** server.
    * JBoss           - **EC-JBoss**
    * IBM WebSphere   - **EC-WebSphere**
    * Microsoft IIS   - **EC-IIS7**
    * Oracle Weblogic - **EC-Weblogic**
    * Tomcat          - **EC-Tomcat**
    * IIS             - **EC-IIS7**
  
  2. The **EC-FileSysRepo** is assumed to be pre-installed on the **ElectricFlow** server.
  
  3. Repository for **EC-FileSysRepo** plugin should contain WAR file, that will be deployed to Java application servers (**JBoss**, **WebLogic** or **WebSphere**). For IIS Web server repository should contain zipped archive of Web Application that will be deployed.

## Instructions ##

1. Edit the template file for your choosen application server replacing the parameter values with the desired values.

2. Run the following command to execute the updated DSL template.
 `ectool evalDsl --dslFile <file-path>`
 
3. You should now have the Master Component created or updated in **ElectricFlow** under **Applications -> Master Components** that can be used to create applications for deployment. 