## Embracing Inclusivity: Power App for Employee Intros, Pronouns, and Name Pronunciation

### App Introduction
Even three years after switching to a hybrid work environment, we are still finding innovative ways to foster connections and promote a sense of belonging. 
After a successful implementation of a Coworker Compliment Power App, my organization's HR requested an app where employees could share more information about themselves. They wanted a place where our employees can build a sense of familiarity, even when working remotely or in different locations. 

I realized this task aligned with a separate request I had heard in my company’s Diversity and Equity Subcommittee: A way that staff, who feel comfortable to opt in, can share their pronouns, name phonetics, and a recording of how their name is pronounced.

To meet both of these requests, I built a user-friendly Power App to facilitate the sharing of employee introductions, pronouns, name phonetics, and even recordings of name pronunciations. This Staff Profile App empowers our team members to personalize their profiles and express their individuality within our collaborative workspace. With just a few clicks, colleagues can discover common interests, pronounce names correctly, and better connect with one another on a personal level. Recognizing and honoring individual identities is an essential aspect of fostering a welcoming and supportive work environment. 

<br>

![Home Page of Staff Profile App](https://github.com/KarissaLowe/KarissaLowe.github.io/blob/main/Images/Home1.png?raw=true)

---

### Solution Architecture

- Power Apps was used to create the Staff Profile Application. I used a Canvas App and started from scratch to allow the most customization.
- Sharepoint is used to store the data collected from the Profile app in Sharepoint Lists. Any name recordings or profile pictures taken in the app is stored in Sharepoint Document Libraries.
- Power Automate is used to take the name pronunciation recording from the app and transform it into a saveable file for Sharepoint. There is also an option to take a profile photo within the app. This feature also uses a Power Automate Flow to save the photo to a Sharepoint Document Library.

<br>

![Staff Profile Solution Architecture](https://github.com/KarissaLowe/KarissaLowe.github.io/blob/main/Images/Microsoft%20Power%20Apps.png?raw=true)


---

### Power App Structure
The Power App has two main pages in addition to the Home Page:

Edit your Profile: 
This page allows employees to fill out their profile. Information is collected and stored through a Form control connected to a Sharepoint List. Some example questions are: Preferred Name? Pronouns? What days do you come into the office? No fields are required, so the user can fill out as little or as much as they would like.
The Microphone control and Audio control are also used to allow the employee to record their name and play back the recording. A Power Automate flow is used to save the file from the Microphone control into the Sharepoint Document library.
 
![Edit Page of Staff Profile](https://github.com/KarissaLowe/KarissaLowe.github.io/blob/main/Images/Edit1.png?raw=true)

View Profiles: 
This page uses Power App’s Gallery and Form Display function to show the information employees provide. The gallery of names is searchable by department or employee name using the search function. To view a profile, you can click on the name of the employee.

![View page](https://github.com/KarissaLowe/KarissaLowe.github.io/blob/main/Images/View1.png?raw=true)

In addition to these main two pages, I added a link to my company’s organization chart and a page to collect user feedback. There is also a Settings page only accessible by HR to allow removal of profiles if inappropriate content is added.

---

### Power Automate Flows
The trickiest part of this app was saving the Name Pronunciation recording into Sharepoint. Power Apps has a handy recording feature, but allowing the user to save their recording takes a bit of work.

We need to first convert the recording to a binary format and send it to Power Automate when the profile is submitted. The Power Automate flow will then convert and save this recording to the Sharepoint Document Library that backs the app. To accomplish this, I followed this amazing guide written by [Rajkiran Swain](https://www.enjoysharepoint.com/saving-microphone-audio-recorded-in-powerapps-to-sharepoint-online/).

And that’s it! I hope this can help you innovatively use Power Apps to create a supportive work environment for all.
```
