# Code Review Analysis

This [code review](https://www.youtube.com/watch?v=IWou8g_Eeg4) analyzes and proposes the enhancements of three original artifacts for the Software Design/Engineering, Algorithms and Data Structures, and Databases categories. The code review presented is an individual code review, where I am the sole reviewer of the artifact files. Being the sole reviewer, I can analyze my faults and create plans for the issues in the artifacts. I can use this code review to accept my mistakes and fail fast, which allows me to adapt to the industry. I intend to collaborate with team members on code reviews and incorporate their suggestions in the future. 

## Software Design/Engineering Category 
The Software Design/Engineering category originates from the artifacts within the course CS 410: Software Reverse Engineering. The psuedocode presented will improve the artifact, and will be altered in the final enhancement one code. 
### Psuedocode
```
START <stdio.h>


START int main(){

PRINT printf(“This C file was created by Clara Kellermann-Bryant”);

DEFINE int information, int customerchoice, int permissions, int i;

IF ( i = 1; i & gt 9; i) THEN

INITIALIZE int information = int customerchoice + int permissions;


PRINT printf( int customerchoice “+” int permissions “=” int information); 

}


START int ChangeCustomerChoice(){

DEFINE int customerchoice, int k;

IF (k = 1; k & gt 9; k) THEN

INITIALIZE int customerchoice = int k + 1;

PRINT printf(“Change customer choice”);


DEFINE int customerchoice2, int e;

IF (e = 1; e & gt 9; e) THEN

INITIALIZE int customerchoice2 = int e + 1;

PRINT printf(“Customer choice stays the same”);
}



START int CheckUserPermissionAccess() {


DEFINE int permissions, int g;

IF (g = 1; g & gt 9; g) THEN

INITIALIZE int permissions = int g + 1;

PRINT printf(“Permission is granted”);


DEFINE int permissions2, int h;

IF (h = 1; h & gt 9; h) THEN

INITIALIZE int permissions2 = int h + 1;

PRINT printf(“Permission denied”);

}



START int DisplayInfo () {


DEFINE int information, int information2, int customerchoice, int customerchoice2, int permissions, int permissions2;

INITIALIZE int information = int customerchoice + int permissions

INITIALIZE int information2 = int customerchoice2 + int permissions2


PRINT printf(customerchoice “+” permissions “=” information);

PRINT printf(customerchoice2 “+” permissions2 “=” information);

}



```


## Algorithms and Data Structures Category
The Algorithms and Data Structures category originates from the artifacts within the course CS 405: Secure Coding. The psuedocode presented will improve the artifact, and will be altered in the final enhancement two code. 
### Psuedocode
```
Data structure 
INITIALIZE std:: unique_ptr2<std::vector<int>> unique_collection;

START TEST_F (CanAddToEmptyStructureUniqueCollection) {

ASSERT_EQ (unique_collection->size(), 20);


}


Algorithm


START TEST_F (CapacityGreaterThanOrEqualToUniqueCollectionEntries) {

DEFINE add_uentries(0);

DEFINE add_uentries(2);

DEFINE add_uentries(100);

DEFINE add_uentries(1000);

ASSERT_GE (unique_collection.get(), 0);

ASSERT_GE (unique_collection.get(), 2);

ASSERT_GE (unique_collection.get(), 100);

ASSERT_GE (unique_collection.get(), 1000); 

}



Refine CanAddToEmptyVector


START TEST_F (CollectionTest, CanAddToEmptyVector) {


DEFINE add_entries(1);

EXPECT_EQ (collection -> empty, 0);

ASSERT_EQ (collection-> size, 1);

}




Negative Test



START TEST_F (UniqueCollectionTest, ExceptionUniqueCollSizeOutOfBounds) {

INITIALIZE int unique_collect = 1250;


DEFINE unique_collect;


TRY {

FAIL() << Unique Collection Size Out Of Bound Symbolic;

}

CATCH (const std::exception& e)

{
EXPECT_EQ (unique_collection->size, 250);

THROW;

}

CATCH (const std::exception& get())

{

EXPECT_EQ (unique_collection->size, 1000);


FAIL() << Unique Collection Size Out Of Bounds Symbolic;

}


```


## Databases Category
The Databases category originates from the artifacts within the course DAD 220: Introduction to SQL. The psuedocode presented will improve the artifact, and will be altered in the final enhancement three code.
### Psuedocode

```
START mysql;

CREATE DATABASE arkhamboardgameDB

CREATE TABLE arkham_enemies (

INITIALIZE EnemyID int, 

INITIALIZE EnemyName varchar(255),

INITIALIZE EnemyExpansion varchar(255),

INITIALIZE EnemyAttributes varchar(255)

);


CREATE TABLE arkham_consumables (

INITIALIZE ConsumableID int NOT NULL UNIQUE,

INITIALIZE CardType varchar(255) NOT NULL,

INITIALIZE CardName varchar(255),



);



CREATE TABLE arkham_investigators (

INITIALIZE InvestigatorID int NOT NULL UNIQUE,

INITIALIZE InvestigatorType varchar(255) NOT NULL,

INITIALIZE InvestigatorName varchar(255),

INITIALIZE InvestigatorItems varchar(255) NOT NULL,

INITIALIZE InvestigatorHealth varchar(255),

INITIALIZE InvestigatorSanity varchar(255),

INITIALIZE InvestigatorAge int, 

INITIALIZE CHECK (InvestigatorAge<= 100)

);

Join tables

SELECT arkham_investigators.InvestigatorItems, arkham_consumables.CardType

DECLARE FROM arkham_investigators
INITIALIZE INNER JOIN arkham_consumables ON arkham_investigators.InvestigatorType=arkham_consumables.InvestigatorType





SQL Injection Prevention:


INITIALIZE SELECT * FROM Users WHERE Name=” “ or “value” = “value” AND Password=” “ or “value” = “value”;




check low on health and sanity

INITIALIZE SELECT InvestigatorID, InvestigatorHealth, IF(InvestigatorHealth>9, “Healthy”, “Injured”)

INITIALIZE FROM arkham_investigators;


INITIALIZE SELECT InvestigatorID, InvestigatorSanity, IF(InvestigatorSanity>7, “Sane”, “Insane”)

INITIALIZE FROM arkham_investigators;


```

# Code Review Video

You can find a full-screen version of the code review here on [Youtube](https://www.youtube.com/watch?v=IWou8g_Eeg4)

![Image](https://www.youtube.com/watch?v=IWou8g_Eeg4)


![Image](https://www.kindpng.com/picc/m/47-470845_non-copyright-youtube-logo-copyright-free-youtube-logo.png)



@KindPNG,
no copyright infringement is intended. 


