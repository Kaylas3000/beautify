# All screens
![All screen](https://github.com/Kaylas3000/beautify/blob/master/Client-Figma-Screens/All-screens.png)
# Login and registration


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


# 1. Client
## 1.1 Dashboard
![Dashboard screen](https://github.com/Kaylas3000/beautify/blob/master/Client-Figma-Screens/Android%20-%2012CLI.png)


| **Object** | **Function** | **Notes** |
| --- | --- | --- |
|Search box|Search for offers. User types a search confition. Offers should be filtered according to search text.|At the top of the screen|
|Button “Find”||Located under search box from the left side.|
|Button “Map”||Located is under search box from the right side.|
|Filter button|When user click on the button then user is redirected to another page with different filters.||
|All offers|There is offers scrolling option.||
|Button "Book now"|Procedd of booking a service. User should be able to continue in booking a service by clicking this button||
|Picture of service provider|This is a picture that service provider(saloon) uploaded||

## 1.1 Filters
![Filters screen](https://github.com/Kaylas3000/beautify/blob/master/Client-Figma-Screens/Android%20-%2015CLI.png)

| **Object** | **Function** | **Notes** |
| --- | --- | --- |
|Menu back to the Dashboard|||
|Text line with name of the window.||
|Text with name of the filter “Gender”.||
| 3 radio buttons|User can apply a filter “Woman”/ “Man”/ “Kid”.||
|Text with name of the filter “Services”.||
|Different filters: ”Hair cut”, “Hair Styling”, “Hair Coloring”, “Trim & Shaving”, “Make up”, “Facial Make up”, “Manicure”, “Pedicure”, “Gel polish”, “Spa”, “Limphatic drainage massage”, “Classic massage”, “Relaxing massage”, “Men`s epilation”, “Waxing”, “Photoepilation”, “Sugaring”.||
|Text with name of the filter “Raiting”.||
|Filter "stars"|User should be able to filter salons with minimal required rating.|Default value is "any raiting"|
|Text with name of the filter “Distance”.||
|Distance filter(slider)|Allows client to adjust the distance from his\her location to the services. Services should be showed where distance is larger then filter.|Default value is 20 km|
|Text with name of the filter “Price”.||
|Price filter(slider)|Service should be shown in selected price range(lower and higher)|Default value is: form 0 to maximum|
|“Submit button” |When user clicks on submit button then filter is applied and user is redirected back to the dashboard.|On the button there is a text showing maximum available services and services after applying filter.|

## 1.2. Map
![Map screen](https://github.com/Kaylas3000/beautify/blob/master/Client-Figma-Screens/Android%20-%2019CLI.png)

| **Object** | **Function** | **Notes** |
| --- | --- | --- |
|Menu back to the Dashboard|||
|Text line with name of the request||
|Button back to the Menu||
|Button search||
|The screen displays the map. The map shows the location of the person and nearby services|After selecting a salon on the map, can go to the service page.|

## 1.3. Salon`s page
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

## 1.4. Book appointment
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

## 1.5. Payment
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

## 1.6. Add payment card
![Add payment card](https://github.com/Kaylas3000/beautify/blob/master/Client-Figma-Screens/Android%20-%207CLI.png)

| **Object** | **Function** | **Notes** |
| --- | --- | --- |
|Button "Menu"|Tapping on menu button open menu||
|Text line with name of the window||
|Button "Back" to the "Payment"||
|Below, credit cards displayed|Under credit cards are two buttons "Delete card" and "Add new card"|Credit cards can be one, two or more. If the user does not have a credit card, he can add a card by clicking the "Add new credit card" button. And the user redirected to the "Add New Card" page.||
|Button "Pay now"|When user click button, he redirected to the page "You payment was successful"||

## 1.7. Add new card
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
|Button "Add new card"|When user click button, he redirected to the page "Add payment card"||
||User can go to the page from the "Settings" page||
