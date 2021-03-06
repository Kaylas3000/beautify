# Functional Specification Document

# Master-hand



**DOCUMENT VERSION**  **0.1**



**AUTHORS**

| **Name** | **Role** | **Department** |
| --- | --- | --- |
|- Sokolov Mykola |- technical implementation of the project <br> - ideas generator|   |
| |- user experience, design |   |



**DOCUMENT HISTORY**

| **Date** | **Version** | **Document Revision Description** | **Document Author** |
| --- | --- | --- | --- |
| 05/07/19 | 0.0 | Initial version. Basic ideas | Strogonova A. |
| 07/07/19 | 0.1 | Minor changes  | Sokolov M. |
| 06/08/19 | 0.2 | added some information about buttons, redaction of view of document  |   Strogonova A. |
| 07/08/19 | 0.3 |  several pictures of screen A from "Fluid" with discriptions <br> redact the dictionary of termins |  Strogonova A.   |
| 03/03/2021  | 0.4  | Added DMS specification, changed risks section.  | Sokolov M. |
| 04/03/2021  | 0.5  | Added authentication and localization sections.  | Sokolov M. |


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

2.1. [ Context Diagram/ Interface Diagram/ Data Flow Diagram, Application Screen Flow, Sitemap, Process Flow ](#contextdiagram)

2.2. [ System Actors ](#systemactors)

2.3. [ Dependencies and Change Impacts ](#dependencies)

3. [ Functional Specifications ](#functionalspecifications)

3.1. [ Database management system ](#Database)

3.2. [ Authentication and authorization mechanism ](#Authentication)

3.3. [ Localization ](#Localization)

4. [ System Configurations ](#systemconfigurations)

5. [ Other System Requirements/ Non-Functional Requirements ](#othersystemrequirements)

6. [ Reporting Requirements ](#reporting)

7. [ Integration Requirements ](#integration)

7.1. [ Exception Handling/ Error Reporting ](#exceptionhandling)

8. [ Data Migration/ Conversion Requirements ](#datamigration)

8.1. [ Data Conversion Strategy ](#dataconversionstrategy)

8.2. [ Data Conversion Preparation ](#dataconversionpreparation)

8.3. [ Data Conversion Specifications ](#dataconversionspecifications)

9. [ Security ](#security)

10. [ References ](#references)

11. [ Open Issues ](#openissues)

12. [ Appendix ](appendix)

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

3. interaction of application with user

4. interaction of users among themselves

5. basic design of the application

<a name="relateddocuments"></a>
## 1.4 Related documents

| **Component** | **Name (with link to the document)** | **Description** |
| --- | --- | --- |
|   |   |   |

<a name="terms"></a>
## 1.5 Terms/Acronyms and Definitions
[ Moved to Appenndix ](appendix)

<a name="risks"></a>
## 1.6 Risks and Assumptions

- the idea might be stolen or concurrency will bring better application to the market
- it is not known what part of the market hides its revenues and therefore will be interested a little in using the application
- masters will be able to  use  the application dishonest  
- avoiding interest payment by masters(masters will take a client contacts instead of using the app)
- masters will be able to cheat  &quot;likes&quot;, resulting in distrust to the application. A systematic check of the quality of reviews is needed.
- lack of media advertising. As a result application would not be interesting to audience
- it might be too difficult to implement all features in time so the customers might quickly loose the interest to the app


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
| _include the specified user/role such as Purchasing Manager, Dept Admin, Faculty, Student, etc_ | _include examples of real people  in the role_ | _describes how often they use the system. State Frequent, Occasional or Rare_ | _describe the features of the system available for the role and any security/access permissions that should be stated_ | _add any additional notes or supporting documentation as necessary_    |
| administrator |   | often  |   | Superuser. This user has access everywhere.  |
| developer     |   |        |   | Developer user role. Used for access to the app as developer  |
| costomer      |   | often  | REGISTRATION:add date: Name Surname e-mail password repeat password sign insign out <br> Home Page: 1. Сcould select the necessary section in the main menu (directory)- internal 1.1- use the filter when searching (date, time, minimum maximum price, location territorial- search by map- selection of S :- service selection- internal 1.1.1- choosing a convenient time- contact the S phone watches, etc. <br> 1. C can search services in the search bar <br>  2. C can entry to the S schedule (duplicate calendar) <br> 3. C can send a request for the selected time of servise <br>  4. C can receve notifications <br>  5. C can edit their profile <br> 6. C can create and redact list of their S <br>  7. help <br> 8.  feedback |   |
| specialist |   | often | S can edit your calendar:internal 1:- select customerinternal <br>  1.2clients- customer groups- choose a service- session date (start - end)- comment search for customers in the search barinvite customers <br> Add FB and other applications to attract customers add customer dataphone email birthday synchronization with a notebook create customer groupsnew customersblack listpassive clients |   |
| tester  |   | sometimes  |   | Testing user role. Will be assigned for testers.   |
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

List and identify any dependencies the proposed solution will have on other systems.

- operating system of users phone
- maps (google or another)
- Help stuff (any chats program)
- the system of notifications
- e-mail
- check system (personification)
- synchronization with calendar (google or another)
- synchronization with Telephone address list
- synchronization with social media (FB, instagramm, VK, snapchat)
- sms services
- synchronization with wallet, credit cards


### 2.3.2. Change Impacts
The A change:
+ hairdresser recording system
+ system for recording clients to supervisors
+ system of a reminder about the time of the visit (no need to call customers)
+ the market of beauty services
+ the sistem of appointment

<a name="functionalspecifications"></a>
## 3. Functional Specifications

Start describing the specifications related to the overall system here. You may want to create a table/ index of all functionalities explained in the sections below and link them to the items below

If no separate reference/ traceability document is created for the project, use this section to map the business requirements, use cases, functional requirements and the test cases

Group your functional specifications as appropriate for your project. You may want to divide them by screens, functional areas, user role, JIRA tickets or high-level functions Vs detailed functions or any other way that works for your project

<a name="Database"></a>
### 3.1. Database management system

Database management system should meet following requirements:
- reliable (support fault tolerance technology)
- provide sufficient Performance
- support backup\restore
- cost effective, preferably open source, free software
- data privacy and encryption should be considered
- data conversion


Amazon RDS should be considered. Advantages: ready solution(works out of the box), automatic backup\restore, perfect reliability. Disadvantage: pricing.

MySQL or PostgreSQL inside Amazon EC2 instance. Advantages: Easy to install, cost effective. Disadvantages: does not provide good fault tolerance, there are issues with backup\restore.

Google Firebase. Support real time database, Authentication. Cloud Firestore (noSQL database).

### 3.1.2. Use case

_Map the functional requirement to one or more use cases mentioned in the Business Requirements document. If the use case is not described in detail in the Business Requirements document, describe the use case here. This typically includes the element s in the following table._

<a name="Authentication"></a>
### 3.2 Authentication and authorization mechanism

Authentication and authorization might be implemented using google Firebase. It's available for Android as well as for iOS. User roles described in [System Actors section](#systemactors).

Authentication should be available with

- Facebook
- Gmail
- Apple
- Email
- Phone number

User should be able to logout. User should be able to close the account (probably on setting page). Account should be removed as well as user data after closing account.

<a name="Localization"></a>
### 3.3 Localization

The application should support localization. All section of the app should support translation to different languages. Translation to different languages should be in separate xml file.

<a name="Billing"></a>
### 3.3 Billing (checkout)
Users should be able to pay for the services by payment cards (credit or debit). User should be able to add a card in their profile. Should be investigated is it's possible t use Google Pay, Apple pay and integrate it the the app (android and iPhone respectively). 

## Registration part


![Login picture](https://github.com/nzamb1/find-haircut/blob/master/login.jpg)

| **1** | **Registration page** |
| --- | --- |
| **Primary Actor(s)**| specialist or client |
| **Stakeholders and Interest** | specialist or client |
| **Trigger** | entrance to registration page |
| **Pre-conditions** | user has not been registered before | 
| **Post-conditions** | the user receives his individual account and is registered | 
| **Main Success Scenario** |  1. visit STARTING-POINT — registration page <br>  2. put data into edit fields of registration data (name, telephone number, e-mail, social network)<br> 3. click the register button (join)<br> 4. Make sure GOAL-ACHIEVED - Go to the created profile page> |
| **Extensions** | 1.registration through social networks<br> 2.invalid phone number<br> 3.retry confirmation code<br> 4.Invalid Email<br> 5.invalid characters entered in fields<br> 6.user with given mail number already exists_ |
| **Priority** | priority of high|
| **Special Requirements** |communication with the registration system through social networks <br> communication with the communication system by phone number|
|**Open Questions** |  |


![today calendar picture](https://github.com/nzamb1/find-haircut/blob/master/1969c23f79.jpg)

## Calendar

| **2** | **today calendar** |
| --- | --- |
| **Primary Actor(s)** | S |
| **Stakeholders and Interest** | Ad |
| **Trigger** | sign in after that will open the page **today calendar** |
| **Pre-conditions** | the desire to create a session. session not created. check the schedule |
| **Post-conditions** | session created |
| **Main Success Scenario** | 1. STARTING-POINT - press to the time line (grid view of the calendar at the screen <br>  2. choose day, week, month calendar <br> 3.  Make sure GOAL-ACHIEVED - start to create a sassion(s) |
| **Extensions** | 1.the S wants to change the information in actual Ss. <br> 2.the S can press the icon of main menu in right top corner of the screen and choose action from here <br> 3. leaf the dates of present month, week by pressing <br> 4. check the schedule <br> |
| **Priority** | priority of highthe S can press the icon of main menu in right top corner of the screen and choose action from here |
| **Special Requirements** | synchronization with googl calendar and other types of calendars |
| **Open Questions** | What is the best ways to add sassions? |



![calendar menu](https://github.com/nzamb1/find-haircut/blob/master/menu%20create%20session.jpg)

## Session (creation)

| **3** | **create session** |
| --- | --- |
| **Primary Actor(s)** | S |
| **Stakeholders and Interest** | C |
| **Trigger** | press the **menu** icon on the right top corner at previous screen|
| **Pre-conditions** | S wants to add Ss in calendar|
| **Post-conditions** | create new Ss which S and C can see in their calendar |
| **Main Success Scenario** | 1. STARTING-POINT - press to the time line of the calendar grid at the screen or icon of main menu, after that appear dropdown menu (top right coner of previus screen) <br>  2. choose the client <br> 3. choose the service or servises <br> 4.choose the day 5. choose the start time <br> 5. the duration of session <br> 6. if need choose the time of breack <br> 7. optional add photos <br> 8. optional add comments to Ss <br>  9. choose colore of the Ss, which will be shown in calendar. <br> 3.  Make sure GOAL-ACHIEVED -  add a sassion(s) with full information.
| **Extensions** | 1.return to the current calendar day/week/month menu. <br> 2.Also possible to partially fill in the session information<br>  |
| **Priority** | hight |
| **Special Requirements** | connection with adress phone list, Fb, VK e.t.c., e-mail. Connection with calendar of C |
| **Open Questions** | How to choose faster several servises, which S will do to the same C? Add a function of sms notification for C and alarm for every S? |


![choosing clients menu](https://github.com/nzamb1/find-haircut/blob/master/clients%20list.jpg)

| **4** | **choosing clients for Ss** |
| --- | --- |
| **Primary Actor(s)** | S |
| **Stakeholders and Interest** | C |
| **Trigger** | press the **client** on the pull down menu of main menu icon|
| **Pre-conditions** | S wants to add definite C or group of C or several Cs to new session(s)|
| **Post-conditions** | the C have been choosen for definite Ss |
| **Main Success Scenario** | 1. STARTING-POINT - press to **client** in dropdown menu <br>  2. choose the client from the App list or search bar <br> 3. return to updated previus page  <br> 4.3.  Make sure GOAL-ACHIEVED - add a definite C in Ss.|
| **Extensions** | 1.return to the page **create session**. <br> 2. Add new C not from App list by the button **plus** by hand <br> 3. Add groups of Cs. <br> |
| **Priority** | normal |
| **Special Requirements** | connection with adress phone list, Fb, VK e.t.c., e-mail. Connection with calendar of C |
| **Open Questions** | What is the right name of link/button **client**, **plus**?|





### 3.1.3. Mock-up

_Provide the mock-up of the functionality or a mock-up of the entire page_

### 3.1.4.  Functional Requirements

_Describe the page level details that are not captured in section 3.1.5 below.  These may include any requirements related to Navigation Menu, Actions, transaction status, verification and validation requirements etc._

_Make sure each specification has a reference number and is explained in the following format._

| **Spec ID** | **Specification Description** | **Business Rules/ Data Dependency** |
| --- | --- | --- |
| _Specification Identifier_ | _Short explanation of the specification_ | _Any validation rules or business rules_ |

_Note: Section 3.1.4 and section 3.1.5 may be combined if there are a few functionalities on a particular page_

### 3.1.5. Field level specifications

_Specify all the field data elements related to the functional requirement in both tables below._

**Form Elements:**

| **Call-out** | **Field Label** | **UI Control** | **Mand?** | **Editable** | **Data Type** | **Value Set** | **Default Value** | **Data Example** | **Data Source** |
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
| _mock-up reference_ | _Label name_ | _specify what UI control will be on screen_ | _specify if field is mandatory_ | _specify if field is editable_ | _Specify the data type that will be used for this field_ | _If value is from the set, specify the entire value set here_ | _Specify if it should be defaulted to any value_ | _Provide an example of the data_ | _Specify the source of the data_ |
| Example: Call-out 1 | User name | textbox | Yes | Yes | Alpha-numeric | none | NA | agujar | User entry |

**Form Business Rules and Dependencies:**

| **Field Label** | **Validation / Business Rules**   | **Error Messages** | **Data Dependencies** | **Additional Info/ Notes** |
| --- | --- | --- | --- | --- |
| _Label name_ | _Specify the validation rules and/ or business rules applicable to the form element_ | _List the error message that should be displayed and under what conditions_ | _Specify if there are any date dependencies_ | _Provide any additional information here_ |
| _Example: User name_ | _User name shall be a valid Stanford Sunet ID_ | _For incorrect user name display on setFocusOff: &quot;Please provide a valid user name&quot;_ | _None_ | _Access prohibited only to Stanford affiliates. For non-Stanford affiliates, check call-out 3.1_ |

**Buttons, Links and Icons:**

| **Button, Link, Icon Label** | **OnClick Event** | **Other Event** | **Visible** | **Enabled Vs Disabled** | **Navigate To** | **Validation** | **Dependencies** |
| --- | --- | --- | --- | --- | --- | --- | --- |
| _Button label name_ | _Specify the operation that would be performed on an on-click event_ | _Specify the operation that would be performed on other events_ | _Specify default visibility of the button_ | _Specify if button is enabled or disabled and the condition, if any_ | _Specify the link where the page will be re-directed, if any_ | _Specify the validation rules on operation of the button_ | _Mention if there are any dependencies on other form elements and/ or buttons_ |
|Button-**login**_ | Move on page with fields of user’s information_ | __ | Yes, always_ | __ | User Dashboard page_ | V_ | Disable the New user functionality on subsequent pages if user logs in through this button._ |
|Button- **registration**| Move on  page with fields of user’s information |||||
|Button-**as spesialist**| Move on  page with fields of user’s information for new spesialists||||
|Button-**as client**|Move on page with fields of user’s information for new clients||||
|Button-**Help**|Move on  page with help desk||||









Disable the New user functionality on subsequent pages if user logs in through this button.




<a name="systemconfigurations"></a>
## 4. System Configurations

_Provide an overview of all the steps or the set ups required to configure an application/program. Also state the intent or purpose behind each set up or configuration. Discuss the possible alternatives, customizations, workaround&#39;s, conditions and dependencies in a particular configuration. In case of Oracle applications, please list all applicable BR100&#39;s or Application set up documents_

<a name="othersystemrequirements"></a>
## 5. Other System Requirements/ Non-Functional Requirements

_This section is used in contrast with stated functional requirements to highlight the additional details on the quality related aspects as well as other behavioral aspects of a system. This section is used to capture the stakeholders&#39; implicit expectations about how well the system will work under a given circumstance. Here you can  state the specific SLA&#39;s related to system response times (Data search and retrieval), Performance needs and metrics, Latencies in a particular timeframe or during high volume transactions, System failures and recovery management, Security levels and accessibility constraints, Data Backup and archiving Capabilities, Legal compliance needs etc. The broader definition of the term &#39;system&#39; also includes integrations with all types of Mobile platforms, Mobile devices, Tablets and Smart phones._

<a name="reporting"></a>
## 6. Reporting Requirements

_This section is used to capture the reporting needs, including but not limited to the scope and format of the report, data elements and contents required on the report, file types and extraction mechanisms, user base and accessibility levels, frequency of report extractions etc. Also provide the mock up of the report if needed.  If necessary, create a separate document for reporting requirements._

<a name="integration"></a>
## 7. Integration Requirements

_Identify the integration needs and state all required interfaces with anything external to this solution including hardware, software, and users. Include Architectural overview diagrams, high level data flow diagrams, table structures and schema, interface protocols, API&#39;s, Error conditions, Error validations and messaging needs, Auto processing requirements etc. You can optionally state hardware and software dependencies, Upgrade requirements, compatibility issues with existing frameworks and solutions, etc_

_(Data Flow Diagrams,_ _Interface_ _Diagrams – if necessary)_


<a name="exceptionhandling"></a>
## 7.1 Exception Handling/ Error Reporting

_This is where you can explain the error conditions/Exceptions that normally happen in Interfaces or cross flow system integrations. Explain the nature of exception, Error Id, Root cause of the error and also the strategy to handle the scenario. You can also indicate if there are any concurrent programs designed to automatically handle the error records or error conditions. State if there are any error reports generated or notifications utilized to alarm the support teams and system Administrators during the interface failures or outages_

| **Exception/ Error ID** | **Error** | **Cause** | **Solution Strategy** |
| --- | --- | --- | --- |
|   |   |   |   |

<a name="datamigration"></a>
## 8. Data Migration/ Conversion Requirements

_Explain in brief the data conversion plan._ _Provide full identifying information for the automated system, application, or situation for which the Data Conversion Plan applie __s._ _Describe_ _briefly_ _any assumptions__ , constraints_ _or_ _risks_ _regarding the data conversion effort._ _(Provide details in section 1.6)_


<a name="dataconversionstrategy"></a>
## 8.1 Data Conversion Strategy

_Include the overall strategy for the Data Conversion. This includes how and when you will perform the conversion - the approach used to extract, transform and load data during the conversion process, the conversion schedule, and test plan for testing the converted data._

<a name="dataconversionpreparation"></a>
8.2 Data Conversion Preparation

_Provide details on any prerequisites necessary for the conversion. Discuss the backup strategy, restoration process in case the conversion fails._

<a name="dataconversionspecifications"></a>
8.3 Data Conversion Specifications

| **Source** | **Source Data Element** | **Target** | **Target Data Element** | **Conversion Rules** | **Notes** |
| --- | --- | --- | --- | --- | --- |
| _Source location_ | _Source Data Element Identifier_ | _Target location_ | _Target Data Element Identifier_ | _Describe rules for Data conversion_ | _Additional notes_ |

<a name="security"></a>
## 9. Security
System be compliant with following standards: GDPR.

<a name="references"></a>
## 10. References

_List all references to external material used as background information or knowledge for the FSD. Examples may include a compliancy website, Stanford website, etc_

<a name="openissues"></a>
## 11. Open Issues

| **Issue ID** | **Issue** | **Raised By** | **Raised On** | **Solution/ Decision** | **Resolved By** | **Resolved On** | **Status** |
| --- | --- | --- | --- | --- | --- | --- | --- |
|   |   |   |   |   |   |   |   |

<a name="appendix"></a>
## 12. Appendix
<a name="terms"></a>
## 12.1 Terms/Acronyms and Definitions

| **Term/Acronym** | **Definition** | **Description** |
| --- | --- | --- |
| A | Application  |  |
| Ad | Administrator |   |
| C | Customers | service buyer; person interested in choosing a specialist |
| S | Specialists  | hairdressers, makeup artists, stylists, beauticians, nail service &amp; etc. |
| U | User| all users of the application|
| Ss | sassion | time of the provision of services with indication of data on the client |
| B |Button | control which can be clicked upon to perform an action. An equivalent to a push-button as found on mechanical or electronic instruments.|
|RB|Radio button| control which can be clicked upon to select one option from a selection of options, similar to selecting a radio station from a group of buttons dedicated to radio tuning. Radio buttons always appear in pairs or larger groups, and only one option in the group can be selected at a time; selecting a new item from the group's buttons also de-selects the previously selected button.|
 |CB|Check box| – control which can be clicked upon to enable or disable an option. Also called a tick box. The box indicates an "on" or "off" state via a check mark/tick ☑ or a cross ☒. Can be shown in an intermediate state (shaded or with a dash) to indicate that various objects in a multiple selection have different values for the property represented by the check box. Multiple check boxes in a group may be selected, in contrast with radio buttons.|
|SB|Split button| – control combining a button (typically invoking some default action) and a drop-down list with related, secondary actions.|
|ClB| Cycle button| - a button that cycles its content through two or more values, thus enabling selection of one from a group of items.
|Sl| Slider|  – control with a handle that can be moved up and down (vertical slider) or right and left (horizontal slider) on a bar to select a value (or a range if two handles are present). The bar allows users to make adjustments to a value or process throughout a range of allowed values.|
| Lb| List box| – a graphical control element that allows the user to select one or more items from a list contained within a static, multiple line text box.|
|Sp|Spinner – value input control which has small up and down buttons to step through a range of values
|DdL|Drop-down list| – A list of items from which to select. The list normally only displays items when a special button or indicator is clicked.|
|M| Menu| – control with multiple actions which can be clicked upon to choose a selection to activate.|
|CM| Context menu| – a type of menu whose contents depend on the context or state in effect when the menu is invoked.|
|PM| Pie menu| – a circular context menu where selection depends on direction.|
|Mb|Menu bar| – a graphical control element which contains drop down menus.|
|Tb|Toolbar| – a graphical control element on which on-screen buttons, icons, menus, or other input or output elements are placed.|
|Rb|Ribbon|– a hybrid of menu and toolbar, displaying a large collection of commands in a visual layout through a tabbed interface.|
|Cbx|Combo box| (text box with attached menu or List box) – A combination of a single-line text box and a drop-down list or list box, allowing the user to either type a value directly into the control or choose from the list of existing options.|
|I|Icon| – a quickly comprehensible symbol of a software tool, function, or a data file.|
|TrV| Tree view|– a graphical control element that presents a hierarchical view of information.|
|GV|Grid view or datagrid| – a spreadsheet-like tabular view of data that allows numbers or text to be entered in rows and columns.|

### Navigation

| **Term/Acronym** | **Definition** | **Description** |
| --- | --- | --- |
|L|Link| – Text with some kind of indicator (usually underlining and/or color) that indicates that clicking it will take one to another screen or page.|
|Tb|Tab| – a graphical control element that allows multiple documents or panels to be contained within a single window.|
|Scr|Scrollbar| – a graphical control element by which continuous text, pictures, or any other content can be scrolled in a predetermined direction (up, down, left, or right).|

### Text/value input

| **Term/Acronym** | **Definition** | **Description** |
| --- | --- | --- |
|Tbox|Text box |– (edit field) - a graphical control element intended to enable the user to input text.|
|Cbox|Combo box| – a graphical control element combining a drop-down list or list box and a single-line editable textbox.|

### Output

| **Term/Acronym** | **Definition** | **Description** |
| --- | --- | --- |
|Lb|Label| – text used to describe another widget.|
|Tt|Tooltip| – informational window which appears when the mouse hovers over another control.|
||Balloon help||
||Status bar| – a graphical control element which poses an information area typically found at the window's bottom.|
||Progress bar| – a graphical control element used to visualize the progression of an extended computer operation, such as a download, file transfer, or installation.|
||Infobar| – a graphical control element used by many programs to display non-critical information to a user.|

  ## Container

 | **Term/Acronym** | **Definition** | **Description** |  
 | --- | --- | --- |
|Wn|Window|– a graphical control element consisting of a visual area containing some of the graphical user interface elements of the program it belongs to.|
||Collapsible panel| – a panel that can compactly store content which is hidden or revealed by clicking the tab of the widget.|
||Drawer| Side sheets or surfaces containing supplementary content that may be anchored to, pulled out from, or pushed away beyond the left or right edge of the screen.|
||Accordion| – a vertically stacked list of items, such as labels or thumbnails where each item can be "expanded" to reveal the associated content.|
||Modal window| – a graphical control element subordinate to an application's main window which creates a mode where the main window can't be used.|
||Dialog box|– a small window that communicates information to the user and prompts for a response.|
||Palette window| – also known as "Utility window" - a graphical control element which floats on top of all regular windows and offers ready access tools, commands or information for the current application.|
||Inspector window| – a type of dialog window that shows a list of the current attributes of a selected object and allows these parameters to be changed on the fly.|
||Frame| – a type of box within which a collection of graphical control elements can be grouped as a way to show relationships visually.|
||Canvas| – generic drawing element for representing graphical information.|
||Cover Flow – an animated, three-dimensional element to visually flipping through snapshots of documents, website bookmarks, album artwork, or photographs.|
||Bubble Flow| – an animated, two-dimensional element that allows users to browse and interact the entire tree view of a discussion thread.|
