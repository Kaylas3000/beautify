# Functional Specification Document

# Master and client hand



**DOCUMENT VERSION**  **0.8**



**AUTHORS**

| **Name** | **Role** | **Department** |
| --- | --- | --- |
| Sokolov Mykola |- technical implementation of the project <br> - ideas generator|   |
| Svitlana Sokolova|- user experience, design |   |



**DOCUMENT HISTORY**

| **Date** | **Version** | **Document Revision Description** | **Document Author** |
| --- | --- | --- | --- |
| 05/07/19 | 0.0 | Initial version. Basic ideas | Strogonova A. |
| 07/07/19 | 0.1 | Minor changes  | Sokolov M. |
| 06/08/19 | 0.2 | added some information about buttons, redaction of view of document  |   Strogonova A. |
| 07/08/19 | 0.3 |  several pictures of screen A from "Fluid" with discriptions <br> redact the dictionary of termins |  Strogonova A.   |
| 03/03/2021  | 0.4  | Added DMS specification, changed risks section.  | Sokolov M. |
| 04/03/2021  | 0.5  | Added authentication and localization sections.  | Sokolov M. |
| 04/03/2021  | 0.6  | Moved some sections to separate document. Overall improvement.  | Sokolov M. |


**APPROVALS**

| **Approval Date** | **Approved Version** | **Approver Role** | **Approver** |
| --- | --- | --- | --- |
|   |   | Technical specification  | Mykola Sokolov  |
|   |   | Functional specification  | Svitlana Sokolova  |

**Table of Contents**

