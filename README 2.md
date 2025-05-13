# Complete_Adobe_Commerce_Guide
complete adobe commerce(magento guide) - https://developer.adobe.com/commerce/php/development/roadmap/


Technology used for Magento(adobe commerce)
-------------------------------------------
<details><summary><b>tech stack : - </b></summary>
    - Php 
    - Html
    - Css
    - Javascript
    - Knockout JS
    - Xml
    - Jquery
    - 
 </details>  

Best Practices - no comparmise
------------------------------
### alway's remind - before start development
<details><summary><b>info</b></summary>
               
                 - Before Code - Understood what is the Requirement
                 - Some Time Directly Try - If you are not gettting 
                 - Always Try with Dummy Value then Implement Real
                 - Implement Oops Concept
                            |
                            |--- Divide code into small methods 
                            |--- Write Clean Code (Proper Naming )
                            |--- 
                 -  Avoid the Deprecated Code
                 -  Always follow vendor code and DevDocs
                 -  Re-test the Scenario (twice )
                 -  Optimize the Code (Best Way)
                 -  Debug & Debug (Xdebug | Read Online | Logs | Hacks)
    
 </details>  
 
### Print Logs
<details><summary><b>info</b></summary>
  
          $writer = new \Zend\Log\Writer\Stream(BP . '/var/log/mylogfile.log');
          $logger = new \Zend\Log\Logger();
          $logger->addWriter($writer);
          $logger->info('This Is Simple Text Log'); //To print simple text log
          $logger->info(print_r($myarray, true)); //To print array log  
 
</details>  

 ### exception handling
<details><summary><b>infp</b></summary>
    
             try { echo 'Perferom your Operation'; } catch(Exception $e) { echo 'Message: ' .$e->getMessage(); }
               try {
                   //check if
                     var $test = "TEST";
                     if(($test) === "TEST") {
                     //throw exception if condition is not valid
                     throw new customException($test);
                 }
                  //check for "TEST" in dummy value
                   if(strpos($test, "TEST") !== FALSE) 
                   {
                    throw new Exception("$test is an example Dummy Value");
                  }
                 }
                 catch (customException $e) {
                    echo $e->errorMessage();
                    }
                 catch(Exception $e) {
                  echo $e->getMessage();
                }  
  </details>

### Setup coding standards
<details><summary><b>Setup coding standards</b></summary>
    
              Step - 1
              --------
                         - Install the coding-standard folder   --- https://developer.adobe.com/commerce/php/coding-standards/
                                           |
                                           |
                                           |------------------ direct folder
                                           |
                                           |------------------ install via composer way
    
              Step - 2
              --------
                        - Install(keep) folder any directory location
    
                        - Here i kept under directory location i.e -  /var/www/html/coding-standards
    
                        - cd /var/www/html/coding-standards   ---- composer install
    
    
              Step -3
              -------
                       - use below command to check the coding standard
    
                       - vendor/bin/phpmd /var/www/html/marina/app/code/Codilar/CustomApi/ text /var/www/html/marina/dev/tests/static/testsuite/Magento/Test/Php/_files/phpmd/ruleset.xml
                       
                       - vendor/bin/phpcs --standard=Magento2 --extensions=php /var/www/html/marina/app/code/Codilar/CustomApi/
                       
                       - php src/php-cpd/phpcpd.phar --fuzzy /var/www/html/marina/app/code/Codilar/CustomApi/
                    
     
</details> 

### Debug untill fix - no matter what
<details><summary><b>info</b></summary>
    
</details>  
     
</details>   

History of Magento(Adobe Commerce)
----------------------------------
<details><summary><b>info</b></summary>
    
</details>  


## Tools Require 
<details><summary><b>info</b></summary>
    
       - Nginx
       - Apache
       - Php
       - Elasticsearch
       - OpenSearch
       -  Redish
       - Varnish
       - RabbitMQ
       - Xdebug
     
</details>        
        
Adobe Training Docs & Syllabus
------------------------------      
<details><summary><b>info: </b></summary>
    
### Ground Level
----------------
<details><summary><b>info: </b></summary>
    
    - How magento is taking memory.
            |-------From Which File Magento Code get Executed
            |-------How i can find particular route in magento by folder(code) structure way internally
            |-------Why magento keep this much folder 
            |-------Explain all the folder present in magento and their uses
            |-------If we delete some of the folder then what happen if not then why 
                            |-------Based on Which mechanism magento is Working
                            |-------What all concept magento is implementing  and When




   

             - Use of Elasticsearch. why magento use elasticsearch
                                                 |--------what is elasticsearch
                                                 |--------advantage of elasticsearch
                                                 |--------how elasticsearch work internally
                                                 |--------It is necessary to use elasticsearch
                                                 |--------If We need to change anything in elasticsearch then how can we change 
                                                 |--------Which port it is taking and how it detect the port 
                                                 |-------Why anyone choose elasticsearch
                                       
  
              - Use of Varnish. Why magento use varnish
                                         |--------what is varnish
                                         |--------advantage of varnish
                                         |--------how varnish work internally
                                         |--------It is necessary to use varnish
                                         |--------If We need to change anything in varnish then how can we change 
                                         |--------Which port it is taking and how it detect the port 
                                         |-------Why anyone choose varnish
  
              - Use of Redis . Why magento use Redis
                                      |--------what is Redis
                                      |--------advantage of Redis
                                      |--------how Redis work internally
                                      |--------It is necessary to use Redis
                                      |--------If We need to change anything in redis then how can we change 
                                      |--------Which port it is taking and how it detect the port
                                      |-------Why anyone choose redis 



                   - How to Know In Which File or Which Mechanism Magento Configure Varnish, Redis and Elasticseaerch along with Php
                                                        |
                                                        |-------How Varnish and Redis is Related with Cache and Indexing
                                                        |-------Is it mandotory to use varnish and redis at the same time for magento if yes then Why 
                                                                                         
                                                                                        
                                    
       

                 - What all Application Mode in Magento
                                 |-------By default which application mode magento have 
                                 |-------How to know which application mode we will use and When
                                 |-------What advantage we will get by Application Mode
                                 |-------Is it Helpfull for  Magento 
                               

                - What is Indexing
                            |----------------What are all Indexing mode in magento
                            |----------------How Indexing is Usefull for Magento
