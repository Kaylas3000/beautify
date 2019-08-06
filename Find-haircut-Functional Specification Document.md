# Functional Specification Document

# Master-hand



**DOCUMENT VERSION**  **0.1**



**AUTHORS**

| **Name** | **Role** | **Department** |
| --- | --- | --- |
|- Sokolov Mykola |- technical implementation of the project <br> - ideas generator|   |
|- Strogonova Anastasia |- user experience, design |   |



**DOCUMENT HISTORY**

| **Date** | **Version** | **Document Revision Description** | **Document Author** |
| --- | --- | --- | --- |
| 05/07/19 | 0/0 | Initial version. Basic ideas | Strogonova A. |
| 07/07/19 | 0/1 |   | Sokolov M. |
|  06/07/19 |0/2   | some information by buttons, redaction of view of document  |   Strogonova A. |
|   |   |   |   |
|   |   |   |   |



**APPROVALS**

| **Approval Date** | **Approved Version** | **Approver Role** | **Approver** |
| --- | --- | --- | --- |
|   |   |   |   |
|   |   |   |   |
|   |   |   |   |
|   |   |   |   |

**Table of Contents**

1. [ Introduction ](#introduction)

1.1 [ Purpose of the document ](#purpose)

1.2 [ Project Scope ](#projectscope)

1.3 [ Scope of the document ](#scopedocument)

1.4 [ Related documents ](#relateddocuments)

1.5 [ Terms/Acronyms and Definitions ](#terms)

1.6 [ Risks and Assumptions ](#risks)

2. [ System/ Solution Overview ](#systemsolution)

2.1 [ Context Diagram/ Interface Diagram/ Data Flow Diagram, Application Screen Flow, Sitemap, Process Flow ](#contextdiagram)

2.2. [ System Actors ](#systemactors)

2.3. [ Dependencies and Change Impacts ](#dependencies)

3. [ Functional Specifications ](#functionalspecifications)

4. [ System Configurations ](#systemconfigurations)

5. [ Other System Requirements/ Non-Functional Requirements ](#othersystemrequirements)

6. [ Reporting Requirements ](#reporting)

7. [ Integration Requirements ](#integration)

7.1. [ Exception Handling/ Error Reporting ](#exceptionhandling)

8. [ Data Migration/ Conversion Requirements ](#datamigration)

8.1. [ Data Conversion Strategy ](#dataconversionstrategy)

8.2. [ Data Conversion Preparation ](#dataconversionpreparation)

8.3. [ Data Conversion Specifications ](#dataconversionspecifications)

9. [ References ](#references)

10. [ Open Issues ](#openissues)

Appendix

<a name="introduction"></a>
## 1. Introduction

The application to provide the relationship between customers(С) and craftsmen (service providers-SP) - hairdressers, makeup artists, nail art masters, cosmetologists &amp; etc.

<a name="purpose"></a>
## 1.1. Purpose of the document

Will be described in this document:

1. Technical requirements for application (A)

2. Stages of testing the application (A)

3. Stages of analyzing user data

4.  Interactions methodology (?) of users and program, aiming at obtaining the result (profit) by obtaining the final service by the user (U),

5. The methodology of interaction (?) between users

6. Requirements for the style of the application (appearance)

<a name="projectscope"></a>
## 1.2. Project Scope

The application solves the following tasks of a small business:
* attracting customers through targeted advertising
customer expansion
* keeping a calendar of the accounting of working hours (dates and time of visits)
* opportunity for a specialist to plan your day more efficiently
* a specialist can inform his clients about various promotions thereby increasing sales of his services

The client can select the wizard based on the actual parameters of the location, free time, price range, reviews of other clients, verified photos.

<a name="scopedocument"></a>
## 1.3. Scope of the document


1. preliminary analysis of data

2. technical data

3. interaction of program  with user,

4. interaction of users among themselves

5. the outer view of A

<a name="#relateddocuments"></a>
## 1.4 Related documents


| **Component** | **Name (with link to the document)** | **Description** |
| --- | --- | --- |
|   |   |   |

<a name="terms"></a>
## 1.5 Terms/Acronyms and Definitions

Application (A)

Customers (С)

Specialists (S) – hairdressers, makeup artists, stylists, beauticians, nail service &amp; etc.

User (U)



| **Term/Acronym** | **Definition** | **Description** |
| --- | --- | --- |
|   |   |   |

<a name="risks"></a>
## 1.6 Risks and Assumptions

- it is not known what part of the market hides its revenues and therefore will be interested a little in using the application
- masters will be able to  use  the application dishonest  
- avoiding interest payment
- masters will be able to cheat  &quot;likes&quot;, result is distrust to the application. A systematic check of the reality of reviews is needed.
- lack of media advertising at first

<a name="systemsolution"></a>
## 2.  System/ Solution Overview

Mobile application for android (Android mobile operating system 7.0 and newer) and iOS ( iOS mobile operating system 9.3.6 and newer)

the A should correctly display on the screens of mobile phones with the following parameters:
Proportions: 16:9 5:3 3:2
Size: Flagmans - iPhone Xr (1792 x 828), iPhone X Plus (2688 x 1242), iPhone X(2436 x 1125),  iPhone 8 (1334 х 750), iPhone 8  (1920 х 1080) and minimal - 5 (1136 x 640) 4 (960 x 640).

Galaxy A50 (1080x2340 px),Galaxy A70 (1080 x 2400 px)

Huawei Honor 10 Lite (1080 x 2340px) + 415ppi
Huawei Honor 8X (1080 x 2340px) + 397ppi





<a name="contextdiagram"></a>
## 2.1 Context Diagram/ Interface Diagram/ Data Flow Diagram, Application Screen Flow, Sitemap, Process Flow

**For preparing mental maps. Please, Use this program (website and this login)**

[**https://writemaps.com/**](https://writemaps.com/)

[**anstrogonova@gmail.com**](mail to:anstrogonova@gmail.com)

**18121800qQ**

**Please, be attention**  **in every little logical box can be consist a marks. You can see it, If you click to right top corner.**



**Masters**** :**

[**file:///C:/Users/loo-l/Desktop/sitemap%20(3).xml**](./../../home/k/Desktop/sitemap%20(3).xml)

[_https://writemaps.com/wmaps/shareMap/a5pbrkxj3g4h8jx_](https://writemaps.com/wmaps/shareMap/a5pbrkxj3g4h8jx)



**Customers:**

[**https://writemaps.com/wmaps/shareMap/zeiyzno6b3d10e7**](https://writemaps.com/wmaps/shareMap/zeiyzno6b3d10e7)

[**file:///C:/Users/loo-l/Downloads/sitemap%20(4).xml**](./../../home/k/%D0%97%D0%B0%D0%B3%D1%80%D1%83%D0%B7%D0%BA%D0%B8/sitemap%20(4).xml)


<a name="systemactors"></a>
## 2.2. System Actors

### 2.2.1     User Roles and Responsibilities / Authority Requirements

| **User/Role** | **Example** | **Frequency of Use** | **Security/Access, Features Used** | **Additional Notes** |
| --- | --- | --- | --- | --- | 
| _\&lt;include the specified user/role such as Purchasing Manager, Dept Admin, Faculty, Student, etc\&gt;_ | _\&lt;include examples of real people  in the role\&gt;_ | _\&lt;describes how often they use the system. State Frequent, Occasional or Rare\&gt;_ | _\&lt;describe the features of the system available for the role and any security/access permissions that should be stated\&gt;_ | _\&lt;add any additional notes or supporting documentation as necessary\&gt;_    | 
| administrator |   |   |   |   |
| programmer |   |   |   |   |
| disigner |   |   |   |   |  
| Costomer  |   |   | REGISTRATION:add date: Name Surname e-mail password repeat password sign insign out <br> Home Page: 1. Сcould select the necessary section in the main menu (directory)- internal 1.1- use the filter when searching (date, time, minimum maximum price, location territorial- search by map- selection of S :- service selection- internal 1.1.1- choosing a convenient time- contact the S phone watches, etc. <br> 1. C can search services in the search bar <br>  2. C can entry to the S schedule (duplicate calendar) <br> 3. C can send a request for the selected time of servise <br>  4. C can receve notifications <br>  5. C can edit their profile <br> 6. C can create and redact list of their S <br>  7. help <br> 8.  feedback |   |
| Specialist |   |   | S can edit your calendar:internal 1:- select customerinternal <br>  1.2clients- customer groups- choose a service- session date (start - end)- comment search for customers in the search barinvite customers <br> Add FB and other applications to attract customers add customer dataphone email birthday synchronization with a notebook create customer groupsnew customersblack listpassive clients |   |
|   |   |   |   |   |
|   |   |   |   |   |
|   |   |   |   |   |
|   |   |   |   |   |
|   |   |   |   |   |
|   |   |   |   |   |
|   |   |   |   |   |
|   |   |   |   |   |
|   |   |   |   |   |

<a name="dependencies"></a>
## 2.3.  Dependencies and Change Impacts

### 2.3.1. System Dependencies

_\&lt;List and identify any dependencies the proposed solution will have on other systems.\&gt;_

- operative system of users phone
- maps (google or another)
- synchronization with Telephone address list
- Help stuff (any chats program)
- the system of notifications
- e-mail
- check system (personification)
- calendar synchronization (google or another)
- synchronization with social nets and media (FB, instagramm, VK, snapchat)
- sms services
- synchronization with wallet, credit card


### 2.3.2. Change Impacts
The A change: 
+ hairdresser recording system
+ system for recording clients to supervisors
+ system of a reminder about the time of the visit (no need to call customers)
+ the market of beauty services
+ the sistem of appointment

<a name="functionalspecifications"></a>
## 3. Functional Specifications

_\&lt;Start describing the specifications related to the overall system here. You may want to create a table/ index of all functionalities explained in the sections below and link them to the items below\&gt;_

_\&lt;If no separate reference/ traceability document is created for the project, use this section to map the business requirements, use cases, functional requirements and the test cases\&gt;_

_ \&lt;Group your functional specifications as appropriate for your project. You may want to divide them by screens, functional areas, user role, JIRA tickets or high-level functions Vs detailed functions or any other way that works for your project\&gt;_

## 3.1. \&lt;Title\&gt;

### 3.1.1. Purpose/ Description

_\&lt;Include a high-level description and purpose of the specifications covered in the section.\&gt;_

### 3.1.2. Use case

_\&lt;Map the functional requirement to one or more use cases mentioned in the Business Requirements document. If the use case is not described in detail in the Business Requirements document, describe the use case here. This typically includes the element s in the following table.\&gt;_


| **UC-1** | **Registration page** |
| --- | --- |
| **Primary Actor(s)**| specialist or client |
| **Stakeholders and Interest** | specialist or client |
| **Trigger** | entrance to registration page |
| **Pre-conditions** | user has not been registered before | 
| **Post-conditions** | the user receives his individual account and is registered | 
| **Main Success Scenario** |  1. visit STARTING-POINT — registration page<br>  2. put data into fields of registration data (name, telephone number, e-mail, social network)<br> 3. click the register button (join)<br> 4. Make sure GOAL-ACHIEVED - Go to the created profile page> |
| **Extensions** | 1.registration through social networks<br> 2.invalid phone number<br> 3.retry confirmation code<br> 4.Invalid Email<br> 5.invalid characters entered in fields<br> 6.user with given mail number already exists_ |
| **Priority** | priority of high|
| **Special Requirements** |communication with the registration system through social networks <br> communication with the communication system by phone number|
|**Open Questions** |  |


| **UC-1** | **\&lt;Use case name\&gt;** |
| --- | --- |
| **Primary Actor(s)** | _\&lt; primary actors that participate in this use case\&gt;_ |
| **Stakeholders and Interest** | _\&lt;One sentence describing other stakeholders\&gt;_ |
| **Trigger** | _\&lt;Condition/action that initiates/starts the use-case\&gt;_ |
| **Pre-conditions** | _\&lt;Condition assumed to be true before the first step\&gt; _ |
| **Post-conditions** | _\&lt;Condition after the use case is successfully executed \&gt; _ |
| **Main Success Scenario** | 1. _\&lt;visit STARTING-POINT_ 2. _Step_ 3. _Step_ 4. _Make sure GOAL-ACHIEVED\&gt;_|
| **Extensions** | If Condition, then Alternative Steps\&lt;List any extended steps/ scenarios that occur, other than the main success scenario.\&gt; |
| **Priority** | _\&lt;indicate priority of high, medium or low)_ |
| **Special Requirements** | _\&lt;Any system related special requirements needed to fulfill the use case\&gt;_ |
| **Open Questions** | _\&lt;Notes and questions\&gt;_ |

### 3.1.3. Mock-up

_\&lt;Provide the mock-up of the functionality or a mock-up of the entire page\&gt;_

### 3.1.4.  Functional Requirements

_\&lt;Describe the page level details that are not captured in section 3.1.5 below.  These may include any requirements related to Navigation Menu, Actions, transaction status, verification and validation requirements etc._

_Make sure each specification has a reference number and is explained in the following format.\&gt;_

| **Spec ID** | **Specification Description** | **Business Rules/ Data Dependency** |
| --- | --- | --- |
| _\&lt;Specification Identifier\&gt;_ | _\&lt;Short explanation of the specification\&gt;_ | _\&lt;Any validation rules or business rules\&gt;_ |

_\&lt;Note: Section 3.1.4 and section 3.1.5 may be combined if there are a few functionalities on a particular page\&gt;_

### 3.1.5. Field level specifications

_\&lt;Specify all the field data elements related to the functional requirement in both tables below.\&gt;_

**Form Elements:**

| **Call-out** | **Field Label** | **UI Control** | **Mand?** | **Editable** | **Data Type** | **Value Set** | **Default Value** | **Data Example** | **Data Source** |
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
| _\&lt;mock-up reference\&gt;_ | _\&lt;Label name\&gt;_ | _\&lt;specify what UI control will be on screen\&gt;_ | _\&lt;specify if field is mandatory\&gt;_ | _\&lt;specify if field is editable\&gt;_ | _\&lt;Specify the data type that will be used for this field\&gt;_ | _\&lt;If value is from the set, specify the entire value set here\&gt;_ | _\&lt;Specify if it should be defaulted to any value\&gt;_ | _\&lt;Provide an example of the data\&gt;_ | _\&lt;Specify the source of the data\&gt;_ |
| Example: Call-out 1 | User name | textbox | Yes | Yes | Alpha-numeric | none | NA | agujar | User entry |

**Form Business Rules and Dependencies:**

| **Field Label** | **Validation / Business Rules**   | **Error Messages** | **Data Dependencies** | **Additional Info/ Notes** |
| --- | --- | --- | --- | --- |
| _\&lt;Label name\&gt;_ | _\&lt;Specify the validation rules and/ or business rules applicable to the form element\&gt;_ | _\&lt;List the error message that should be displayed and under what conditions\&gt;_ | _\&lt;Specify if there are any date dependencies\&gt;_ | _\&lt;Provide any additional information here\&gt;_ |
| _Example: User name_ | _User name shall be a valid Stanford Sunet ID_ | _For incorrect user name display on setFocusOff: &quot;Please provide a valid user name&quot;_ | _None_ | _Access prohibited only to Stanford affiliates. For non-Stanford affiliates, check call-out 3.1_ |

**Buttons, Links and Icons:**

| **Button, Link, Icon Label** | **OnClick Event** | **Other Event** | **Visible** | **Enabled Vs Disabled** | **Navigate To** | **Validation** | **Dependencies** |
| --- | --- | --- | --- | --- | --- | --- | --- |
| _\&lt;Button label name\&gt;_ | _\&lt;Specify the operation that would be performed on an on-click event\&gt;_ | _\&lt;Specify the operation that would be performed on other events\&gt;_ | _\&lt;Specify default visibility of the button\&gt;_ | _\&lt;Specify if button is enabled or disabled and the condition, if any\&gt;_ | _\&lt;Specify the link where the page will be re-directed, if any\&gt;_ | _\&lt;Specify the validation rules on operation of the button\&gt;_ | _\&lt;Mention if there are any dependencies on other form elements and/ or buttons\&gt;_ |
|Button-**login**_ | Move on page with fields of user’s information_ | __ | Yes, always_ | __ | User Dashboard page_ | V_ | Disable the New user functionality on subsequent pages if user logs in through this button._ |
|Button- **registration**| Move on  page with fields of user’s information |||||
|Button-**as spesialist**| Move on  page with fields of user’s information for new spesialists||||
|Button-**as client**|Move on page with fields of user’s information for new clients||||
|Button-**Help**|Move on  page with help desk||||









Disable the New user functionality on subsequent pages if user logs in through this button.




<a name="systemconfigurations"></a>
## 4. System Configurations

_\&lt;Provide an overview of all the steps or the set ups required to configure an application/program. Also state the intent or purpose behind each set up or configuration. Discuss the possible alternatives, customizations, workaround&#39;s, conditions and dependencies in a particular configuration. In case of Oracle applications, please list all applicable BR100&#39;s or Application set up documents\&gt;_

<a name="othersystemrequirements"></a>
## 5. Other System Requirements/ Non-Functional Requirements

_\&lt;This section is used in contrast with stated functional requirements to highlight the additional details on the quality related aspects as well as other behavioral aspects of a system. This section is used to capture the stakeholders&#39; implicit expectations about how well the system will work under a given circumstance. Here you can  state the specific SLA&#39;s related to system response times (Data search and retrieval), Performance needs and metrics, Latencies in a particular timeframe or during high volume transactions, System failures and recovery management, Security levels and accessibility constraints, Data Backup and archiving Capabilities, Legal compliance needs etc. The broader definition of the term &#39;system&#39; also includes integrations with all types of Mobile platforms, Mobile devices, Tablets and Smart phones.\&gt;_

<a name="reporting"></a>
## 6. Reporting Requirements

_\&lt;This section is used to capture the reporting needs, including but not limited to the scope and format of the report, data elements and contents required on the report, file types and extraction mechanisms, user base and accessibility levels, frequency of report extractions etc. Also provide the mock up of the report if needed.  If necessary, create a separate document for reporting requirements.\&gt;_

<a name="integration"></a>
## 7. Integration Requirements

_\&lt;Identify the integration needs and state all required interfaces with anything external to this solution including hardware, software, and users. Include Architectural overview diagrams, high level data flow diagrams, table structures and schema, interface protocols, API&#39;s, Error conditions, Error validations and messaging needs, Auto processing requirements etc. You can optionally state hardware and software dependencies, Upgrade requirements, compatibility issues with existing frameworks and solutions, etc\&gt;_

_(Data Flow Diagrams,_ _Interface_ _Diagrams – if necessary)_


<a name="exceptionhandling"></a>
## 7.1 Exception Handling/ Error Reporting

_\&lt;This is where you can explain the error conditions/Exceptions that normally happen in Interfaces or cross flow system integrations. Explain the nature of exception, Error Id, Root cause of the error and also the strategy to handle the scenario. You can also indicate if there are any concurrent programs designed to automatically handle the error records or error conditions. State if there are any error reports generated or notifications utilized to alarm the support teams and system Administrators during the interface failures or outages\&gt;_

| **Exception/ Error ID** | **Error** | **Cause** | **Solution Strategy** |
| --- | --- | --- | --- |
|   |   |   |   |

<a name="datamigration"></a>
## 8. Data Migration/ Conversion Requirements

_\&lt;Explain in brief the data conversion plan._ _Provide full identifying information for the automated system, application, or situation for which the Data Conversion Plan applie __s._ _Describe_ _briefly_ _any assumptions__ , constraints_ _or_ _risks_ _regarding the data conversion effort._ _(Provide details in section 1.6)\&gt;_


<a name="dataconversionstrategy"></a>
## 8.1 Data Conversion Strategy

_\&lt;Include the overall strategy for the Data Conversion. This includes how and when you will perform the conversion - the approach used to extract, transform and load data during the conversion process, the conversion schedule, and test plan for testing the converted data.\&gt;_

<a name="dataconversionpreparation"></a>
8.2 Data Conversion Preparation

_\&lt;Provide details on any prerequisites necessary for the conversion. Discuss the backup strategy, restoration process in case the conversion fails.\&gt;_

<a name="dataconversionspecifications"></a>
8.3 Data Conversion Specifications

| **Source** | **Source Data Element** | **Target** | **Target Data Element** | **Conversion Rules** | **Notes** |
| --- | --- | --- | --- | --- | --- |
| _\&lt;Source location\&gt;_ | _\&lt;Source Data Element Identifier \&gt;_ | _\&lt;Target location\&gt;_ | _\&lt;Target Data Element Identifier\&gt;_ | _\&lt;Describe rules for Data conversion\&gt;_ | _\&lt;Additional notes\&gt;_ |

<a name="references"></a>
## 9. References

_\&lt;__List all references to external material used as background information or knowledge for the FSD. Examples may include a compliancy website, Stanford website, etc\&gt;_

<a name="openissues"></a>
10. Open Issues

| **Issue ID** | **Issue** | **Raised By** | **Raised On** | **Solution/ Decision** | **Resolved By** | **Resolved On** | **Status** |
| --- | --- | --- | --- | --- | --- | --- | --- |
|   |   |   |   |   |   |   |   |

# Appendix
