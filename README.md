# Digital Forensics Computer Drive Image Analysis

## Objective

To analyze the forensic image of a suspect’s laptop to uncover digital evidence of preparation for a violent act, including deleted files, communications, cloud storage activity, and internet searches. The goal is to reconstruct the suspect’s planning and intentions through detailed forensic analysis.

### Skills Learned


- Recovered deleted files and extracted evidence using Autopsy and OSForensics  
- Analyzed file systems to reconstruct user activity  
- Examined metadata and user artifacts to link evidence to the suspect  
- Investigated cloud storage sync data to identify stored and shared files  
- Correlated documents, images, and communications to build a full case narrative  
- Applied Windows file system knowledge to track user behavior  
- Created clear forensic reports to communicate findings effectively

  
### Tools Used

<div> <img src="https://img.shields.io/badge/-Autopsy-8B4513?&style=for-the-badge&logo=Blackberry&logoColor=white" /> <img src="https://img.shields.io/badge/-OSForensics-2ECC71?&style=for-the-badge&logo=Microsoft&logoColor=white" /> <img src="https://img.shields.io/badge/-The_Sleuth_Kit-000000?&style=for-the-badge&logo=Blackberry&logoColor=white" /> </div>

-Autopsy: A powerful digital forensics platform used to analyze disk images, recover deleted files, and examine metadata for evidence.

-OSForensics: A good forensic suite for file recovery, keyword searches, and timeline analysis on disk images.

## Overview
The Lone Wolf scenario is set from the fictional seizure of a laptop of a fictional individual who was planning a mass shooting. In this scenario, the individual’s brother alerted the police regarding the increasingly concerning behavior of his brother. As a result of the alert, the police seized the brother’s laptop. The laptop was then imaged.
## Scenario
Jim Cloudy is a resident of Alexandria, VA. He is unhappy with the media’s 
coverage of gun violence and what he perceived as an attack on the 2nd Amendment. 
Prior to the start of the scenario, Jim gets into a heated online argument with his 
brother, Paul Cloudy. During this argument, Jim destroys his laptop by throwing it on the 
floor. Jim disposes of this laptop using his Apartment’s trash chute, which is collected 
daily. Paul gives Jim one of his old laptops with the promise that he wouldn’t break it. 
Paul wiped the laptop’s drive prior to giving it to Jim. Jim does not encrypt any data and 
takes no overt steps to obfuscate data.

Jim is currently unemployed and has trouble sleeping, so he sometimes spends 
odd hours on the computer. While officially unemployed, the scenario briefly alludes to 
his marihuana growing activities, and an amassed savings of $325,000. Jim becomes 
increasingly irate concerning the growing support for “gun-control”. Jim starts writing 
about his personal views and begins planning a “Lone Wolf” style attack. Jim wants to 
ensure his views are saved for posterity and his documents and plans can be accessed 
from anywhere; therefore, he uploads documents to a variety of cloud storage services. 
Prior to the planned date of the attack Jim gives Paul access to his cloud storage 
accounts. Paul is suspicious based on Jim’s sudden decision to go on vacation and not 
come back. When Paul reads some of the documents he notifies police and a Search 
Warrant of Jim’s apartment is executed and he is apprehended while talking to Paul 
online.

Jim’s plan was attack a town hall meeting scheduled from 12:30 PM until 2:00PM 
on April 7th, 2018, at the Cascades Library, 21030 Whitfield Pl, Sterling, VA, 20165. The 
a meeting was held to discuss solutions for gun violence and was attended by two U.S. 
Senators. Meeting Room B has a seating capacity of 130 people. After the attack, Jim 
planned to fly from Dulles International Airport to Bali Indonesia, where there is no 
current extradition treaty. Sometime after his arrival, he planned to release a “press 
statement” explaining his actions. Jim had no intention of ever returning to the U.S. and 
calculated he could live comfortably in Bali for nine years on savings alone.
Find evidence that supports all the scenario description parts to show Jim was guilty in his plans.
Create a forensic report that contains:
• Relevant documents (Word, PowerPoint, pictures, etc ).
• Cloud storage services are being used to store and synchronize documents in the cloud.
• Internet searches.
• Chats.
## Questions

### 1. Using Autopsy, identify the five files that the user jcloudy has deleted. Include the file path, name of the file, and time and date deleted. Do the timestamps match between applications? If not, why would this be?

