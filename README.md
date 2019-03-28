# eBioDigitDB


## INSTRUCTIONS FOR DOWNLOADING e-BioDigit DB 
1) [Download license agreement](http://atvs.ii.uam.es/atvs/licenses/e-BioDigit_License.pdf), send by email one signed and scanned copy to **atvs@uam.es** according to the instructions given in point 2.
 
 
2) Send an email to **atvs@uam.es**, as follows:

   *Subject:* **[DATABASE download: e-BioDigit DB ]**

   Body: Your name, e-mail, telephone number, organization, postal mail, purpose for which you will use the database, time and date at which you sent the email with the signed license agreement.
 

3) Once the email copy of the license agreement has been received at ATVS, you will receive an email with a username, a password, and a time slot to download the database.
 

4) [Download the database](http://atvs.ii.uam.es/atvs/intranet/free_DB/e-BioDigit), for which you will need to provide the authentication information given in step 4. After you finish the download, please notify by email to **atvs@uam.es** that you have successfully completed the transaction.
 

5) For more information, please contact: **atvs@uam.es**

## DESCRIPTION OF e-BioDigit DB

The e-BioDigit database comprises **on-line handwritten numerical digits from 0 to 9** acquired using a Samsung Galaxy Note 10.1 general purpose tablet for a total of 93 users. All samples were acquired **using the finger touch as input** so only information related to X and Y spatial coordinates are considered. Regarding the acquisition protocol, data subjects had to perform handwritten numerical digits from 0 to 9 one at a time. Some examples of the handwritten numerical digits acquired for the e-BioDigit database are depicted in Figure 1. Additionally, **samples were collected in two sessions with a time gap of at least three weeks between them** in order to consider inter-session variability, very important for behavioural biometric traits. For each session, users had to perform a total of 4 numerical sequences from 0 to 9. Therefore, **there are a total of 8 samples per numerical digit and user**. The software for capturing handwritten numerical digits was developed in order to minimize the variability of the user during the acquisition process. **A rectangular area with a writing surface size similar to a 5-inch screen smartphone was considered**. A horizontal line was represented in the bottom part of the rectangular area, including two buttons OK and Cancel to press after writing if the sample was good or bad respectively. If the sample was not good, then it was repeated.

![](http://atvs.ii.uam.es/atvs/digito_0.png )

![](http://atvs.ii.uam.es/atvs/digito_2.png )

Figure 1. Examples of different handwritten numerical digits of the e-BioDigit database. X and Y denote horizontal and vertical position versus the time samples. [CVPR2018_OTP].


#### FILES FORMAT
The handwritten numerical digits are stored in text files, where:

+ ROW 1: it just contains one entry with the number of sampled points of the numerical digit (N).

+ ROWS 2 to (N+1): 

  + COLUMN 1: represents the x coordinate.

  + COLUMN 2: represents the y coordinate.

  + COLUMN 3: this is a synthetic timestamp.

  + COLUMN 4: represents the pressure (p) function. All values are set to 255 as this information is not available when using the finger touch.

#### FILES NOMENCLATURE
The nomenclature followed to name the numerical digit files is as follows: uAAA_digit_B_CCC.txt

+ AAA: indicates the number of the user [101, 102, ... , 208]. Some users in between were finally removed having in total 93 users.

+ B: indicates the numerical digit [0, 1, ... , 9].

+ CCC: indicates the number of the acquisition sample [002, 004, ... , 016]. There are a total of 8 samples per numerical digit and user.

Finally, handwritten numerical digits are organized into "session_1" and "session_2" folders.

#### REFERENCES
For further information on the database and on different applications where it has been used, we refer the reader to (all these articles are publicly available in the  [publications](http://atvs.ii.uam.es/atvs/listpublications.do) section of the BiDA group webpage.) 
+ [CVPR2018_OTP] R. Tolosana, R. Vera-Rodriguez, J. Fierrez and J. Ortega-Garcia, "Incorporating Touch Biometrics to Mobile One-Time Passwords: Exploration of Digits.", in Proc. IEEE Conf. on Computer Vision and Pattern Recognition Workshops, CVPRW, Salt Lake City, USA, 2018..

Please remember to reference articles [CVPR2018_OTP] on any work made public, whatever the form, based directly or indirectly on any part of the e-BioDigit Database.