1. [ Introduction ](#introduction)

1.1 [ Purpose of the document ](#purpose)

1.2 [ Project Scope ](#projectscope)

1.3 [ Scope of the document ](#scopedocument)

1.4 [ Related documents ](#relateddocuments)

1.5 [ Terms/Acronyms and Definitions ](#terms)

1.6 [ Risks and Assumptions ](#risks)

2. [ System/ Solution Overview ](#systemsolution)

2.1. [ Application Screen Flow ](#contextdiagram)

2.2. [ System Actors ](#systemactors)

2.3. [ Dependencies and Change Impacts ](#dependencies)

3. [ Functional Specifications ](#functionalspecifications)

3.1. [ Database management system ](#Database)

3.2. [ Authentication and authorization mechanism ](#Authentication)

3.3. [ Localization ](#Localization)

3.4. [ Billing (checkout) ](#Billing)

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

The application to provide the relationship between customers(С) and craftsmen (service providers, specialists) - hairdressers, makeup artists, nail art masters, cosmetologists, barber shops &amp; etc.

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
* Customers should be able to find the most desirable services nearby(in terms of price and quality).
* Opportunity for a specialist to plan your day more efficiently.
* Keeping a calendar for the accounting of working hours (dates and time of visits).
* A specialist can inform his clients about various promotions thereby increasing sales of his services.
* Attracting customers through targeted advertising. Customer expansion.
* The client can use the search filter based on the actual parameters of the location, free time, price range, reviews of other clients, verified photos.

<a name="scopedocument"></a>
## 1.3. Scope of the document


1. Preliminary analysis of data.
2. Technical details.
3. Interaction of application with users.
4. Interaction of users among themselves (specialists and customers).
5. The Basic design of the application.

<a name="relateddocuments"></a>
## 1.4 Related documents

| **Component** | **Name (with link to the document)** | **Description** |
| --- | --- | --- |
| Client  | [Client screens detailing ](https://github.com/Kaylas3000/beautify/blob/master/client-screens-detalisation.md)  | Specification of clients part  |
| Specialist  | [Specialist screens detailing ](https://github.com/Kaylas3000/beautify/blob/master/specialist-screens-detalisation.md)  | Specification of specialist part  |
|   | [User flow diagram ](https://github.com/Kaylas3000/beautify/blob/master/UserFlowDiagram.png)  | User flow diagram  |
|   | [ Simple test scenarios ](https://github.com/nzamb1/find-haircut/blob/master/basic_test_scenario.md) | list of basic test cases  |

<a name="terms"></a>
## 1.5 Terms/Acronyms and Definitions
[ Moved to Appenndix ](appendix)

<a name="risks"></a>
## 1.6 Risks and Assumptions

- The idea might be stolen or concurrency will bring a better application to the market.
- It is not known what part of the market hides its revenues and therefore will be interested a little in using the application.
- Masters will be able to use the application dishonestly.
- avoiding interest payment by masters(masters will take client contacts instead of using the app).
- Masters will be able to cheat "likes", resulting in distrust of the application. A systematic check of the quality of reviews is needed.
- Lack of media advertising. As a result, the application would not be interesting to an audience.
- It might be too difficult to implement all features in time so the customers might quickly lose interest in the app.


<a name="systemsolution"></a>
## 2.  System/ Solution Overview

Mobile application for android (Android mobile operating system 7.0 and newer) and iOS ( iOS mobile operating system 9.3.6 and newer)

The application should be correctly displayed on the screens of mobile phones with the variety screen resolutions like:
Proportions: 16:9 5:3 3:2
Size: Flagmans - iPhone 12, iPhone 11, iPhone SE, iPhone Xr (1792 x 828), iPhone X Plus (2688 x 1242), iPhone X(2436 x 1125),  iPhone 8 (1334 х 750), iPhone 8  (1920 х 1080) and minimal - 5 (1136 x 640) 4 (960 x 640).

Samsung Galaxy A10s, Samsung Galaxy A50,Samsung Galaxy A10, Redmi Note 8
Huawei Honor 10 Lite (1080 x 2340px) + 415ppi
Huawei Honor 8X (1080 x 2340px) + 397ppi



<a name="contextdiagram"></a>
## 2.1 Application Screen Flow

**Customers screen flow:**

![Application Screen Flow](https://github.com/Kaylas3000/beautify/blob/master/scenario-client.png)

**Specialist screen flow:**
![Application Screen Flow](https://github.com/Kaylas3000/beautify/blob/master/scenario-specialist.png)

<a name="systemactors"></a>
## 2.2. System Actors

### 2.2.1     User Roles and Responsibilities / Authority Requirements

| **User/Role** | **Example** | **Frequency of Use** | **Security/Access, Features Used** | **Additional Notes** |
| --- | --- | --- | --- | --- |
| _include the specified user/role such as Purchasing Manager, Dept Admin, Faculty, Student, etc_ | _include examples of real people  in the role_ | _describes how often they use the system. State Frequent, Occasional or Rare_ | _describe the features of the system available for the role and any security/access permissions that should be stated_ | _add any additional notes or supporting documentation as necessary_    |
| administrator |   | often  |   | Superuser. This user has access everywhere.  |
| developer     |   |        |   | Developer user role. Used for access to the app as developer  |
| costomer      |   | often  | REGISTRATION:add date: Name Surname e-mail password repeat password sign insign out <br> Home Page: 1. Сcould select the necessary section in the main menu (directory)- internal 1.1- use the filter when searching (date, time, minimum maximum price, location territorial- search by map- selection of S :- service selection- internal 1.1.1- choosing a convenient time- contact the S phone watches, etc. <br> 1. C can search services in the search bar <br>  2. C can entry to the S schedule (duplicate calendar) <br> 3. C can send a request for the selected time of servise <br>  4. C can receve notifications <br>  5. C can edit their profile <br> 6. C can create and redact list of their S <br>  7. help <br> 8.  feedback |   |
| specialist |   | often | S can edit own calendar:internal 1:- select customerinternal <br>  1.2clients- customer groups- choose a service- session date (start - end)- comment search for customers in the search barinvite customers <br> Add FB and other applications to attract customers add customer dataphone email birthday synchronization with a notebook create customer groupsnew customersblack listpassive clients |   |
| tester  |   | sometimes  |   | Testing user role. Will be assigned for testers.   |
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
+ the system of appointment

<a name="functionalspecifications"></a>
## 3. Functional Specifications
The application should be built on Flutter SDK, Google's UI toolkit for crafting natively compiled applications for mobile. The main programming language is Dart as it is a client-optimized language for fast apps development on any platform.

<a name="Database"></a>
### 3.1. Database management system

The application should be built on Cloud Firestore as it is a flexible, scalable database for mobile, web, and server development from Firebase and Google Cloud.

<a name="Authentication"></a>
### 3.2 Authentication and authorization mechanism

Authentication and authorization might be implemented using Google Firebase. It's available for Android as well as for iOS. User roles are described in [System Actors section](#systemactors).

Authentication should be available with

- Facebook
- Google
- Instagram
- Email

Requirements for authentication.
- The user should be able to logout.
- The user should be able to close the account. The account should be removed as well as user data after closing the account.
- User should see an error message in case of errors during authentication(like account does not exist, incorrect passord, no connection to backend etc..).

<a name="Localization"></a>
### 3.3 Localization

The application should support localization. All sections of the app should support translation to different languages. Translation to different languages should be in a separate file(for example xml).

<a name="Billing"></a>
### 3.3 Billing (checkout)
Users should be able to pay for the services by payment cards (credit or debit). Users should be able to add a card to their profile. Should be investigated if it's possible to use Google Pay, Apple pay and integrate them with the app (android and iPhone respectively).

### 3.4 In app messaging
The application should support sending and receiving messages (after making a deal between parties)

### 3.5 Appointment cancellation
The client or master should be able to cancel an appointment (no longer than 3 hours before the appointment). If an appointment is canceled in less than 3 hours then sanctions should be applied.

### 3.6 Geolocation
The application should support geolocation.  The application should identify and estimate the real geographic location of the device. So users should be able to find the closest service providers.

### 3.7 Push notifications
Specialists must be able to see the details of service requests submitted by users.
Customers should be able to receive updates
- bookings
- payments
- cancellations
- promotions and offers
- discounts

### 3.8 Booking History
Specialists as well as customers should be able to see past bookings and booking details like:
- booking time
- booking date
- ordered services
- service price

Specialists should be able to see reviews left by customers.

_Make sure each specification has a reference number and is explained in the following format._

| **Spec ID** | **Specification Description** | **Business Rules/ Data Dependency** |
| --- | --- | --- |
| _Specification Identifier_ | _Short explanation of the specification_ | _Any validation rules or business rules_ |

_Note: Section 3.1.4 and section 3.1.5 may be combined if there are a few functionalities on a particular page_


<a name="systemconfigurations"></a>
## 4. System Configurations


<a name="othersystemrequirements"></a>
## 5. Other System Requirements/ Non-Functional Requirements

<a name="reporting"></a>
## 6. Reporting Requirements

<a name="integration"></a>
## 7. Integration Requirements


<a name="exceptionhandling"></a>
## 7.1 Exception Handling/ Error Reporting


| **Exception/ Error ID** | **Error** | **Cause** | **Solution Strategy** |
| --- | --- | --- | --- |
|   |   |   |   |

<a name="datamigration"></a>
## 8. Data Migration/ Conversion Requirements

<a name="dataconversionstrategy"></a>
## 8.1 Data Conversion Strategy


<a name="dataconversionpreparation"></a>
8.2 Data Conversion Preparation


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
