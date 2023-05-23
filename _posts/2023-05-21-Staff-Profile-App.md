## Embracing Inclusivity: Power App for Employee Intros, Pronouns, and Name Pronunciation

### App Introduction
Even three years after switching to a hybrid work environment, we are still finding innovative ways to foster connections and promote a sense of belonging. 
After a successful implementation of a Coworker Compliment Power App, my organization's HR requested an app where employees could share more information about themselves. They wanted a place where our employees can build a sense of familiarity, even when working remotely or in different locations. 

I realized this task aligned with a separate request I had heard in my company’s Diversity and Equity Subcommittee: A way that staff, who feel comfortable to opt in, can share their pronouns, name phonetics, and a recording of how their name is pronounced.

To meet both of these requests, I built a user-friendly Power App to facilitate the sharing of employee introductions, pronouns, name phonetics, and even recordings of name pronunciations. This Staff Profile App empowers our team members to personalize their profiles and express their individuality within our collaborative workspace. With just a few clicks, colleagues can discover common interests, pronounce names correctly, and better connect with one another on a personal level.Recognizing and honoring individual identities is an essential aspect of fostering a welcoming and supportive work environment. 

---

### Solution Architecture

- Power Apps was used to create the Staff Profile Application. I used a Canvas App and started from scratch to allow the most customization.
- Sharepoint is used to store the data collected from the Profile app in Sharepoint Lists. Any name recordings or profile pictures taken in the app is stored in Sharepoint Document Libraries.
- Power Automate is used to take the name pronunciation recording from the app and transform it into a saveable file for Sharepoint. There is also an option to take a profile photo within the app. This feature also uses a Power Automate Flow to save the photo to a Sharepoint Document Library.

---

### Power App Structure
Text here
Text here
Text here

---

### Sharepoint List Structure
Text here
Text here
Text here

---

### Power Automate Flows
The trickiest part of this app was saving the Name Pronunciation recording into a file in the Sharepoint Library. Power Apps has a handy recording feature, but allowing the user to save their recording takes a bit of work.

A similar approach using a Power Automate flow was applied to allow the user to save a photo from Power App’s built in camera function in addition to the upload photo in the Form.


```
