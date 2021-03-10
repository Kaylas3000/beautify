# Functional tests

|**Test N** | **Test description**  | **Comments** |
| --- | --- | --- |
|   1   | Ensure the app has been launched by downloading and installing it for use. | |
|   2   | Verify that the mobile app display is adaptable to the device screen and also ensures all menus on the app are functioning. | |
|   3   | Verify that the text on the mobile app is readable and clear. | |
|   4   | Check that the app display is adaptable and amenable to the various display mode (i.e. landscape and portrait). | |
|   5   | Verify that the app does not stop the functioning of other apps in the mobile device. | |
|   6   | Is the device able to multitask as expected when the app is in use or running in the background? | |
|   7   | Can other applications perform satisfactorily once the app is installed? | |
|   8   | Verify that in the play screen, the back key allows the app to go back to the start-up screen. | |
|   9   | check that the app still operates as intended, if the device resumes from inactive mode or from the lock screen. | |
|   10  | Verify that the on-screen keyboard appears immediately the user attempt to enter a text. | |
|   11  | Check if the app behaves as designed if the mobile device is shaken | |
|   12  | Verify that the app still functions as designed when “battery low” notifications appear on the screen. | |
|   13  | Check that the app goes into the background when on call | |
|   14  | Check that the app still operates as designed when a message or notification pop-up from another app such as Facebook messaged, Instagram, etc. | |
|   15  | If the app comes with a users’ settings features, check if the app changes when some form of changes is affected by the user. | |
|   16  | Check the Performance of the app on the different internet networks such as 1G, 2G, 3G or 4 G network. | |
|   17  | Check that the app operates as intended when the device is connected to the internet through WiFi. | |
|   18  | Check that the app still operates normally when there is an incoming call or SMS. | |
|   19  | Check that the font size and style of the app are compatible and readable to the users | |
|   20  | Verify that that the loading time for the app is not too long. | |
|   21  | Check how the app function under different battery levels and temperatures. | |
|   22  | Verify that the app is not draining too much battery. | |
|   23  | Check that the app support image capturing. | |
|   24  | Check that the app does not log-out the user before the end of a session. | |
|   25  | Сheck for error messages, for example, «Network error. Please, try again later» in case of incorrect network operation. | |


# Standard login / logout can include such options:

registration: with a login and password, without a password, through the social network, etc.;
authorization: with a login and password, through the social network, etc,;
password recovery;
logout: standalone, after the session, etc.

## Positive scenarios:

Registration in the application is available with all the methods described in the terms of a technical specification.
You can register by filling in only the mandatory fields.
You can register by filling in all the fields completely.
It is possible to log in to the application after the registration. In this case, the entered data is correctly stored in the profile (e-mail, password, personal information, etc.).
Registering on one device, you can log in to another – the data is available and correctly stored on the server and available.
Logout works correctly.
Password recovery works correctly.

## Negative scenarios (the most obvious):

Re-registration for the same e-mail with the same login is not available.
Registration without filling in the mandatory fields is not available.
Registration, if all the fields are left blank, is unavailable.
Registration, if the format of the entered data does not meet the requirements, is not available.
Authorization with empty fields is not available.
Authorization with a wrong / deleted / blocked login is not available.
Authorization with incorrect password is not available.
