 `Test Report

` `(CogniOpen - Nurturing Memory Wellness for Cognitive Impairment)



` `Submitted to:



` `University of Maryland Global Campus in partial fulfillment of the course Software Engineering Capstone (SWEN 670)



` `Submitted By: Team B



` `Fall Semester 2023



` `Version 1.0





` `November 4, 2023

` `Department of Software Engineering

` `University of Maryland Global Campus (UMGC)



\

# **Table of Contents**
[**1. EXECUTIVE SUMMARY	**4****](#_toc150003879)

[**2. INTRODUCTION	**4****](#_toc150003880)

[**2.1 Test Objectives**	4](#_toc150003881)

[**2.2 Test Scope**	4](#_toc150003882)

[**2.3 Documents**	5](#_toc150003883)

[**2.4 Definitions, Abbreviations, and Acronyms**	5](#_toc150003884)

[**2.5 Stakeholders**	7](#_toc150003885)

[**3. REFERENCES	**7****](#_toc150003886)

[**3.1 Test Methodology**	7](#_toc150003887)

[**3.2 Pass vs Fail Criteria**	8](#_toc150003888)

[**3.3 Defect Severity Levels**	8](#_toc150003889)

[**3.4 Tests Conducted**	8](#_toc150003890)

[**4. REQUIREMENTS TRACEABILITY MATRIX	**9****](#_toc150003891)

[**5. FUNCTIONAL TEST EXECUTION FINDINGS	**10****](#_toc150003892)

[**TC-1 Login with Valid Credentials**	11](#_toc150003893)

[**TC-2 Deny Login with Invalid Credentials**	11](#_toc150003894)

[**TC-3 Request to Create an Account**	12](#_toc150003895)

[**TC-4 Home Interface Test Cases**	13](#_toc150003896)

[**TC-5 Verify Virtual Assistant Interaction**	15](#_toc150003897)

[**TC-6 Verify Virtual Assistant Receives Transcripts**	17](#_toc150003898)

[**TC-7 Activate/Deactivate Record Audio**	18](#_toc150003899)

[**TC-8 Play/Stop Preview Recorded Audio**	19](#_toc150003900)

[**TC-9 Start New Recording from Audio Preview Screen**	20](#_toc150003901)

[**TC-10 Delete Recorded Audio from Audio Preview Screen**	21](#_toc150003902)

[**TC-11 View Profile Information**	22](#_toc150003903)

[**TC-12 Edit Profile Information**	23](#_toc150003904)

[**TC-13 View Guided Tour**	24](#_toc150003905)

[**TC-14 Cancel Guided Tour**	25](#_toc150003906)

[**TC-15 Onboarding Voice Assistance**	26](#_toc150003907)

[**TC-16 Logout Application**	27](#_toc150003908)

[**6. TEST RESULTS	**27****](#_toc150003909)

[**6.1 Functional Test Results**	27](#_toc150003910)

[**7.  SUMMARY	**28****](#_toc150003911)


# **Table of Contents**

[Table 1: Project Documents	5](#_toc150003912)

[Table 2: Definitions, Acronyms, and Abbreviations	6](#_toc150003913)

[Table 3: Stakeholders	7](#_toc150003914)

[Table 4: Requirements Traceability Matrix	9](#_toc150003915)

[Table 5: Requirements Traceability Matrix Continued	10](#_toc150003916)

[Table 6: TC-1 Valid Login	11](#_toc150003917)

[Table 7: TC-2 Deny Login	11](#_toc150003918)

[Table 8: TC-3 Create Account	12](#_toc150003919)

[Table 9: TC-4 Home Screen	13](#_toc150003920)

[Table 10: TC-4 Home Screen Continued	14](#_toc150003921)

[Table 11: TC-5 Virtual Assistant	16](#_toc150003922)

[Table 12: TC-5 Virtual Assistant Continued	16](#_toc150003923)

[Table 13: TC-6 Virtual Assistant Transcriptions	17](#_toc150003924)

[Table 14: TC-7 Activate/Deactivate Audio Recording	18](#_toc150003925)

[Table 15: TC-8 Play/Pause Audio Recording	19](#_toc150003926)

[Table 16: TC-9 Start New Audio Recording	20](#_toc150003927)

[Table 17: TC-10 Delete Recorded Audio	21](#_toc150003928)

[Table 18: TC-11 View Profile	22](#_toc150003929)

[Table 19: TC-12 Edit Profile	23](#_toc150003930)

[Table 20: TC-13 View Guided Tour	24](#_toc150003931)

[Table 21: TC-14 Cancel Guided Tour	25](#_toc150003932)

[Table 22: TC-15 Onboarding Assistant	26](#_toc150003933)

[Table 23: TC-16 Application Logout	27](#_toc150003934)

[Table 24: Test Metrics	28](#_toc150003935)

[Table 25: Bug Report	28](#_toc150003936)
**\

# <a name="_toc150003879"></a>**1. Executive Summary**
`       `The purpose of this test report is to document the scope and approach of all testing activities for the CogniOpen Application. This report identifies the items that have been tested, and details regarding said tests. This document serves as a reference for various stakeholders involved in the application development process. Furthermore, this serves as a reference specifically for stakeholders involved directly in the testing process. Stakeholders involved in the testing process include developers, project managers, testers, and end-users. The test report gives clear directions on the testing approach, including the testing environment, testing tools, test data, and test deliverables.
# <a name="_toc150003880"></a>**2. Introduction**
## <a name="_toc150003881"></a>**2.1 Test Objectives**
`       `The purpose of the tests is to confirm that the application meets the requirements set with our client. In specific the functionality, performance, security, and compatibility requirements will be confirmed. Furthermore, these tests show any unforeseen defects or limits found within the app. These tests consist of both functional and non-functional tests. 
## <a name="_toc150003882"></a>**2.2 Test Scope**
`       `This project is completed in conjunction with another development team. For the purposes of this project the following sections will define portions of the application that are in scope and out of scope for Team B.

`       `The testing activities were focused on the functional, non-functional, and UI testing of the features listed below, and the testing approach for manual test cases ensured comprehensive coverage. The manual test case deliverables include the test case name, description, requirements, prerequisites, test data, test steps, expected results, test environment, pass/fail criteria, and assumptions. In addition, the test report documents test phases, which include unit testing, functional testing, integration testing, regression testing, and user-acceptance testing. The testing was conducted on various mobile devices with different screen sizes, resolutions, and operating systems, and it was performed in a controlled environment to ensure the accuracy and reliability of the results. 

`       `The following features are part of the scope of work for Team B and are covered by the test cases in this document:

- Registering and logging in to the application
- Accessing features through the <a name="_int_nmdqqjdd"></a>Home interface
- Interacting with the Virtual Assistant
- Recording audio
- Using the hamburger menu
- Managing the user profile
- Viewing the guided tour
## <a name="_toc150003883"></a>**2.3 Documents**

|**Document**|**Version**|**Date**|
| :- | :- | :- |
|Project Plan (PPL) |1\.2|10/28/2023|
|Software Requirements Specification (SRS) |1\.2|10/28/2023|
|Technical Design Document (TDD)|1\.1|10/28/2023|
|Test Plan (TP)|1\.1|10/28/2023|
|Programmer Guide (PG) |1\.0|10/28/2023|
|Deployment and Operations Guide (DOG) |1\.0|10/28/2023|
|Software Test Report (STR) |-|-|
|User Guide (UG) |-|-|
|Traceability Matrix (TM) |-|-|

<a name="_toc149669513"></a><a name="_toc150003912"></a>Table 1: Project Documents
## <a name="_toc150003884"></a>**2.4 Definitions, Abbreviations, and Acronyms**
**

|**Term**|**Definition**|
| :- | :- |
|**ADO**|Azure DevOps|
|**API**|Application Programming Interface|
|**App** |A program that is included on the User’s mobile device|
|**AWS**|Amazon Web Services|
|**Cora**|CogniOpen Remote Assistant|
|**HIPPA**|Health Insurance Portability and Accountability Act|
|**HTTPS**|Hypertext Transfer Protocol Secure|
|**IAM**|Identity and Access Management|
|**IDE**|Integrated development environment|
|**iOS** |iPhone Operating System|
|**MB**|Megabytes|
|**Mobile Device** |A smart phone, tablet, or some other portable computer with either the iOS or Android operating system|
|**MVC**|Model View Controller|
|**OS**|Operating System|
|**REST**|Representational State Transfer|
|**SDK**|Software Development Kit|
|**SNS**|Simple Notification Service|
|**TDD** |Technical Design Document|
|**UI**|User Interface |
|**UMGC**|University of Maryland Global Campus|
|**UX**|User Experience|

<a name="_toc150003913"></a>Table 2: Definitions, Acronyms, and Abbreviations
**\

## <a name="_toc150003885"></a>**2.5 Stakeholders**

|**Name** |**Roles** |
| :- | :- |
|Dr. Mir Assadullah |Customer |
|Roy Gordon |Project Manager Mentor |
|Robert Wilson |DevSecOps Mentor |
|Abebe Natea|<p>Technical Writer</p><p>Lead Test Engineer</p>|
|Alexis (Alex) Shannon |<p>Software Developer</p><p>Business Analyst</p>|
|Edward Devine |<p>Project Manager</p><p>Lead Business Analyst</p>|
|Eyerusalme (Jerry) Gebrehiwot |<p>UI/UX Developer</p><p>Software Developer</p>|
|Gabriel Gomes |UI/UX Developer|
|John Hamilton |<p>Software Developer</p><p>Technical Writer</p>|
|Malachi Jamison |<p>Lead UI/UX Developer</p><p>Software Developer</p>|
|Sean Mirani |<p>Lead Software Developer</p><p>Business Analyst</p>|
|Zac Cappella |<p>Lead Technical Writer</p><p>Test Engineer</p>|

<a name="_toc150003914"></a>Table 3: Stakeholders
# <a name="_toc150003886"></a>**3. References**
## <a name="_toc150003887"></a>**3.1 Test Methodology**
`       `Testing for CogniOpen primarily assesses the function of the system and is therefore composed primarily of functional test cases. Test cases were designed based on user stories and requirements, ensuring comprehensive coverage. Development of test cases has been divided by User Interface (UI) screens. Each screen was analyzed in order to determine and note all possible user interactions. Each interaction was then given a test case. Finally, every test case was given an expected behavior, and tested by a test engineer. 

`       `Any non-functional requirements not applicable to functional tests are handled in the non-functional tests section. These are not self-contained tests that can be performed on the system. Non-functional tests were referenced whenever the system performs any relevant activity that cannot be handled by self-contained tests that can be performed on the system. Additionally, due to resource limitations, some non-functional tests were deemed untestable in the current build environment.
## <a name="_toc150003888"></a>**3.2 Pass vs Fail Criteria**
`       `For a test to be considered passed, the expected result should occur when the function is tested. Furthermore, the delivery of this result should cause no unexpected errors during operation of the application. Test case results that do not meet these criteria will be considered failed. Test case functions that meet all of these criteria are considered passed.
## <a name="_toc150003889"></a>**3.3 Defect Severity Levels**
`       `**Critical:** These are issues that prevent core functionality within CogniOpen. These are errors which cause the system to cease to operate in a way that fulfills the stakeholders' requirements regarding minimum function of the app. Errors upon startup and shutdown are included. Errors that cause the app to crash are also considered critical level errors. Finally, the main functions not being fully operational are considered critical defects.

`       `**Major:** These are issues that make the app significantly more difficult to use. The app may still function on a basic level, but basic functions become severely limited during major defects. Since this app was created for special needs individuals, judgment on major issues will be strict. 

`       `**Minor:** These are smaller issues that make the app inconvenient for the user but should still maintain proper functionality. These issues will be noticeable, but not distractingly so. Users should not have issues working around defects at this level.

`       `**Cosmetic:** These are small visual issues, some that users may not even notice. These are not high priority issues but should be noted and taken care of. 
## <a name="_toc150003890"></a>**3.4 Tests Conducted** 
`       `The CogniOpen application will undergo multiple testing phases to ensure its proper function and user-friendliness. These phases include unit testing, functional testing, integration testing, regression testing, and user acceptance testing. Unit testing will check the code for UI rendering and functionality. Functional testing will be performed by test engineers to ensure that the feature being developed meets system requirements and user needs. Integration testing will ensure that new features have not broken the interaction between existing features and core functionality. Regression testing will exercise every possible feature within the application to test all non-functional requirements. Finally, the customer will perform user acceptance testing to ensure that the requirements provided by the customer are met. If issues arise during any of these testing phases, the teams will work together to resolve them and provide a new version of the software.
# <a name="_toc150003891"></a>**4. Requirements Traceability Matrix**
`       `A Requirements Traceability Matrix (RTM) was maintained to track the coverage of test cases against requirements.

|**Test Case ID**|**Test Case Title**|<p>**SRS**</p><p>**Requirement #**</p>|**Test Description**|**Result**|
| :- | :- | :- | :- | :- |
|**TC-1**|Login with Valid Credentials|3\.1.1|A user can login to the CogniOpen application with valid user credentials.| |
|**TC-2**|Deny Login with Invalid Credentials|3\.1.1|A user cannot login to the CogniOpen application with invalid user credentials.||
|**TC-3**|Request to Create an Account|3\.1.8|A user can request to create an account.||
|**TC-4**|Home Interface |3\.1.1|Verify that the home screen application button features functions correctly and meets all specified requirements. ||
|**TC-5**|Verify Virtual Assistant Interaction|3\.1.2|Check if the Virtual Assistant screen works as expected. Users should be able to interact with the AI assistant through text input, voice input, and responses.||
|**TC-6**|Verify Virtual Assistant Receives Transcripts||Verify that the Virtual Assistant screen in the application receives transcripts from the Gallery when the user navigates from there. Users should be able to ask questions about the transcript.||
|**TC-7**|Activate/Deactivate Record Audio|3\.1.3|Verify if tapping the “Start Audio Recording” circular button starts recording and changes to square button and tapping "Stop Recording" button ends recording and switches to preview screen.||
<a name="_toc150003915"></a>Table 4: Requirements Traceability Matrix



|**Test Case ID**|**Test Case Title**|<p>**SRS**</p><p>**Requirement #**</p>|**Test Description**|**Result**|
| :- | :- | :- | :- | :- |
|**TC-8**|Play/Stop Preview Recorded Audio|3\.1.7|Verify that the on the “Play Preview” button starts playing the recorded audio when tapped. Verify that the on the “Stop Preview” button stop playing the recorded audio when tapped.||
|**TC-9**|Start New Recording from Audio Preview Screen|3\.1.7|To start a new recording, simply press the "New Recording" button, this will begin capturing new audio. ||
|**TC-**10|Delete Recorded Audio from Audio Preview Screen|3\.1.8|To delete a recorded audio, press the “Trash Can" icon to remove the recording from your device.||
|**TC-11**|View Profile Information|3\.1.9|A user can successfully view their profile information in the application.||
|**TC-12**|Edit Profile Information|3\.1.9|A user can successfully edit their profile information in the application.||
|**TC-13**|View Guided Tour|3\.1.10|The guided tour feature is designed to assist users in navigating the system and understanding its functionalities. The guided tour is accessible from the system's interface and provides a step-by-step tutorial on how to use the system's key features.||
|**TC-14**|Cancel Guided Tour|3\.1.10|A user can decide to cancel the guided tour, they can do so at any point during the tutorial by clicking on the cancel button provided on the screen.||
|**TC-15**|On-boarding Voice Assistance|3\.1.11|The virtual assistant welcomes the user and provides an overview of the system. It then proceeds to guide the user through a series of steps to complete the necessary tasks.||
|**TC-16**|Logout Application|3\.1.6|Verify that the logout functionality of the application works as expected and meets all specified requirements.||
<a name="_toc150003916"></a>Table 5: Requirements Traceability Matrix Continued
# <a name="_toc150003892"></a>**5. Functional Test Execution Findings** 
`       `Below are the functional tests that were carried out showing the respective results of the different test cases.
**\

### <a name="_toc150003893"></a>**TC-1 Login with Valid Credentials**

|**Description**|A user can login to the CogniOpen application with valid user credentials.|
| :- | :- |
|**Requirements**|The application shall authenticate and redirect a user to the home screen when they enter valid login information and tap the login button.|
|**Test Steps**|<p>1. Launch the CogniOpen application from the device</p><p>2. User taps the “Login in Here” button.</p><p>3. Users enter their biometric authentication information.</p>|
|**Expected Result**|The user is logged in and is redirected to the Home Interface|
|**Assumptions**|<p>- The user has previously registered with the application</p><p>- The user is connected to the internet</p><p>- The application is active and able to receive requests</p><p>- The application is able to communicate with the backend database services</p>|
|**Actual Result**|The application prompted for biometric authentication and redirected to the home screen.|
|**Pass/Fail**|Pass|

<a name="_toc150003917"></a>Table 6: TC-1 Valid Login
### <a name="_toc150003894"></a>**TC-2 Deny Login with Invalid Credentials**

|**Description**|A user cannot login to the CogniOpen application with invalid user credentials.|
| :- | :- |
|**Requirements**|The application shall deny users access to the application if they enter invalid user credentials and display a generic login error message.|
|**Test Steps**|<p>1. Launch the CogniOpen application from the device</p><p>2. User taps the “Login in Here” button</p><p>3. Users enter their biometric authentication information.</p>|
|**Expected Result**|The application does not redirect the user to Home Interface and displays an error message to the user.|
|**Assumptions**|<p>- The user did not register with the application</p><p>- The user is connected to the internet</p><p>- The application is active and able to receive requests</p><p>- The application can communicate with the backend database services</p>|
|**Actual Result**|The application prompted for biometric authentication and denied when given invalid credentials.|
|**Pass/Fail**|Pass|

<a name="_toc150003918"></a>Table 7: TC-2 Deny Login
**\

### <a name="_toc150003895"></a>**TC-3 Request to Create an Account**

|**Description**|A user can request to create an account.|
| :- | :- |
|**Requirements**|The application shall allow users to create a new account.|
|**Test Steps**|<p>1. Launch the CogniOpen application from the device</p><p>2. User taps the “Create Account” button</p><p>3. Users enters first name, last name and email</p><p>4. Users taps the “Create Account” button.</p><p></p>|
|**Expected Result**|The application creates a new user account with the input information and redirects to the user to the onboarding screen.|
|**Assumptions**|<p>- The user is connected to the internet</p><p>- The application is active and able to receive requests</p><p>- The application can communicate with the backend database services</p>|
|**Actual Result**|A user account was created and was redirected to the Home Screen|
|**Pass/Fail**|Pass|

<a name="_toc150003919"></a>Table 8: TC-3 Create Account
**\

### <a name="_toc150003896"></a>**TC-4 Home Interface Test Cases**

|**Description**|<p>This test case is designed to verify that the home screen application with six button features functions correctly and meets all specified requirements. The application contains six buttons that lead to different features and functionalities. The main objective of this test case is to ensure that all the buttons and features work as expected and that the application is user-friendly and easy to navigate. The six features are as follows Team B responsibility:</p><p>1. Virtual Assistant Button </p><p>2. Record Audio Button</p><p>3. Guided Tour Button</p><p>4. Home Button</p><p>5. Menu Button</p><p>6. Back Button</p>|
| :- | :- |
|**Requirements**|<p>- The home screen will allow users to access all the application’s main features. The home screen application should display buttons with their respective icons and labels to users upon logging in.</p><p>- Each button should lead to the expected feature or functionality </p><p>- The buttons should be responsive when clicked </p><p>- All UI elements, such as buttons and text boxes, should be responsive and functional –</p><p>- All required data should be displayed accurately and consistently throughout the application </p><p>- User input should be accepted and processed correctly by the application </p><p>- The application should be usable in all supported device orientations and screen sizes</p>|
|**Test Steps**|<p>1. Verify that the application is installed and configured correctly on the device.</p><p>2. Launch the CogniOpen application from the device </p><p>3. User taps the “Login in Here” button.</p><p>4. User enters their biometric authentication information.</p><p>5. Verify that the home screen displays all six buttons with their respective icons and labels. </p><p>6. Test each button by clicking on it and verify that it leads to the expected feature or functionality.</p><p>7. Verify that the buttons are responsive and that they highlight when clicked.</p><p>8. Test that all UI elements, such as buttons and text boxes, are responsive and functional.</p><p>9. Verify that all required data is displayed accurately and consistently throughout the application.</p><p>10. Test that user input is accepted and processed correctly by the application.</p><p>11. Verify that the application can be used in all supported device orientations and screen sizes.</p><p></p>|
<a name="_toc150003920"></a>Table 9: TC-4 Home Screen

|**Expected Result**|<p>- All buttons and features are displayed as expected.</p><p>- All features should open and load without any errors or crashes.</p><p>- The feature's UI elements should be responsive and functional.</p><p>- User input should be accepted and processed correctly by the feature.</p><p></p>|
| :- | :- |
|**Assumptions**|<p>- The user is connected to the internet</p><p>- The application is active and able to receive requests</p><p>- The application can communicate with the backend database services</p>|
|**Actual Result**|All home screen functionality is acting as expected.|
|**Pass/Fail**|Pass|

<a name="_toc150003921"></a>Table 10: TC-4 Home Screen Continued
**\

### <a name="_toc150003897"></a>**TC-5 Verify Virtual Assistant Interaction**

|**Description**|Verify that the Virtual Assistant screen in the application functions as expected, allowing users to interact with the AI assistant through text input, voice input, and receiving responses.|
| :- | :- |
|**Requirements**|<p>- The Virtual Assistant screen in the CogniOpen application must allow users to interact with the AI assistant through text input, voice input, and receiving responses. </p><p>- The Virtual Assistant must accurately recognize and respond to user inputs, including text-based and voice-based queries.</p><p>- The chat history of the conversation between the user and the Virtual Assistant must be displayed and maintained until the user closes the application or navigates to a different screen.</p>|
|**Test Steps**|<p>1. Launch the CogniOpen application from the device.</p><p>2. User taps the “Login in Here” button.</p><p>3. Users enter their biometric authentication information.</p><p>4. Navigate to the Virtual Assistant screen </p><p>5. Observe the Virtual Assistant screen and verify the presence of the following elements:</p><p>6. A text box for user input (keyboard input).</p><p>7. An option to enable microphone input (voice input) as seen in Figure 5 of the TDD.</p><p>8. Chat history displaying previous interactions.</p><p>9. Virtual Assistant responses or options presented to the user.</p><p>**Interaction with the Virtual Assistant:**</p><p>10. Enter a text-based question or request in the text box and tap the "Send" button. </p><p>11. Enable microphone input (if available) and speak a question or request. </p><p>12. Tap on any buttons or links presented by the Virtual Assistant within the conversation. </p><p>13. Continue the conversation by asking multiple questions or making requests. </p>|
|**Expected Result**|<p>- The Virtual Assistant responds with a relevant text-based reply or presents options if applicable.</p><p>&emsp;- The Virtual Assistant accurately recognizes and responds to voice input, providing text-based replies or options.</p><p>&emsp;- The Virtual Assistant maintains context and responds appropriately to each user input.</p>|
|**Assumptions**|<p>- The user is connected to the internet</p><p>- The application is active and able to receive requests</p><p>- The application can communicate with the backend database services</p><p>- Internet connectivity is available for Virtual Assistant functionality.</p><p>- The Virtual Assistant's natural language processing (NLP) capabilities are properly configured and connected to the internet for processing user queries.</p>|

<a name="_toc150003922"></a>Table 11: TC-5 Virtual Assistant

|**Actual Result**|The virtual assistant receives user input, responds, and provides feedback appropriately.|
| :- | :- |
|**Pass/Fail**|Pass|

<a name="_toc150003923"></a>Table 12: TC-5 Virtual Assistant Continued
**\

### <a name="_toc150003898"></a>**TC-6 Verify Virtual Assistant Receives Transcripts**

|**Description**|Verify that the Virtual Assistant screen in the application receives transcripts from the Gallery when the user navigates from there, allowing users to ask questions about the transcript.|
| :- | :- |
|**Requirements**|<p>- The Virtual Assistant screen in the CogniOpen application must allow users to interact with the AI assistant through text input, voice input, and receiving responses. </p><p>- The Virtual Assistant must accurately recognize and respond to user inputs, including text-based and voice-based queries.</p><p>- The Virtual Assistant must be able to receive a conversation transcript and be able to interpret it and respond to questions about it.</p><p>- The chat history of the conversation between the user and the Virtual Assistant must be displayed and maintained until the user closes the application or navigates to a different screen.</p>|
|**Test Steps**|<p>1. Launch the CogniOpen application from the device.</p><p>2. User taps the “Login in Here” button.</p><p>3. Users enter their biometric authentication information.</p><p>4. Navigate to the Gallery screen </p><p>5. Tap on a conversation.</p><p>6. Tap on the “Ask Cora” button.</p><p>7. Verify the app redirects to the Virtual Assistant screen.</p><p>**Interaction with the Virtual Assistant:**</p><p>8. Enter a text-based question or request, related to the transcript selected in step 5, in the text box. Then tap the "Send" button. </p><p>9. Continue the conversation by asking multiple questions or making requests. </p>|
|**Expected Result**|<p>- The Virtual Assistant responds with a relevant text-based reply that demonstrates understanding of the transcript.</p><p>&emsp;- The Virtual Assistant maintains context of both the transcript and previous messages and responds appropriately to each user input.</p>|
|**Assumptions**|<p>- The user is connected to the internet</p><p>- The application is active and able to receive requests</p><p>- The application can communicate with the backend database services</p><p>- There is at least one conversation stored in the Gallery.</p><p>- Internet connectivity is available for Virtual Assistant functionality.</p><p>- The Virtual Assistant's natural language processing (NLP) capabilities are properly configured and connected to the internet for processing user queries.</p>|
|**Actual Result**|Virtual assistant received transcriptions and provided a summary.|
|**Pass/Fail**|Pass|

<a name="_toc150003924"></a>Table 13: TC-6 Virtual Assistant Transcriptions
### <a name="_toc150003899"></a>**TC-7 Activate/Deactivate Record Audio**

|**Description**|Verify that the “Start Audio Recording” circular button on the Record Audio screen initiates the recording process when tapped. Verify that the circular button is replaced by a square-shaped button during recording, indicating that recording is in progress. Verify that tapping the "Stop" button ends the recording and transitions to the preview screen.|
| :- | :- |
|**Requirements**|<p>- The CogniOpen application must have a “Start Audio Recording” circular button on the Record Audio screen that initiates the recording process when tapped.</p><p>- During recording on the Record Audio screen, the circular button must be replaced by a square-shaped button to indicate that recording is in progress. The timer must also start counting.</p><p>- The Record Audio screen must feature a " Stop Audio Recording" " button that ends the recording when tapped, transitioning to the preview screen.</p><p></p>|
|**Test Steps**|<p>1. Launch the CogniOpen application.</p><p>2. User taps the “Login in Here” button.</p><p>3. Users enter their biometric authentication information.</p><p>4. Navigate to the Record Audio screen.</p><p>5. Tap the “Start Audio Recording” circular button in the center of the screen.</p><p>6. Check if the timer has started and accurately count during recording.</p><p>7. While recording is in progress (with the square-shaped button displayed), tap the "Stop" button.</p>|
|**Expected Result**|<p>- Tapping the “Start Audio Recording” circular button starts the recording. </p><p>&emsp;- The circular button is replaced by a square-shaped button, indicating that recording is in progress. The timer starts counting.</p><p>&emsp;- Tapping the "Stop Audio Recording" button ends the recording and transitions to the audio preview screen</p>|
|**Assumptions**|<p>- The CogniOpen application is properly installed and functioning on the test device.</p><p>- The device's operating system is compatible with the application.</p><p>- The user has successfully logged into the application and navigated to the Record Audio screen.</p>|
|**Actual Result**|Audio started recording immediately and stopped when it was paused.|
|**Pass/Fail**|Pass|

<a name="_toc150003925"></a>Table 14: TC-7 Activate/Deactivate Audio Recording
### <a name="_toc150003900"></a>**TC-8 Play/Stop Preview Recorded Audio**

|**Description**|Verify that the on the “Play Preview” button starts playing the recorded audio when tapped. Verify that the on the “Stop Preview” button stop playing the recorded audio when tapped.|
| :- | :- |
|**Requirements**|<p>- The CogniOpen application must have a “Play Preview” button on the Record Audio screen that initiates the recorded audio when tapped.</p><p>- The Record Audio screen must feature a " Stop Preview” button that stops the recorded audio when tapped.</p>|
|**Test Steps**|<p>1. Launch the CogniOpen application.</p><p>2. User taps the “Login in Here” button.</p><p>3. Users enter their biometric authentication information.</p><p>4. Navigate to the Record Audio screen.</p><p>5. Tap the “Start Audio Recording” button.</p><p>6. Say a few words to be recorded.</p><p>7. Tap the “Stop Audio Recording" button.</p><p>8. Tap the “Play Preview” button”</p><p>9. Ensure the accuracy of the audio by listening to it and verifying that it correctly captures what you were saying.</p><p>10. Tap the “Stop Preview” button.</p>|
|**Expected Result**|<p>- Tapping the “Start Preview” button plays the recording. </p><p>&emsp;- Tapping the "Stop Preview" button stops the recording.</p>|
|**Assumptions**|<p>- The CogniOpen application is properly installed and functioning on the test device.</p><p>- The device's operating system is compatible with the application.</p><p>- The user has successfully logged into the application and navigated to the Record Audio screen.</p>|
|**Actual Result**|The audio started playing when the play button was hit and stopped when the pause button was hit.|
|**Pass/Fail**|Pass|

<a name="_toc150003926"></a>Table 15: TC-8 Play/Pause Audio Recording

**
### <a name="_toc150003901"></a>**TC-9 Start New Recording from Audio Preview Screen**

|**Description**|To start a new recording, simply press the "New Recording" button, this will begin capturing new audio. |
| :- | :- |
|**Requirements**|<p>- The CogniOpen application must have a “New Recording” button on the Record Audio screen that initiates a new recording when tapped.</p><p>&emsp;</p>|
|**Test Steps**|<p>1. Launch the CogniOpen application.</p><p>2. User taps the “Login in Here” button.</p><p>3. Users enter their biometric authentication information.</p><p>4. Navigate to the Record Audio screen.</p><p>5. Tap the “Start Audio Recording” button.</p><p>6. Say a few words to be recorded.</p><p>7. Tap the “Stop Audio Recording" button.</p><p>8. Tap the “New Recording” button.</p><p></p>|
|**Expected Result**|<p>- Tapping the “New Recording” button starts a recording. </p><p>&emsp;&emsp;</p>|
|**Assumptions**|<p>- The CogniOpen application is properly installed and functioning on the test device.</p><p>- The device's operating system is compatible with the application.</p><p>- The user has successfully logged into the application and navigated to the Record Audio Preview screen.</p>|
|**Actual Result**|Clicking the New Recording button prompted for a new audio recording, and the recording began.|
|**Pass/Fail**|Pass|

<a name="_toc150003927"></a>Table 16: TC-9 Start New Audio Recording
**\

### <a name="_toc150003902"></a>**TC-10 Delete Recorded Audio from Audio Preview Screen**

|**Description**|To delete a recorded audio, press the “Trash Can" icon to remove the recording from the CogniOpen application.|
| :- | :- |
|**Requirements**|- The Record Audio screen must feature a " Trash Can" icon button that deletes the recorded audio when tapped.|
|**Test Steps**|<p>1. Launch the CogniOpen application.</p><p>2. User taps the “Login in Here” button.</p><p>3. Users enter their biometric authentication information.</p><p>4. Navigate to the Record Audio screen.</p><p>5. Tap the “Start Audio Recording” button.</p><p>6. Say a few words to be recorded.</p><p>7. Tap the “Stop Audio Recording" button.</p><p>8. Tap the “Trash Can” icon button.</p><p></p>|
|**Expected Result**|Tapping the “Trash Can” icon button deletes the saved recording. |
|**Assumptions**|<p>- The CogniOpen application is properly installed and functioning on the test device.</p><p>- The device's operating system is compatible with the application.</p><p>- The user has successfully logged into the application and navigated to the Record Audio Preview screen.</p>|
|**Actual Result**|After clicking the delete button, the recording was deleted.|
|**Pass/Fail**|Pass|

<a name="_toc150003928"></a>Table 17: TC-10 Delete Recorded Audio
**\

### <a name="_toc150003903"></a>**TC-11 View Profile Information**

|**Description**|A user can successfully view their profile information in the application.|
| :- | :- |
|**Requirements**|<p>- The profile screen displays the user's current information, including first name, last name, email address, and password</p><p>- The user shall be able to edit any of the displayed fields</p><p>- The user shall be able to save the edited information</p><p>- The user shall be able to cancel any changes made and revert to the previous information</p>|
|**Test Steps**|<p>1. Launch the CogniOpen application from the device.</p><p>2. User taps the “Login in Here” button.</p><p>3. Users enter their biometric authentication information.</p><p>4. Navigate to the profile screen from the home screen.</p><p>5. On the profile screen, locate and edit any of the provided fields.</p><p>6. Tap the "Cancel" button to exit the profile.</p>|
|**Expected Result**|- The user's profile information is displayed correctly on the profile screen.|
|**Assumptions**|<p>- The user is already registered with the application</p><p>- The user has previously entered profile information during registration</p><p>- The application is connected to the internet to retrieve user profile data</p><p>- The application has access to a backend database to store and retrieve user profile data</p><p>&emsp;</p>|
|**Actual Result**|The profile information was displayed.|
|**Pass/Fail**|Pass|

<a name="_toc150003929"></a>Table 18: TC-11 View Profile
**\

### <a name="_toc150003904"></a>**TC-12 Edit Profile Information** 

|**Description**|A user can successfully edit their profile information in the application.|
| :- | :- |
|**Requirements**|<p>- The profile screen displays the user's current information, including first name, last name, email address, and password</p><p>- The user shall be able to edit any of the displayed fields</p><p>- The user shall be able to save the edited information</p><p>- The user shall be able to cancel any changes made and revert to the previous information</p>|
|**Test Steps**|<p>1. Launch the CogniOpen application from the device.</p><p>2. User taps the “Login in Here” button.</p><p>3. Users enter their biometric authentication information.</p><p>4. Navigate to the profile screen from the home screen.</p><p>5. On the profile screen, locate and edit any of the provided fields.</p><p>6. Tap the "Save" button to save the changes made.</p><p>7. Verify that the edited information is saved by checking the displayed profile information.</p>|
|**Expected Result**|- The edited information is successfully saved, and the displayed profile information reflects the changes.|
|**Assumptions**|<p>- The user is already registered with the application</p><p>- The user has previously entered profile information during registration</p><p>- The application is connected to the internet to retrieve user profile data</p><p>- The application has access to a backend database to store and retrieve user profile data</p><p>&emsp;</p>|
|**Actual Result**|The edited information was displayed.|
|**Pass/Fail**|Pass|

<a name="_toc150003930"></a>Table 19: TC-12 Edit Profile
**\

### <a name="_toc150003905"></a>**TC-13 View Guided Tour**

|**Description**|The guided tour feature is designed to assist users in navigating the system and understanding its functionalities. The guided tour is accessible from the system's interface and provides a step-by-step tutorial on how to use the system's key features.|
| :- | :- |
|**Requirements**|<p>- The application shall display a guided tour to users when they tap the “Guided Tour” button on the CogniOpen application’s Home Screen.</p><p>- When the user taps the green arrow facing right, the application shall progress the user to the next guided tour screen.</p><p>- When the user taps the green arrow facing left, the application shall take the user back to the previous screen.</p>|
|**Test Steps**|<p>1. Launch the CogniOpen application from the device.</p><p>2. User taps the “Login in Here” button.</p><p>3. Users enter their biometric authentication information.</p><p>4. Navigate to the Guided Tour screen from the home screen.</p><p>5. User taps the “Green Arrow” facing to the right</p><p>6. User taps the “Green Arrow” facing left</p><p>7. Repeat the step 7 two times</p><p>8. Repeat step 8 one time</p><p>9. Repeat steps 7 until the tour is complete.</p>|
|**Expected Result**|<p>- The guided tour feature allows users to navigate through the tutorial easily. </p><p>&emsp;- When a user taps the green arrow to the right, they are automatically redirected to the next page of the tutorial.</p><p>&emsp;- When a user taps the green arrow to the left, they are redirected back to the previous screen.</p>|
|**Assumptions**|<p>- The user has previously registered with the application</p><p>- The user is connected to the internet</p><p>- The application is active and able to receive requests</p><p>- The application is able to communicate with the backend database services</p>|
|**Actual Result**|The guided tour was displayed and changed pictures after every swipe.|
|**Pass/Fail**|Pass|

<a name="_toc150003931"></a>Table 20: TC-13 View Guided Tour
**\

### <a name="_toc150003906"></a>**TC-14 Cancel Guided Tour**

|**Description**|A user can decide to cancel the guided tour, they can do so at any point during the tutorial by clicking on the cancel button provided on the screen.|
| :- | :- |
|**Requirements**|<p>- The application shall display a guided tour to users when they tap the “Guided Tour” button on the CogniOpen application’s Home Screen.</p><p>- When the user taps the green arrow facing right, the application shall progress the user to the next guided tour screen.</p><p>- When the user taps the green arrow facing left, the application shall take the user back to the previous screen.</p><p>- When the user taps the “X” button on the top right of the screen, the Guided Tour will exit and take the user back to the Home Screen.</p>|
|**Test Steps**|<p>1. Launch the CogniOpen application from the device.</p><p>2. User taps the “Login in Here” button.</p><p>3. Users enter their biometric authentication information.</p><p>4. Navigate to the Guided Tour screen from the home screen.</p><p>5. User taps the “Green Arrow” facing to the right</p><p>6. User taps the “X” button to cancel the tour.</p><p>7. The screen redirects to the home screen.</p>|
|**Expected Result**|<p>- When a user taps the “X” button, the Guided Tour is closed out and they are automatically redirected to the home screen.</p><p>&emsp;</p>|
|**Assumptions**|<p>- The user has previously registered with the application</p><p>- The user is connected to the internet</p><p>- The application is active and able to receive requests</p><p>- The application is able to communicate with the backend database services</p>|
|**Actual Result**|The back arrow was clicked, and the Home Screen was displayed.|
|**Pass/Fail**|Pass|

<a name="_toc150003932"></a>Table 21: TC-14 Cancel Guided Tour
**\

### <a name="_toc150003907"></a>**TC-15 Onboarding Voice Assistance**

|**Description**|During the onboarding process, the virtual assistant welcomes the user and provides an overview of the system. It then proceeds to guide the user through a series of steps to complete the necessary tasks. The virtual assistant will have a conversation with the user to help them understand the system functions.|
| :- | :- |
|**Requirements**|<p>- The onboarding should be able to guide users through the process of interacting with the virtual assistance and create a conversation summary.</p><p>- The virtual assistance onboarding should be able to adapt to the user's individual needs and preferences and provide them with a personalized onboarding experience.</p><p>- The AI onboarding should be easy to use and navigate, and should not require any prior knowledge of the application</p>|
|**Test Steps**|<p>1. Launch the CogniOpen application from the device</p><p>2. User taps the “Create Account” button</p><p>3. Users enters first name, last name, and email</p><p>4. Users tap the “Create Account” button.</p><p>5. The screen is redirected to the onboarding welcome screen.</p><p>6. The user performs each action virtual assistance is asking of you, then click the “Next” button.</p><p>7. After the onboarding, the user is redirected to the home screen</p><p>&emsp;</p>|
|**Expected Result**|- The user should be able to complete the onboarding process successfully and the system should redirect the user to the home screen.|
|**Assumptions**|<p>- The user must be a first-time registered user to login to the application. </p><p>- The user is connected to the internet</p><p>- The application is active and able to receive requests</p><p>- The application is able to communicate with the backend database services</p>|
|**Actual Result**|Onboarding screen prompts the user for inputs and takes it for attribution.|
|**Pass/Fail**|Pass|

<a name="_toc150003933"></a>Table 22: TC-15 Onboarding Assistant
**\

### <a name="_toc150003908"></a>**TC-16 Logout Application**

|**Description**|Verify that the logout functionality of the application works as expected and meets all specified requirements. The test case involves testing the logout button and verifying that the user's session is securely ended.|
| :- | :- |
|**Requirements**|<p>- Launch the CogniOpen application from the device.</p><p>- User taps the “Login in Here” button.</p><p>- Users enter their biometric authentication information.</p><p>- The logout button should be accessible to the user from the menu screen in the application.</p><p>- ` `Clicking on the logout button or option should immediately end the user's session and securely clear any unsaved data or input.</p><p>- The user should be returned to the login screen, or the application should be exited altogether.</p>|
|**Test Steps**|<p>1. Verify that the logout button or option is available and accessible to the user.</p><p>2. Click on the logout button or option and verify that the user's session is immediately ended.</p><p>3. Verify that any unsaved data or input is securely cleared from the device or server.</p><p>4. Verify that the user is returned to the login screen or that the application is exited altogether.</p><p></p>|
|**Expected Result**|<p>- The logout feature performs as intended, closing the user's session in a secure manner, erasing any unsaved information, and providing suitable feedback to the user. </p><p>&emsp;- The logout functionality is protected by appropriate security protocols to prevent unauthorized access.</p>|
|**Assumptions**|<p>- The user has previously registered with the application </p><p>- The user is connected to the internet </p><p>- The application is active and able to receive requests </p><p>- The application can communicate with the backend database services </p>|
|**Actual Result**|The logout button was clicked and the login screen is displayed.|
|**Pass/Fail**|Pass|

<a name="_toc150003934"></a>Table 23: TC-16 Application Logout
# <a name="_toc150003909"></a>**6. Test results** 
### <a name="_toc150003910"></a>**6.1 Functional Test Results**
`       `Functional tests were used to confirm and validate the internal logic and test the primary functionality of CogniOpen’s backend services. All tests were passed as of last run. The total includes 16 functional tests. These tests were all implemented using the Flutter test framework. 


|**Status**|**Total Count**|
| :-: | :-: |
|**Pass**|16|
|**Fail**|0|

<a name="_toc150003935"></a>Table 24: Test Metrics
# <a name="_toc150003911"></a>**7.  Summary**
`       `This test report provides a comprehensive overview of the testing activities for the CogniOpen Application. Due to the time restrictions and limited number of team members, the report outlines a focused approach to testing that aims to ensure the application meets the specified requirements and identify any unforeseen defects or limitations. However, the CogniOpen Application was successful and passed all the required testing with zero failings during all integration testing activities.

`       `However, there were a few defects found during the functional testing of the application. Review the table below for more information about the defects found.

|**Bug ID** |**Description**|**Severity**|
| :- | :- | :- |
|1 |If you don’t have a user profile, you can’t use the Virtual Assistant|Minor|
|2|<p>If the phone/emulator microphone is turned off (not disabled), transcription fails silently.</p><p></p>|Major|
|3|If the phone/emulator file permissions are turned off, no functionality works.|Major|

<a name="_toc150003936"></a>Table 25: Bug Report

`       `The report covers various testing activities, including functional, and UI testing of different features such as registering and logging in, accessing features through the home interface, interacting with the virtual assistant, recording audio, using the hamburger menu, managing the user profile, and viewing the guided tour. The testing phases include unit testing, functional testing, integration testing, regression testing, and user acceptance testing. The report also includes an RTM to ensure that the test cases cover all the requirements. The RTM lists the test case ID, test case title, requirement number, description, and results. Additionally, the report provides clear direction on the testing approach, including the testing environment, testing tools, test data, and test deliverables.

`       `Overall, the testing efforts for CogniOpen have been thorough and have identified both successes and areas for improvement. This report serves as a valuable reference for quality assurance, development, and project management teams