</details>

   
###  PHP
--------

    <details><summary><b>info: </b></summary>
           PHP
           ===
            |------ How Php code get executed
            |------ Php is a which type of language compiled or interpreted
            |------ Difference between Compiled and Interpreted Language
            |------ Functional Programming vs Object oriented 
            |------ What all mechanishm Php follow for better Performance Result
            |------ What are all the Step Require to Compile the Php Code
            |------ What is Opchace Mechanism in Php
            |------ What JIT concept in Php and Where it Require
            |------ What is the use of Zend Engine in Php
            |------ What all file contain Zend Engine
            |------ What is the Difference between Zend Engine and Zend Framework
            |------ What is the use of PEAR and PECL
            |------ What is the use of Auto_load() method in Php
            |------ Why any one need to use namespaces in Php
            |------ What are all magic method Present in Php and what is magic method
            |
            |------------------OOPS
            |                    |------What is Class
            |                    |                |------variable
            |                    |                |          
            |                    |                |------constructor
            |                    |                |             |------default
            |                    |                |             |------parameterized
            |                    |                |------methods
            |                    |                
            |                    |------What is Object
            |                    |                |--------what is state 
            |                    |                |--------what is behaviour
            |                    |                |--------what is identity
            |                    |------What is Methods
            |                    |                |--------final and static method
            |                    |------What is Variables
            |                    |                 |-------What all variable Scope in Php
            |                    |-------What is Abstraction
            |                    |                    |-----------What is abstract class
            |                    |                    |-----------What is abstract method 
            |                    |                    |-----------Explain exact rule to implement abstraction concept in Php
            |                    |-------What is Encapsulation
            |                    |                      |--------Explain the encapsulation by giving proper code representation
            |                    |-------What is Inheritance
            |                    |                   |---------How many types of inheritance support by Php
            |                    |                   |---------What is the use of Traits in Php
            |                    |-------What is Polymorphisim
            |                    |                     |----------compiled time(static)or(overloading)
            |                    |                     |----------run time(dynamic)or(overriding)
            |                    |
            |                    |-------What is Interface in Php
            |                    |                    |---------------Explain complete implementation of Interface
            |                    |------What is the Difference betweeen Interface and Abstraction  
            |
            |-------------What are all Access Specifier in Php
            |                                      |-------------What is Public and its Scope
            |                                      |-------------What is Protected and its Scope
            |                                      |-------------What is Private and its Scope
            |
            |
            |-----comming soon......
            
    </details>


