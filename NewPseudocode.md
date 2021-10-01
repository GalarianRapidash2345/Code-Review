# REFINEMENT PLAN PSEUDOCODE


## Artifact 1: CS 410 Project One for software engineering and design



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





## Artifact 2: CS 405 Milestone Two for data structures and algorithms



Data structure 


START TEST_F (CanAddToEmptyStructureUniqueCollection) {

INITIALIZE std:: unique_ptr2<std::vector<int>> unique_collection;

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

FAIL() << “Unique Collection Size Out Of Bounds”;

}

CATCH (const std::exception& e)

{
EXPECT_EQ (unique_collection->size, 250);

THROW;

}

CATCH (const std::exception& get())

{

EXPECT_EQ (unique_collection->size, 1000);


FAIL() << “Unique Collection Size Out Of Bounds”;

}















## Artifact 3: DAD 220 Report for Databases




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


