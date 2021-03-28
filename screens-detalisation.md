
## Login and registration


![Login picture](https://github.com/Kaylas3000/beautify/blob/master/SignUp-1.png)

|  | **Login page** |
| --- | --- |
| **Primary Actor(s)**| specialist or client |
| **Stakeholders and Interest** | specialist or client |
| **Trigger** | entrance to login page |
| **Pre-conditions**  | user has been registered before | 
| **Post-conditions** |  | 
| **Main Success Scenario** |  1. visit STARTING-POINT — login page <br>  2. put data into edit fields (user id, password)<br> 3. click the login button <br> 4. Make sure GOAL-ACHIEVED - applicatiion main page> |
| **Extensions** | 1.login through social networks<br> 2.invalid login id<br> 3.retry confirmation code<br> 4.Invalid Email<br> 5.invalid characters entered in fields<br> 6.user with given id does not exists |
| **Priority** | high|
| **Special Requirements** |communication with the login system through social networks <br> communication with the login system by phone number|
|**Open Questions** |  |

![Registration picture](https://github.com/nzamb1/find-haircut/blob/master/SignUp-2.png)

| **1** | **Registration page** |
| --- | --- |
| **Primary Actor(s)**| specialist or client |
| **Stakeholders and Interest** | specialist or client |
| **Trigger** | entrance to registration page |
| **Pre-conditions** | user has not been registered before | 
| **Post-conditions** | the user receives his individual account and is registered | 
| **Main Success Scenario** |  1. visit STARTING-POINT — registration page <br>  2. put data into edit fields of registration data (name, telephone number, e-mail, social network)<br> 3. click the register button (join)<br> 4. Make sure GOAL-ACHIEVED - Go to the created profile page> |
| **Extensions** | 1.registration through social networks<br> 2.invalid phone number<br> 3.retry confirmation code<br> 4.Invalid Email<br> 5.invalid characters entered in fields<br> 6.user with given mail number already exists_ |
| **Priority** | high|
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