### Magento Fundamentals Part-1
-------------------------------

    <details><summary><b>info: </b></summary>
        
              Unit-1 Fundamentals of Magento Development pt-1
              -----------------------------------------------
    
                                    - Video Intro
                                    - Using the Player
                                    - Introduction
                                    - Approach Audience
                                    - Course Content
                                    - Best Way to Take the Course
                                    - Unit One Home Page
    
              Preparation
              -----------
                              - Preparation | Module Topics
                              - Preparation | LAMP $ Composer
                              - Preparation | Magento2 Installation
                              - Video :Install Magento part1
                              - Video :Install Magento part2
                              - Video :Install Magento part3
                              - Video :Install Magento part4
            Overview $ Architecture
            -------------------------
                            - Magento 2 Overview & Architecture | Module Topics
                            - Magento 2 Platform & Architecture Platform
                            - Magento 2 Platform & Architecture | Architecture
                            - Magento 2 Platform & Architecture | Areas
                            - Magento 2 Platform & Architecture | Magento 2 Essentials
                            - Magento 2 Platform & Architecture | Components
                            - Magento 2 Platform & Architecture | Paths
                            - Magento 2 Platform & Architecture | File Types
                            - Magento 2 Platform & Architecture | Config Files
                            - Magento 2 Platform & Architecture | PHP Classes
                            - Magento 2 Platform & Architecture | Development Process
                            - Magento 2 Platform & Architecture | Enable Custom Code
                            - Magento 2 Platform & Architecture | Modules
                            - Modules | Location
                            - Modules | Naming a Module 
                            - Modules | Registering a Module/Empty Module Structure
                            - Modules | module.xml
                            - Modules | module.xml Example
                            - Modules | registration.php
                            - Modules | Module Dependencies
                            - Modules | Types of Module Dependencies
                            - Modules | Module Dependencies Tasks
                            - Reinforcement Exercise 1.3.1:Modules
    
    
               File System
               -----------
                            - File System | Module Topics
                            - File System | Root Folders
                            - File System | App Folder Contents 
                            - File System | Framework & Core Modules
                            - File System | Core Source Code
                            - File System | Framework Source Code
                            - File System | Module Structure
                            - File System | Module View File Types
                            - File System | Templates
                            - File System | Templates(expanded)
                            - File System | Themes
                            - File System | Static Files
                            - MULTIPLE CHOICE QUESTION
    
               Development Operations
               ----------------------
    
                                              - Development Operations | Module Topics
                                              - Modes | Modules in Magento2
                                              - Modes | Developer Mode in Magento 2 
                                              - Modes | Production Mode in Magento 2 
                                              - Modes | Default Mode in Magento 2 
                                              - Modes | Summary of Mode Features
                                              - Modes | Maintenance Mode in Magento 2 
                                              - Modes | Specifying a Mode : Environment Variable
                                              - Modes | Specifying a Mode : Web Server Environment
                                              - Modes | Specifying a Mode : php-fpm Environment
                                              - Video : Magento Modes
                                              - Reinforcement Exercise 1.5.1:Mode
                                              - Command-Line Interface | Magento 2 CLI
                                              - Cache | Cache in Magento 2 
                                              - Cache | Cache Type
                                              - Cache | Cache Cleaning
                                              - Reinforcement Exercise 1.5.2:Cache
                                            
                   DI & Object Manager
                   ------------------ 
                  
                                              - DI & Object Manager  | Modules Topics 
                                              - Dependency Injection | DI Pattern
                                              - Dependency Injection | Overview
                                              - Reinforcement Exercise 1.6.1:Dependency Injection
                                              - Dependency Injection | Class Instantiation in Magento 2
                                              - Dependency Injection | Different Classes Instantiation
                                              - Object Manager
                                              - Object Manager | Shared Instances Concept
                                              - Object Manager | Object Manager Usage
                                              - Object Manager | Magento 2 Best Practice
                                              - Object Manager | Auto-generated Classes
                                              - Object Manager | Configuration
                                              - Object Manager Configuration | Specification
                                              - Object Manager Configuration | Preferences Example
                                              - Object Manager Configuration | Argument Example
                                              - Object Manager | Configuration Shared Argument Example
                                              - Video : Dependency Injection
                                              - Reinforcement Exercise 1.6.2: Object Manager
                                              - Check Your Understanding(1.6.B)
                                              
                                              
                                        
                    Plugins
                    -------
                                            - Plugins | Module Topics
                                            - Plugins | Defination
                                            - Plugins | Customizations
                                            - Declare a Plugin
                                            - Plugin Example | Before-Listener Method
                                            - Plugin Example | After-Listener Method
                                            - Plugin Example | Around-Listener Method
                                            - Prioritizing Plugins
                                            - Configuration Inheritance & Plugins
                                            - Plugins | Interception
                                            - Reinforcement Exercise 1.7.1: Plugins 1
                                            - Reinforcement Exercise 1.7.2: Plugins 2
                                            - Check Your Understanding 
                                            - Check Your Understanding
                                        
    
                  Events
                  ------
    
                                            - Events | Module Example
                                            - Events | Defination
                                            - Events | Schema
                                            - Events | Core Example: Saving an Order Process
                                            - Demo | Registering an Event
                                            - Reinforcement Exercise 1.8.1:Events
                                            
                                            
                                            
                                          
                    Module Configuration
                    --------------------
                                           - Module Configuration | Module Topics 
                                           - Configuration Files Overview
                                           - Configuration Files: Application Configuration
                                           - Configuration Files: Modules's Configuration
                                           - Configuration Files: Merging Config Files
                                           - Configuration Files | Storage
                                           - Configuration Files | core_config_data
                                           - Configuration Files | Backend System Config Page
                                           - Configuration Files | Scope
                                           - Configuration Files | Merging
                                           - Configuration Files | Validation
                                           - Video : XSD Schema
                                           - Error Reporting Settings | Overview
                                           - Check Your Understanding(1.9.1:Module)
                                           - Reinforcement Exercise 1.9.1: Module Configuration
                                           - End of Unit One
      
       </details>
     
### Magento Fundamentals Part-2
-------------------------------

    <details><summary><b>info: </b></summary>
      
          1.1  Introduction to UI Components
    
                    - UiComponent Overview
                    - UiComponent Definition
                    - UiComponent & Block Comparison
                            
          1.2 Architecture and Configuration
      
                   - Architecture 
                   - Configuration
                      
         1.3 Templates and Rendering
    
                   - Templates
                   - Rendering
     
         1.4 JavaScript Role in UiComponents
    
                   - JavaScript in UiComponent Overview
                   - Executing of UiComponents
      
         2.1 Introduction to Grids
    
                  - Grids Overview
                  - Listing UiComponent
                  - DataSource
                  - Columns
                  - Filters
                  - Mass Actions
                  - Grid Indexer
                  - Paging
                  
         2.2  Intriduction to Forms
      
                  - Forms Overview
                  - Form Components
                  - Form Fieldsets
                  - Form Elements 
      </details>
 
 
  