![image](https://github.com/user-attachments/assets/592264b0-f4ae-412d-b86d-c6640cd2a804)

![image](https://github.com/user-attachments/assets/602cbd55-b13d-4b8a-ada0-6657e7df88fc)

Their timestamps match between Autopsy and OSForensics.
4 of the files ($RK7BOIS.html, R23A30B, $RCHAQB.html, $RQAU6NQ) are actually two files with their corresponding files that point to their previous location. Both websites were visited, but they were deleted on  2018-04-04 at 22:02:17 EDT. One file ($RYRY5PT.jpg) is a picture of the place where the attack is planned to occur. This one was deleted two days later  (2018-04-06 at 04:29:21 EDT). These files were deleted on different days. If they did not match this could be because of timezone differences, different timestamps interpretations, or tool-specific parsing differences.

### 2. What are the two email addresses for JCloudy?

![image](https://github.com/user-attachments/assets/c78875fc-a670-4b9a-b0d6-0cafb3f34332)

![image](https://github.com/user-attachments/assets/c7653486-f296-482c-98dd-5dd775f4bca3)

![image](https://github.com/user-attachments/assets/b1c908ec-9c5f-4309-858c-b67c3c74f13e)

![image](https://github.com/user-attachments/assets/331db9e0-2597-4df5-906c-af55e6c6e6a7)

a) jimcloudy@outlook.com

b) jimcloudy1@gmail.com


### 3. What are the email accounts used to log into the following?

a) Microsoft Account jimcloudy@outlook.com

![image](https://github.com/user-attachments/assets/9574e32b-7310-4723-a8b2-df6991d84f02)

b) Google Account jimcloudy1@gmail.com

![image](https://github.com/user-attachments/assets/d3bc0f46-18fe-479b-ba38-9802776d7516)

c) Dropbox Account jimcloudy1@gmail.com

![image](https://github.com/user-attachments/assets/425c2374-2d22-4984-940a-8e21b22e3122)

d) Box Account jimcloudy1@gmail.com

![image](https://github.com/user-attachments/assets/d28809a9-3d5d-4820-a3e2-80678574c9ef)

e) Amazon Web Services Account: jimcloudy1@gmail.com

![image](https://github.com/user-attachments/assets/0b7c2d1c-d53f-42c5-a58e-5c17bab11506)

f) Facebook jimcloudy1@gmail.com

![image](https://github.com/user-attachments/assets/d78c5651-7c35-4ac6-8776-13382003eead)

g) Twitter jimcloudy1@gmail.com

![image](https://github.com/user-attachments/assets/ff294761-5c0d-460a-8788-56b4de55c0e2)


### 4. What type(s) of weapons are being considered?

![image](https://github.com/user-attachments/assets/47e1c3f5-6075-4882-947c-9bd5282bbe31)

The user JCloudy has done research and visited websites to shop for rifles such as the Ruger 10-22, Keltec sub 200, and the FN P90.

![image](https://github.com/user-attachments/assets/b0ce63df-65a2-42c7-9a1a-a074912f1ff5)

![image](https://github.com/user-attachments/assets/2effacdc-759a-4191-b7df-e99ca58dd366)

According to his Planning Document, he will likely chose the Kel-Tec Sub 2000.

### 5. Was there any evidence of video games played?  If so, show the titles.

a) Burnout Paradise

![image](https://github.com/user-attachments/assets/48b9989d-bdd1-426f-9566-62d3c3ab412d)

b) Devil May Cry 4

![image](https://github.com/user-attachments/assets/d195cc58-e905-48e1-9522-22e4ecc70b05)

c) Guitar Hero 3

![image](https://github.com/user-attachments/assets/91b3ce04-5b23-4513-b85e-b13f74d5c202)

d) Tomb Raider Underworld 2

![image](https://github.com/user-attachments/assets/83789b62-ee51-45df-b499-62ef66b39798)
These pictures are under the Extension mismatch category. This is because these are JPEGs marked as JPS, which is a format used to create a 3D effect out of a 2D picture. Such files usually contain two images with different perspectives appropriate for each eye. These pictures are commonly generated and marked with such an extension when a particular graphic software (like a videogame) takes a screenshot and saves it, which means that the games shown must have been installed on the user's computer for them to be created as JPS.

### 6. What country is being considered to flee to?   Explain your reasoning behind this choice.

![image](https://github.com/user-attachments/assets/101db2d0-400b-4e6e-bb49-e43930cf8a24)

![image](https://github.com/user-attachments/assets/2aad6e49-cda1-484b-95c7-1a5d124807e4)

He is considering Vietnam and Indonesia since there are no extradition policies. You can tell that by his planning docs and his web searches.

### 7. What travel plans can you find?  Any proposed layovers?

![image](https://github.com/user-attachments/assets/63334635-0663-4e05-827c-e8726042ff68)

![image](https://github.com/user-attachments/assets/87c6f056-4356-446f-90a6-9e0962c9f18c)

He is considering going through Dulles International Airport with a layover in Qatar, and another option is through Seoul as a layover. He also keeps Vietnam as an option, since he is looking at countries where his savings will last long, as these are cheaper to live in.

### 8. Identify two URLs from the internet searches and provide the IP owner, and reputation scores or blacklist scores from two different resources.


a) https://www.gunbroker.com/#home-footer (172.64.152.34)

![image](https://github.com/user-attachments/assets/38aba712-7d79-43db-be59-7c9dd512663e)

![image](https://github.com/user-attachments/assets/7aa94c8d-04a2-4448-8f8c-89b0e4b36a05)

![image](https://github.com/user-attachments/assets/0f56e327-b1b0-44f4-acdf-d55100fd5b32)

![image](https://github.com/user-attachments/assets/832ed5c3-c32e-45d7-8298-44f42af3e127)


 b) https://lonelyplanet.com/indonesia/money-costs (18.165.140.64)

 ![image](https://github.com/user-attachments/assets/c5fb489b-7ea1-4c94-8d52-a9cbd805e4ba)

 ![image](https://github.com/user-attachments/assets/7c2f323f-59f0-48ce-99e0-a0f24da7c551)

 ![image](https://github.com/user-attachments/assets/808f3d73-ecec-4577-808c-9afbb28eadf3)

 ![image](https://github.com/user-attachments/assets/a81ac69b-c611-4f84-8849-b969420cac6d)

 
### 9. The examination disclosed evidence to show the user conducted multiple internet searches pertaining to the procurement of weapons and ammunition, locations to attack, and evading capture and extradition. Explain at least five NEW items of supporting evidence for these actions and illustrate the facts of the evidence. 

Cloudy’s Desktop Files: 

![image](https://github.com/user-attachments/assets/fcb14920-0ac0-4a8e-8488-0fa9b0fdc8c6)

On his desktop, he left a doc file called “The Cloudy Manifesto”, where he references his plans, his reasons, and hints about what he is going to do.

![image](https://github.com/user-attachments/assets/c5d70986-45ed-4d91-abe4-3de4af682722)

We can also see another doc file with airport information, which indicates he has been researching flights to Indonesia to take through Ronald Reagan Airport, concerned about the flight being on time. Also, we can see he has already calculated the distance it will take him to get there from the place where the meeting is being held.

![image](https://github.com/user-attachments/assets/cadcc0b4-1c61-47c3-88cd-54a748bff394)

![image](https://github.com/user-attachments/assets/9031fc83-fafe-48eb-8b98-065130807465)

![image](https://github.com/user-attachments/assets/cc2fa26b-4be1-43f5-9843-24a4ee80fd04)

![image](https://github.com/user-attachments/assets/f23bffb3-e70b-4f23-a08e-5a435caefac0)

![image](https://github.com/user-attachments/assets/c2e2f35c-ca3a-4467-9cc2-73905413453b)

![image](https://github.com/user-attachments/assets/39eca1dc-4fcc-43a9-bf95-5210ccbc9751)

![image](https://github.com/user-attachments/assets/ac84cc73-9960-4618-8686-318687baac34)



In a PPTX file found on his computer desktop directory, the slides contain information about the operation, including addresses, dates, pictures of the target location, escape route, hotel options, etc.

![image](https://github.com/user-attachments/assets/19bfb47e-c01d-4358-9174-44d979dc5ea8)

A more detailed description of his plans can be seen in a doc file on his desktop.

![image](https://github.com/user-attachments/assets/bef6766a-ed1a-4f9d-a69b-4fe215f9a7b9)

![image](https://github.com/user-attachments/assets/f189ce01-67a9-4bad-b15a-378f73773d19)

![image](https://github.com/user-attachments/assets/e1ee7693-7f7f-4336-baf4-7d060c0c57ce)

We can find those same files backed up in Google Drive, OneDrive, BoxSync, and AWS.

![image](https://github.com/user-attachments/assets/5c26bf66-cc6c-44d2-adde-220348019bc2)

Deleted searches on near shooting ranges to practice for the attack.

![image](https://github.com/user-attachments/assets/b354018e-2424-47de-9090-7135bb329041)

The user jcloudy also shopped for guns and places to get them from.

## Conclusion

### The forensic analysis of Jim Cloudy’s laptop shows clear evidence of a planned mass attack. The findings are:

- Planning Documents

- The Cloudy Manifesto outlined motives and intent.

- PowerPoint and Word files detailed the attack location, timing, escape routes, and hotel options.

- Travel Preparation

- Documents showed research into flights to Indonesia and calculated travel time from the attack site.

- Cloud Storage Evidence

- Identical files were found in Google Drive, OneDrive, and BoxSync under the “JCloudy” user profile.

### User Attribution

All files were created and accessed by the “JCloudy” account, linking Jim directly to the plans.


This evidence confirms premeditation, preparation, and intent, validating that Jim Cloudy was responsible for orchestrating the attempted attack.

