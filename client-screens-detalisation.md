# All screens
![All screen](https://github.com/Kaylas3000/beautify/blob/master/Client-Figma-Screens/All-screens.png)
![All screen](https://github.com/Kaylas3000/beautify/blob/master/Client-Figma-Screens/All-screens-login.png)

**Table of Contents**
1. [ Introduction ](#introduction)
2. [ Login and registration ](#login)
3. [ Dashboard ](#dashboard)
4. [ Filters ](#filters)
5. [ Map ](#map)
6. [ Salon's page ](#salonspage)
7. [ Book appointment ](#bookappointment)
8. [ Payment ](#payment)
9. [ Add payment card ](#addpaymentcard)
10. [ Add new card ](#addnewcard)

<a name="introduction"></a>
# 1. Introduction
This document describes only a Client(Customer) part. Service provider(specialist) part described in the [specialist document](https://github.com/Kaylas3000/beautify/blob/master/specialist-screens-detalisation.md).
The user should be able to register an account (select "client") on the SignUp Screen). After Registration user is redirected to the dashboard where he\she should be able to book a service like a Haircut, Makeup, Manicure, etc. Users should be able to filter services according to his\her location, price range, service name, etc. The user should be able to open a map where he\she should click on the nearest service and book it.

<a name="login"></a>
# 2. Login and registration


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

![Registration picture](https://github.com/Kaylas3000/beautify/blob/master/SignUp-2.png)

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

<a name="dashboard"></a>
# 3. Dashboard
![Dashboard screen](https://github.com/Kaylas3000/beautify/blob/master/Client-Figma-Screens/Android%20-%2012CLI.png)


| **Object** | **Function** | **Notes** |
| --- | --- | --- |
|Search box|Search for offers(services). User types a search condition. Offers should be filtered according to search text.|At the top of the screen|
|Button “Search”|Services should be filtered according to what is user typing in the search field|Located under search box from the left side.|
|Button “Map”||Located is under search box from the right side.|
|Button "Filter"|When the user clicks on the button then the user is redirected to another page with different filters.||
|All offers|There is an offers scrolling option.||
|Button "Book now"|Procedd of booking a service. User should be able to continue booking a service by clicking this button||
|Picture of service provider|This is a picture that the service provider(saloon) uploaded||

<a name="filters"></a>
# 4. Filters
![Filters screen](https://github.com/Kaylas3000/beautify/blob/master/Client-Figma-Screens/Android%20-%2015CLI.png)

| **Object** | **Function** | **Notes** |
| --- | --- | --- |
|Menu back to the Dashboard|||
|Text line with the name of the window.||
|Text with the name of the filter “Gender”.||
| 3 radio buttons|User can apply a filter “Woman”/ “Man”/ “Kid”.||
|Text with the name of the filter “Services”.||
|Different filters: ”Hair cut”, “Hair Styling”, “Hair Coloring”, “Trim & Shaving”, “Make up”, “Facial Make up”, “Manicure”, “Pedicure”, “Gel polish”, “Spa”, “Limphatic drainage massage”, “Classic massage”, “Relaxing massage”, “Men`s epilation”, “Waxing”, “Photoepilation”, “Sugaring”.|Filteres should be clickable. User should be able to select desired filer conditions.|
|Text with the name of the filter “Raiting”.||
|Filter "stars"|User should be able to filter salons with minimal required rating.|Default value is "any raiting"|
|Text with the name of the filter “Distance”.||
|Distance filter(slider)|Allows client to adjust the distance from his\her location to the services. Services should be shown where distance is larger than filter.|Default value is 20 km|
|Text with the name of the filter “Price”.||
|Price filter(slider)|Service should be shown in the selected price range(lower and higher)|Default value is form 0 to maximum|
|“Submit button” |When a user clicks on submit button then the filter is applied and the user is redirected back to the dashboard.|On the button, there is a text showing maximum available services and services after applying the filter.|

<a name="map"></a>
# 5. Map
![Map screen](https://github.com/Kaylas3000/beautify/blob/master/Client-Figma-Screens/Android%20-%2019CLI.png)

| **Object** | **Function** | **Notes** |
| --- | --- | --- |
|Menu back to the Dashboard|||
|Text line with name of the request||
|Button back to the Menu||
|Button search||
|The screen displays the map. The map shows the location of the person and nearby services|After selecting a salon on the map, can go to the service page.|

<a name="salonspage"></a>
# 6. Salon's page
![Salon screen](https://github.com/Kaylas3000/beautify/blob/master/Client-Figma-Screens/Android%20-%2017CLI.png)

| **Object** | **Function** | **Notes** |
| --- | --- | --- |
|Buton back to the Map|||
|At the top of the screen is a photo of the salon.|There is a possibility to scroll the photos.||
|Below is information about the services.|The "stars" button displays the rating of the service.||
|Text with name of the "Service"|A list of salon services with photos are displayed.||
|Below are icon "pin" with service address||
|Under text with name "Gallery"|There is a possibility to add photos with works of masters||
|Button "Book"|When user clicks on "Book" button and user is redirected to the page "Book appointment"||

<a name="bookappointment"></a>
# 7. Book appointment
![Book appointment](https://github.com/Kaylas3000/beautify/blob/master/Client-Figma-Screens/Android%20-%2016CLI.png)

| **Object** | **Function** | **Notes** |
| --- | --- | --- |
|Button "Menu"|Tapping on menu button open menu||
|Text line with name of the window||
|Button "Back" to the "Salon`s page"||
|"Slider"|There are 3 points on the slider. Each point is signed. Active position is highlighted in blue|First: "Book appointment", second: "Payment", third: "Finished"||
|Below, is line with month and arrows|Under, is the calendar|User can select day, month, year||
|text with name of the "Time"|User can select free time|Near, is slider with "AP" or "PM"||
|Text with name of the "Service"|Under is filter with type of service and icon "forward"||
|Text with name of the "Hair Specialist"|Bellow, are photo with specialists, who  provides these services|Each photo of a specialist is signed||
|Button "Procced to Payment"|When user click button, he redirected to the page "Payment"||

<a name="payment"></a>
# 8. Payment
![Payment](https://github.com/Kaylas3000/beautify/blob/master/Client-Figma-Screens/Android%20-%208CLI.png)

| **Object** | **Function** | **Notes** |
| --- | --- | --- |
|Button "Menu"|Tapping on menu button open menu||
|Text line with name of the window||
|Button "Back" to the "Salon`s page"||
|"Slider"|There are 3 points on the slider. Each point is signed. Active position is highlighted in blue|First: "Book appointment", second: "Payment", third: "Finished"||
|Text with name of the "Your payment information"||
|Text with name of the "Name of the service"(for ex. Zara`s salon)|The types of services of all selected services. The cost of all selected services (total payment ... CZK)||
|Text with name of the "Payment methods"|Under, are methods of payment: credit card or cash|User can select payment method. When user selected, a checkmark icon appears near the method||
|Button "Continue"|When user click button, he redirected to the page "Add payment card"||

<a name="addpaymentcard"></a>
# 9. Add payment card
![Add payment card](https://github.com/Kaylas3000/beautify/blob/master/Client-Figma-Screens/Android%20-%207CLI.png)

| **Object** | **Function** | **Notes** |
| --- | --- | --- |
|Button "Menu"|Tapping on menu button open menu||
|Text line with name of the window||
|Button "Back" to the "Payment"||
|Below, credit cards displayed|Under credit cards are two buttons "Delete card" and "Add new card"|Credit cards can be one, two or more. If the user does not have a credit card, he can add a card by clicking the "Add new credit card" button. And the user redirected to the "Add New Card" page.||
|Button "Pay now"|When user click button, he redirected to the page "You payment was successful" or page "Payment failed"||

<a name="addnewcard"></a>
# 10. Add new card
![Add new card](https://github.com/Kaylas3000/beautify/blob/master/Client-Figma-Screens/Android%20-%206CLI.png)

| **Object** | **Function** | **Notes** |
| --- | --- | --- |
|Button "Menu"|Tapping on menu button open menu||
|Text line with name of the window||
|Button "Back" to the "Add payment card"||
|Below, icon credit cards displayed||
|Text line with "Card holder’s name"|Under, is rectangle|User can write his name||
|Text line with "Card number"|Under, is rectangle|User can write his card number||
|Text line with "Expiry Date"|Under, is rectangle|User can write expiry date his card||
|Text line with "CVV"|Under, is rectangle|User can write CVV his card||
|Button "Add new card"|When user click button, he redirected to the page "Payment card has been added" and then "Add payment card"||
||User can go to the page from the "Settings" page||

# 10. Finished
![Finished](https://github.com/Kaylas3000/beautify/blob/master/Client-Figma-Screens/Android%20-%2018CLI.png)

| **Object** | **Function** | **Notes** |
| --- | --- | --- |
|Button "Menu"|Tapping on menu button open menu||
|Text line with name of the window||
|Button "Back" to the "Payment"||
|"Slider"|There are 3 points on the slider. Each point is signed. Active position is highlighted in blue|First: "Book appointment", second: "Payment", third: "Finished"||
|Below, window "Order detail" displayed|Information displayed with data, time, price and address||
|Button "Add a reminder"|??add Google reminder??||

# 11. Payment card has been added
![Payment card has been added](https://github.com/Kaylas3000/beautify/blob/master/Client-Figma-Screens/Android%20-%209CLI.png)


| **Object** | **Function** | **Notes** |
| --- | --- | --- |
|Icon check mark is on the top||
|Text with information "Payment card has been added. You will recive a confirmation of your order by email"||
|Button "Got it"|User redirected to the page "Add payment card"||

# 12. Payment failed
![Payment failed](https://github.com/Kaylas3000/beautify/blob/master/Client-Figma-Screens/Android%20-%2010CLI.png)

| **Object** | **Function** | **Notes** |
| --- | --- | --- |
|Сross icon is on the top||
|Text with information "Payment failed. Unfortunately payment was rejected"|If user writes incorect data about credit card on the page "Add new card", he will turn up on this page||
|Button "Try again"|User redirected to the page "Add payment card"||

# 13. You payment was successful
![You payment was successful](https://github.com/Kaylas3000/beautify/blob/master/Client-Figma-Screens/Android%20-%2011CLI.png)

| **Object** | **Function** | **Notes** |
| --- | --- | --- |
|Icon check mark is on the top||
|Text with information "You payment was successful. Thank you. You will recive an email shortly"||
|Button "Done"|User redirected to the page "Dashboard"||

# 14. Feedback
![Feedback](https://github.com/Kaylas3000/beautify/blob/master/Client-Figma-Screens/Android%20-%2020CLI.png)

| **Object** | **Function** | **Notes** |
| --- | --- | --- |
|Button "Menu"|Tapping on menu button open menu||
|Text line with name of the window||
|Button "Back" to the "Salon's page"||
|Text with "Your review. What are you feel about this service?"||
|Below, "stars"|User can rate, choosing the number of stars||
|Under, is a field for entering feedback||
|Near, is button for sent feedback||

# 15. Menu
![Menu](https://github.com/Kaylas3000/beautify/blob/master/Client-Figma-Screens/Android%20-%202CLI.png)

| **Object** | **Function** | **Notes** |
| --- | --- | --- |
|Button "Back"|Clicking on the "back" button redirects back to the page from which user went||
|Below, is photo profile|Under photo are username and email||