### Cloud for Adobe Commerce
----------------------------

    <details><summary><b>info: </b></summary>
        
                         - Overview
                         - Onboarding tasks
      Architecture
    
                         - Starter architecture
                         - Starter develop and deploy workflow
                         - Pro architecture
                         - Pro develop and deploy workflow
                         - Scaled architecture
                         
      Technologies and requirements
    
                          - Composer
                          - magento-cloud CLI
                          - ece-tools package
                          - Git
                          - SSH and sFTP
                          - PrivateLink
                          - New Relic
                          - SendGrid 
                          
      Manage your project
    
                          - Configure your project
                          - Project structure
                          - Manage user access
                          - Enable MFA for SSH
                          - Manage branches with the Interface
                          - Manage branches with the CLI
                          - Manage disk space
                          - Monitor performance
                          - View logs
                          - Snapshots and backup management
                          - Restore an environment
                          - Profile database queries
                          
       Local development setup
    
                           - Prepare for manual setup
                           - Install prerequisites
                           - Enable SSH keys
                           - Set up the file system owner
                           - Clone and branch the project
                           - Install Commerce
                           - First time deployment
                           - Optional - Configure Xdebug
                           - Optional - Install sample data
                           
       Cloud Docker development
    
                      Install
                          - Additional tools for file synchronization
                          - Upgrade
                      Use Docker
                            - Production mode
                            - Developer mode
                      Configure and manage
                            - Configuration sources
                            - Manage the database
                            - Manage cron jobs
                            - Set up multiple websites or stores
                            - Xdebug for Docker
                            - Extend Docker
                            - Add Blackfire.io service
                     Docker container architecture
                             - Service containers
                             - CLI containers
                     Functional Testing
                             - Application testing
                             - Cloud code testing for Commerce
                             - Docker quick reference
                             - Get support for Cloud Docker
      Integrations
    
                   - Bitbucket integration
                   - GitHub integration
                   - GitLab integration
                   - Health notifications
                   
      Import existing code into a project
    
                   - Prepare your existing system
                   - Import code
                   
      Configure your store
    
                   - Best practices for store configuration
                   - Set up PayPal
                   - Set up B2B
                   - Set up cron jobs
                   - Set up multiple Cloud websites or stores
                   - Install, manage, and upgrade modules
                   - Install a theme
                   - Import URL Rewrites
                   
      Configure Fastly services
    
                   - Set up Fastly
                        - Customize cache configuration
                        - Customize error and maintenance pages
                   - Web Application Firewall
                   - Image Optimization
                   - Custom VCL snippets
                        - Reroute requests to a CMS backend
                        - Block referral spam
                        - IP allow list
                        - IP block list
                        - Bypass Fastly cache
                   - Fastly troubleshooting
                   
      Configure environments
    
                   - Application
                       - Properties
                       - Variables
                       - PHP application
                       - Workers
                       - Set cache for static files
                   - Build and deploy
                       - Set up notifications
                       - Logging handlers
                   - Routes
                        - Caching
                        - Redirects
                        - Server side includes
                   - Services
                        - Set up MySQL service
                        - Set up Redis service
                        - Set up Elasticsearch service
                        - Set up OpenSearch service
                        - Set up RabbitMQ service
                   - PHP (php.ini)
                   - Environment variables
                        - ADMIN variables
                        - Global variables
                        - Build variables
                        - Cloud variables
                        - Deploy variables
                        - Post-deploy variables
                        - Working with variables
                        
      Configuration management for store settings
    
                   - Example of managing system-specific settings
                   
      Optimize deployment
    
                   - Cloud deployment process
                   - Scenario-based deployment
                   - Zero downtime deployment
                   - Static content deployment
                   - Smart wizards
                   
      Deploy your store
    
                   - Deployment process
                   - Continuous deployment
                   - Protective block
                   - Build and deploy on local
                   - Prepare to deploy to Staging and Production
                   - Deploy code and migrate static files and data
                   - Test deployment
                   - Error message reference for ece-tools
                   
      Site launch
    
                   - Launch checklist
                   - Launch steps
                   
      Troubleshooting
    
                   - Component deployment failure
                   - Add site map and search engine robots
                   
      Upgrades and patches
    
                   - Update ece-tools
                   - Apply patches
                   - Upgrade version
                   - Upgrade project
                   
      Release notes
    
                   - ece-tools
                   - Cloud Patches for Commerce
                   - Cloud Docker for Commerce
                   - Cloud Components for Commerce
                   - Backward incompatible changes
        
        
        
               Cloud overview --> https://devdocs.magento.com/cloud/bk-cloud.html
               
               Onboarding --> https://devdocs.magento.com/cloud/onboarding/onboarding-tasks.html
               
               Architecture --> https://devdocs.magento.com/cloud/architecture/cloud-architecture.html
               
               Pro vs Started --> https://devdocs.magento.com/cloud/architecture/starter-architecture.html
               
               Pro vs Started --> https://devdocs.magento.com/cloud/architecture/pro-architecture.html
               
               Technical Requirements --> https://devdocs.magento.com/cloud/requirements/cloud-requirements.html
               
               Magneto CLI --> https://devdocs.magento.com/cloud/reference/cli-ref-topic.html
               
               ECE Tool --> https://devdocs.magento.com/cloud/reference/ece-tools-reference.html
               
               Private Link --> https://devdocs.magento.com/cloud/project/privatelink-service.html
               
               SSH --> https://devdocs.magento.com/cloud/env/environments-ssh.html
               
               NewRelic --> https://devdocs.magento.com/cloud/project/new-relic.html
               
               SendGrid --> https://devdocs.magento.com/cloud/project/sendgrid.html
               
               Cloud Project Structure --> https://devdocs.magento.com/cloud/project/sendgrid.html
               
               Fastly --> https://devdocs.magento.com/cloud/cdn/cloud-fastly.html
               
               Configure Application --> https://devdocs.magento.com/cloud/project/magento-app.html
               
               Build and Deploy --> https://devdocs.magento.com/cloud/project/magento-env-yaml.html
               
               Services Configuration --> https://devdocs.magento.com/cloud/project/services.html
               
               PHP Configuration --> https://devdocs.magento.com/cloud/project/magento-app-php-ini.html
               
               Environment Variable --> https://devdocs.magento.com/cloud/env/variables-intro.html
               
               All Type of Variable --> https://devdocs.magento.com/cloud/env/variables-intro.html
               
               Zero Down time deployment --> https://devdocs.magento.com/cloud/deploy/reduce-downtime.html
               
               Go Live Checklist --> https://devdocs.magento.com/cloud/live/site-launch-checklist.html
               
               Upgrade --> https://devdocs.magento.com/cloud/project/project-upgrade-parent.html 
            
     </details>
     
 </details>  
            

Magento Core Concept
--------------------
<details><summary><b>info</b></summary>
    
