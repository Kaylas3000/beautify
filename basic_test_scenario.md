# Functional tests

|**Test N** | **Test description**  | **Comments** |
| --- | --- | --- |
|   1   | Ensure the app has been launched by downloading and installing it for use. | |
|   2   | Verify that the mobile app display is adaptable to the device screen and also ensures all menus on the app are functioning. | |
|   3   | Verify that the text on the mobile app is readable and clear. | |
|   4   | Verify that the app does not stop the functioning of other apps in the mobile device. | |
|   5   | Is the device able to multitask as expected when the app is in use or running in the background? | |
|   6   | Can other applications perform satisfactorily once the app is installed? | |
|   7   | check that the app still operates as intended, if the device resumes from inactive mode or from the lock screen. | |
|   8  | Verify that the on-screen keyboard appears immediately the user attempt to enter a text. | |
|   9  | Check if the app behaves as designed if the mobile device is shaken | |
|   10  | Verify that the app still functions as designed when “battery low” notifications appear on the screen. | |
|   11  | Check that the app goes into the background when on call | |
|   12  | Check that the app still operates as designed when a message or notification pop-up from another app such as Facebook messaged, Instagram, etc. | |
|   13  | Check if the app changes when some form of changes is affected by the user. | |
|   14  | Check the Performance of the app on the different internet networks such as 1G, 2G, 3G or 4 G network. | |
|   15  | Check that the app operates as intended when the device is connected to the internet through WiFi. | |
|   16  | Check that the app still operates normally when there is an incoming call or SMS. | |
|   17  | Verify that that the loading time for the app is not too long. | |
|   18  | Check how the app function under different battery levels and temperatures. | |
|   19  | Verify that the app is not draining too much battery. | |
|   20  | Check that the app does not log-out the user before the end of a session. | |
|   21  | Сheck for error messages, for example, «Network error. Please, try again later» in case of incorrect network operation. | |


# Standard login / logout can include such options:
|**Test N** | **Test description**  | **Comments** |
| --- | --- | --- |
|   1   | Registration: with a login and password, without a password, through the social network, etc.; | |
|   2   | Authorization: with a login and password, through the social network, etc,; | |
|   3   | Password recovery; | |
|   4   | Logout: standalone, after the session, etc. | |

## Positive scenarios:

|**Test N** | **Test description**  | **Comments** |
| --- | --- | --- |
|   1   | Registration in the application is available with all the methods described in the terms of a technical specification. | |
|   2   | User can register by filling in only the mandatory fields. | |
|   3   | User can register by filling in all the fields completely. | |
|   4   | It is possible to log in to the application after the registration. In this case, the entered data is correctly stored in the profile (e-mail, password, personal information, etc.). | |
|   5   | Registering on one device, you can log in to another – the data is available and correctly stored on the server and available. | |
|   6   | Logout works correctly. | |
|   7   | Password recovery works correctly. | |

## Negative scenarios (the most obvious):

|**Test N** | **Test description**  | **Comments** |
| --- | --- | --- |
|   1   | Re-registration for the same e-mail with the same login is not available. | |
|   2   | Registration without filling in the mandatory fields is not available. | |
|   3   | Registration, if all the fields are left blank, is unavailable. | |
|   4   | Registration, if the format of the entered data does not meet the requirements, is not available. | |
|   5   | Authorization with empty fields is not available. | |
|   6   | Authorization with a wrong / deleted / blocked login is not available. | |
|   7   | Authorization with incorrect password is not available. | |