### Design pattern's 
<details><summary><b>info</b></summary>
</details>

                                                             
### Service Contract
<details><summary><b>info</b></summary>
    
      Service Contract
      ================
               |
               |------What is Service contract
               |                 |-----------why should any one implement Service contract in magento
               |                 |-----------Benefit of Service Contract 
               |------types of interface service contract concept implement
               |                        |-------what is Data interfaces
               |                        |                        |---------what is data integrity
               |                        |-------what is service interfaces 
               |                                                 |----------types of service interfaces
               |                                                 |----------what is  Repository interfaces(CRUD)
               |                                                 |----------what is Management interfaces(send the email, manage related)
               |                                                 |----------what is Metadata interfaces(Eg-name has --first_name, last_name)
               |          
       
    
![Service_contract](https://user-images.githubusercontent.com/78407424/170829619-146e2aa8-2507-4f36-bfaa-718794394412.png)
    
</details>

### Dependency Injection

<details><summary><b>info</b></summary>  
    
              Dependency Injection 
             --------------------
                 |-----deffination
                 |-----diff ways or types of injection(constructor,method, by declaring di.xml way)
                 |-----require file to implement the injection
                 |-----types of dependency class
                 |                          |-----Injectable 
                 |                                      |---------what is singleton(cache memory)
                 |                          |-----Non-Injectable
                 |                                      |----------what is Factory class(entity table)
                 |                                      |                    |-------------when we need to use factory class
                 |                                      |                    |-------------advantage of factory class
                 |                                      |----------what is Proxy Class(Lazy loading, Object chaining)
                 |                                                      |--when we need to use proxy class
                 |                                                      |--where we need to declare the proxy class(di.xml)
                 |                                                          |----why we did not use proxy class directly inside constructor inject
                 |-----which two types of node di.xml file support 
                 |                                      |--------type
                 |                                      |--------virtual type
                 |
                 |-----what is the use type
                 |-----what is the use of virtual type
                 |-----Difference bewteen type and virtual type
                 |                                     |---------when to use type 
                 |                                     |---------when to use virtual type
                 |-----What are all the concept we can use to modify the magento core functionality without touching core files
                 |                             |
                 |                             |
                 |                             |----Type
                 |                             |
                 |                             |----Virtual Type
                 |                             |
                 |                             |----Plugin
                 |                             |         |-------what is plugin
                 |                             |         |-------how to declare plugin(folder way)
                 |                             |         |-------where exactly we can apply the plugin(rule's)
                 |                             |         |-------advantage and limitation of plugin
                 |                             |         |-------types of plugin
                 |                             |                         |------what is before plugin(changing method input parameter)
                 |                             |                         |------what is after plugin(changing method output parameter)
                 |                             |                         |------what is around pluign(changing actuall implementation of original code)
                 |                             |
                 |                             |----Preference
                 |                             |            |----what is preference
                 |                             |            |----how to declare plugin(folder way)
                 |                             |            |----where exactly we can apply the preference(rule's)
                 |                             |            |----advantage and limitation of plugin
                 |                             |
                 |                             |----Event and Observer(no modification to original class. need to communicate with other classes)
                 |                                          |---------what is event and observer
                 |                                          |---------how to declare plugin(folder way)
                 |                                          |---------where exactly we can apply the preference(rule's)
                 |                                          |---------advantage and limitation of plugin
                 |
                 |-----Why magento doe's not create object using new keyword
                 |-----Why magento did not allow direct use of Object Manager
                 |-----Why we did not specify Proxy in the Class Constructor Directly
                 |-----When we put Factory to Any Class -- how magento will knowing this and when    
                 |
                 |------------What is Object Manager in Magento(to mange the object by checking from di.xml(all the things declare here)
                                                          |----------what is the use of create() method (for non-injectable class)
                                                          |----------what is the use of get() method (for injectable class)
                                                          
</details>

### Object Manager
<details><summary><b>info</b></summary>

</details>


### Type vs VirtualType

<details><summary><b>info</b></summary>      
    
![type_virtualtype](https://user-images.githubusercontent.com/78407424/216369559-323f1132-c4f6-46e7-a039-21fc51bfe545.png)
 
</details>

### Factories(Factory Class)
<details><summary><b>info</b></summary>
    
![Factories_3](https://user-images.githubusercontent.com/78407424/170829686-0171959b-3bb8-4469-a952-92ad24aca85d.png)
    
</details>

### Proxies(Proxy Class)
<details><summary><b>info</b></summary>
    
- di.xml is having higher priority rather than constructor
- 
![Proxy_2](https://user-images.githubusercontent.com/78407424/170829650-ccf014c8-d401-4af4-aed3-a8ea578d9482.png)

</details>

### Indexing

<details><summary><b>info</b></summary>
    
      Indexing
      ========
        |
        |---What is Indexing in Magento
        |               |-------Why we need Indexing
        |               |-------How many types of Indexing mode
        |                                 |-----How Update on Save is working
        |                                 |-----How Update on Schedule is working
        |                                           |----Explain end to end how schedule work based on cron job
        |                                                          |------what is change_log table and how it tigger      
        |                                                          |------what is tigger function
        |                                                                  
        |---What all file require to implement indexing concept in magento
                                        |----------what is the use of indexer.xml
                                        |----------what is the use of mview.xml 
                                                          |-----how mview file is link with other files and help cron job to work      
    
    
![Screenshot from 2022-05-28 19-30-43](https://user-images.githubusercontent.com/78407424/170829798-5186503c-dead-4948-a22e-c9620b424515.png)

</details> 

### Caching

<details><summary><b>info</b></summary> 
    
    Caching 
    =======
      |
      |----------what is caching
      |                    |-------why we need caching in magento 
      |                    |-------how to know is cache is enable for particular section in magento
      |                    |-------if we declare cache is false then what happen 
      |                    |-------how to know is the site is full cache enabled
      |
      |----------What are all the way to know is the page is cache enable and how to achieve 
      |
      |---------how many types of cache mechanism
      |                           |---------------what is public content(server side)
      |                           |                            
      |                           |---------------what is private content(client side) 
      |                                                      |------------what type of data is called private content
      |--------how cahce is related with
                                      |------varnih
                                      |------redis
                                      |------Opchache
                                      |------JIT
                                      |------Zend Engine 

![caching_5](https://user-images.githubusercontent.com/78407424/170829843-dc40a7ba-3ebc-40b3-9e6b-1eb3dfd0b73a.png)

 </details>


### EAV
<details><summary><b>info</b></summary>
    
           EAV 
          =======
            |--------what is EAV
            |                 |----Why Magento implement EAV concept why not other concept to manage the data
            |                 |----How many types of entity table in magento(9)
            |                 |----How many types of data types table for entity table in magneto(5)
            |                 |----From Which table we will get the complete details of eav_table(eav_entity_type)    
            |                 |----Explain the complete eav_table relation in magento
            |                 |---If we need to add simple customer attribute then explain 
            |                                                                  |----complete flow table including attribute creation from code
            |  
            |--------types of eav attribute 
            |          |--------Custome attribute
            |          |                     |---------
            |          |                     |---------
            |          |
            |          |--Extension Attribute
            |                 |               
            |                 |
            |                 |---What is extension attribute
            |                 |---what all folder structure need to implemnt extension attribute
            |                 |---what is the use of resource in extension_attribute in magento
            |                 |                |-------------------what is the use of join in extension_attribute
            |                 |                |-------------------what are all type of extension attribute (string, init, float or Object)
            |                 |---If we need to add extension attribute for customer then what we need to do.
            |                 |--For getting and set the extension attribute which interface we need extends in service contract design.
                               
</details>

 ### Custom attribute vs Extension attribute
<details><summary><b>info</b></summary>   

</details>


### Declarative Schema (DataPatch vs SchemaPatch)
<details><summary><b>info</b></summary>

    Declarative Schema
    ==================
        |
        |-----What is declarative schema
        |                          |-------what all files need to implemnt the declare schema in magento
        |                          |-------how we can perform crud operation using db_schema.xml only
        |
        |----what is the use of db_schema_whitelist.json
        |                          |-----------------------Is mantory to keep the db_schema_whitelist if no then why 
        |
        |----What is Patchs
        |             |-------how many types of patchs available
        |             |                            |----------------what is Data patch
        |             |                            |              
        |             |                            |----------------what is Schema patch
        |             |
        |             |------If we need to create attribute then which patch we need to use
        |             |------If we need to insert data into table then which patch we need to use
        |

</details>    

    
### Order Flow
<details><summary><b>order concept</b></summary>
     
        Order Flow: 
            New: when customers just created an order and have not made any payment
            Pending: when the invoice and shipment have not been created
            Processing: the order has been either invoiced or delivered
            Complete: when the order has been both invoiced and shipped
            On hold: admins can assign the On hold status manually
            Canceled: when the order has not been paid for, the store admin or the payment gateway will decide to put this status.
            Closed: a credit memo is included and the refund has been made.
 </details>
    
### how to setup multiple store
<details><summary><b>info</b></summary>
            
            Link - https://www.youtube.com/watch?v=1HrOfr8e96A
            
                pub/index.php
                
                switch($_SERVER['HTTP_HOST']) {
                case 'casio-gshock-ecom.loc':
                $runCode = 'jp';
                $websiteType = 'website';
                break;
                case 'casio-gshock-ecom.loc.sg':
                $runCode = 'sg';
                $websiteType = 'website';
                break;
                }
                $params[\Magento\Store\Model\StoreManager::PARAM_RUN_CODE] = $runCode;
                $params[\Magento\Store\Model\StoreManager::PARAM_RUN_TYPE] = $websiteType;
                
    </details>  
</details>     

## API
-------
![api](https://user-images.githubusercontent.com/78407424/229434266-befbda7b-674b-4156-9a62-75c8a9d37319.png)
    
#### Rest Api in Magento(Service contract & webapi.xml)
 <details><summary><b>info</b></summary>
         - http://magento.local(base_url)/swagger#/
         
                        |
                        |------First check the active mode website is running
                        |                                              |-----------sudo bin/magento deploy:mode:show
                        |----- If It is in default mode then chane it to "developer"
                        |                                                     |--------- sudo bin/magento deploy:mode:set developer (do se:up & ca:fl)
                        |
                        |----Some time it will not work So Check Below Configuration
                                      |
                                      |--------------Stores > Settings > Configuration > Advanced > Developer
                                                                                                      |-------Swagger----->Enabled Yes/No (make it Yes)
   </details> 

#### GraphQl Api in Magento(Resolver & schema.graphqls)
<details><summary><b>info</b></summary>
         - http://magento.local(base_url)/swagger#/
         
                        |
                        |------First check the active mode website is running
                        |                                              |-----------sudo bin/magento deploy:mode:show
                        |----- If It is in default mode then chane it to "developer"
                        |                                                     |--------- sudo bin/magento deploy:mode:set developer (do se:up & ca:fl)
                        |
                        |----Some time it will not work So Check Below Configuration
                                      |
                                      |--------------Stores > Settings > Configuration > Advanced > Developer
                                                                                                      |-------Swagger----->Enabled Yes/No (make it Yes)
 </details> 


## Checkout Flow
----------------
<details><summary><b>info</b></summary>

### require-config.js
<details><summary><b>info</b></summary>
</details> 

### how knock.js work
<details><summary><b>info</b></summary>

</details> 
    
### Payment Method's
<details><summary><b>info</b></summary>
</details> 

</details> 
</details>

Magento Latestes Era
--------------------
<details><summary><b>info: </b></summary>
    
### Magento Contribution Path
<details><summary><b>info: </b></summary>
                <i> https://www.slideshare.net/secret/MwPFaOYcTj496V </i>
            
               - Performance
               - New Tools
               - Architecture
               - As Compare to Other E-commerce 
               - Real Life Simplified
               - Docs Support
               - Security Thread
               
</details>

### Publish your Custom Extension 
<details><summary><b>info: </b></summary>
</details>

</details>
      

E-Commerce Era (how it is working -- flipkart, amazon )
-------------------------------------------------------
<details><summary><b>info: </b></summary>
    
</details>




# Magento Core Concept
#### Multi-Store Setup for Nginx (Ubuntu)
<details><summary><b>info</b></summary>   

     Link  = https://experienceleague.adobe.com/en/docs/commerce-operations/configuration-guide/multi-sites/ms-nginx

     Step-1
     ------
          go the the directory = cd /etc/nginx/sites-available

          create a file i.e   = sudo nano local   (paste the below data - here i am doing two site setup)
     #-------------------------------------------------------------------> 
           upstream fastcgi_backend {
                 server unix:/run/php/php8.1-fpm.sock;
            }
            
            map $http_host $MAGE_RUN_CODE {
                default '';
                dev.forevernew.co.nz fn_nz;
                dev.forevernew.co.au fn_au;
            }
            
            server {
                listen 80;
                server_name dev.forevernew.co.nz dev.forevernew.co.nz dev.forevernew.co.au;
                set $MAGE_ROOT /var/www/html/local;
                set $MAGE_MODE developer;
                set $MAGE_RUN_TYPE website; #or set $MAGE_RUN_TYPE store;
                include /var/www/html/local/nginx.conf.sample;
            }
      #-------------------------------------------------------------------> 
           
            get the website code from this magento table i.e = store_website    (get the Code column value )[here fn_nz and fn_au are  website code ]


    Step-2 
    ------ 
           create two more file inside this  {" cd /etc/nginx/sites-available " directory}  [two store so - two file create if more create more file]

          i)  sudo nano dev.forevernew.co.nz  (paste the below data)

               server {
                    listen 80;
                    server_name dev.forevernew.co.nz;
                    set $MAGE_ROOT /var/www/html/local;
                    set $MAGE_MODE developer;
                    set $MAGE_RUN_TYPE website; #or set $MAGE_RUN_TYPE store;
                    set $MAGE_RUN_CODE fn_nz;
                    include /var/www/html/local/nginx.conf.sample;
                 }

 
         ii) sudo nano dev.forevernew.co.au  (paste the below data)

                server {
                    listen 80;
                    server_name dev.forevernew.co.au;
                    set $MAGE_ROOT /var/www/html/local;
                    set $MAGE_MODE developer;
                    set $MAGE_RUN_TYPE website; #or set $MAGE_RUN_TYPE store;
                    set $MAGE_RUN_CODE fn_au;
                    include /var/www/html/local/nginx.conf.sample;
                }
                
    Step-3
    ------            
             - create the all 3- files symlink to cd /etc/nginx/sites-enabled

             - sudo ln -s /etc/nginx/sites-available/local /etc/nginx/sites-enabled
             - sudo ln -s /etc/nginx/sites-available/dev.forevernew.co.nz /etc/nginx/sites-enabled
             - sudo ln -s /etc/nginx/sites-available/dev.forevernew.co.au /etc/nginx/sites-enabled

             - sudo nginx -t
            
             - sudo service nginx restart

    Step-4
    ------- 

             - Go the your magento folder location (e.g = /var/www/html/local )

             - Find nginx.conf.sample  file 

             - Edit --->  nginx.conf.sample  

             - Search   below location 
                    
                 Previous (existing)
                 =====================
                    # PHP entry point for main application
                        location ~ (index|get|static|report|404|503|health_check)\.php$ {
                            try_files $uri =404;
                            fastcgi_pass   fastcgi_backend;
                            fastcgi_buffers 1024 4k;
                        
                            fastcgi_param  PHP_FLAG  "session.auto_start=off \n suhosin.session.cryptua=off";
                            fastcgi_param  PHP_VALUE "memory_limit=1G \n max_execution_time=18000";
                            fastcgi_read_timeout 600s;
                            fastcgi_connect_timeout 600s;
                        
                            fastcgi_index  index.php;
                            fastcgi_param  SCRIPT_FILENAME  $document_root$fastcgi_script_name;
                            include        fastcgi_params;
                        }
                        
      Step-5
      -------      
             - Modify the above with Below Two Line  (Before " include    fastcgi_params;  Line)
            #------------------------------------------------------------------->   
                    - fastcgi_param MAGE_RUN_TYPE $MAGE_RUN_TYPE;
                    - fastcgi_param MAGE_RUN_CODE $MAGE_RUN_CODE;
            #------------------------------------------------------------------->          

      Step-6
      ------           
                After Modify (currently)
                ========================
                # PHP entry point for main application

                    location ~ (index|get|static|report|404|503|health_check)\.php$ {
                        try_files $uri =404;
                        fastcgi_pass   fastcgi_backend;
                        fastcgi_buffers 1024 4k;
                    
                        fastcgi_param  PHP_FLAG  "session.auto_start=off \n suhosin.session.cryptua=off";
                        fastcgi_param  PHP_VALUE "memory_limit=1G \n max_execution_time=18000";
                        fastcgi_read_timeout 600s;
                        fastcgi_connect_timeout 600s;
                    
                        fastcgi_index  index.php;
                        fastcgi_param  SCRIPT_FILENAME  $document_root$fastcgi_script_name;
                #------------------------------------------------------------------->        
                        # START - Multisite customization
                        fastcgi_param MAGE_RUN_TYPE $MAGE_RUN_TYPE;
                        fastcgi_param MAGE_RUN_CODE $MAGE_RUN_CODE;
                        # END - Multisite customization
                #-------------------------------------------------------------------->
                        include        fastcgi_params;
                    }
  

</details>



#### File & Folder Permission On Magento
<details><summary><b>info</b></summary>   
    
    Magento Folder Permission
    ---------------------------
       - # Change ownership of project directory
             sudo chown -R sanjay:sanjay /var/www/html/local

         # Fix permissions for the project directory
            find /var/www/html/local -type d -exec chmod 755 {} \;
            find /var/www/html/local -type f -exec chmod 644 {} \;

       
    Composer Install Not Working Due to Permission Issue
    ----------------------------------------------------
                     - Magento folder have different permission  & .ssh folder have different permission.
                     
                    - Give root permission to .ssh folder (i.e = sudo chmod -R 777 .ssh/) [or] Change the /var/www/html/local magento permission to .ssh level permission.
                     
                    - If /var/www/html/local  is root permission then  move the .ssh to root 
                                
                                        - sudo cp ~/.ssh /root/.ssh/
                                        - sudo chown root:root /root/.ssh/

     
     Basic of Permission For Owner(user),Group and Others
     ----------------------------------------------------
               -  700 (read, write, and execute for the owner only).

                  7 --- read + write + execute [4 + 2 + 1]
                  0 --- nothing
                  0 --- nothing 

                  


      3-types of access restrictions
      ------------------------------
            permission    |  Action | chmod option
                          |         |
             read         |  view   |  r or 4 
                          |         |
             write        |  edit   |  w or 2
                          |         |
             execute      | execute |  x or 1 



      3-types of user restrictions
      ----------------------------
            user  | Is Output 
                  |
            Owner |  -rwx------
                  |
            Group |  ----rwx---
                  |
            Other |  -------rwx
             
                          
           
        chmod  :-  permission related

        chown  :- owner and group related changes
                                   
 

</details>

   
#### Run Php Script On Magento for Quick Testing 
<details><summary><b>info</b></summary>   
    
                <?php
                use Magento\Framework\App\Bootstrap;
                use Magento\Framework\App\ObjectManager;
            
                // Include Magento Bootstrap file
                require __DIR__ . '/../app/bootstrap.php';
                
                // Initialize the Magento application
                $bootstrap = Bootstrap::create(BP, $_SERVER);
                $objectManager = $bootstrap->getObjectManager();
                $state = $objectManager->get('Magento\Framework\App\State');
                $state->setAreaCode('frontend');
                
                // Retrieve the product repository
                $productRepository = $objectManager->get('\Magento\Catalog\Model\ProductRepository');
                
                // Replace 'your_sku' with the SKU of the product you want to retrieve
                $sku = '257760';
                
                try {
                    // Load the product by SKU
                    $product = $productRepository->get($sku);
                
                    // Display product details
                    echo "Product ID: " . $product->getId() . "<br>";
                    echo "Name: " . $product->getName() . "<br>";
                    echo "SKU: " . $product->getSku() . "<br>";
                    echo "Price: " . $product->getPrice() . "<br>";
                } catch (\Magento\Framework\Exception\NoSuchEntityException $e) {
                    echo "No product found with SKU: $sku";
                }
                
                /*
                 *
                 * File location = inside the pub directory i.e = /opt/homebrew/var/www/forevernew/pub
                 *
                 * To Run on Terminal = cd /opt/homebrew/var/www/forevernew/pub
                 *                    = php Test.php
                 *
                 *  To Run on Frontend = http://dev.forevernew.co.nz/Test.php
                 *
                 */
</details>


            
# Magento Cloud Concept
#### Push and Get Data to Staging Environment Using Ssh
<details><summary><b>info</b></summary>    
    
        Connect to sftp (From the Directory where  you want to Upload the Files)
        ------------------------------------------------------------------------
                run - : sftp 1.ent-wh2okhswlvpuo-staging-ded-yg3eyli@ssh.us-3.magentosite.cloud

                        sftp> put File.php

                        sftp> put -r directoryName

                        sftp> get File.php

                        sftp> get -r applogy_email                        
        
</details>           
            
  
#### Get some select table from staging environment
<details><summary><b>info</b></summary>    
    
        Get some selected table from staging environment
        ------------------------------------------------
          bin/n98-magerun2.phar db:dump --strip="emarsys_events_data core_config_data cron_schedule emarsys_log_cron_schedule experius_emailcatcher forevernew_rma_quote  
          eshopworld_extension_logs fn_riskify_whitelist gene_bluefoot_entity_text rating_option_vote review_detail integration legacym1_giftcardwebservice_giftcardlog 
          magento_giftcardaccount_history mcom_api_messages mcom_logged_messages_queue os_search_result_customers_index password_reset_request_event webpos_staff emarsys_contact_field 
          catalog_category_flat_store_* catalog_category_product_index_* catalog_product_flat_* catalogrule_product_price_* catalogrule_product_* catalogsearch_fulltext_* 
          fredhopper_product_data_index_* queue_* salesrule_customer sequence_creditmemo_* sequence_invoice_* sequence_order_* sequence_rma_item_* sequence_shipment_* social_account adyen_* 
          stockists_location_entity_ @mailchimp @temp @klarna @newrelic_reporting @2fa @dotmailer @development" -c gz var/backups/stg-db-strip_29Oct2024.sql.gz
</details>             
            
            
            
            
            
            
            
            
     

