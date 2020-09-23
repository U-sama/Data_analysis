# (Titanic Dataset)

## by (Osama Mohamed Saad Elahwel)




## Dataset

>
This is the titanic dataset from kaggle 

link : https://www.kaggle.com/c/titanic/overview

this data include 12 column and 891 record

columns are

-survival	Survival	0 = No, 1 = Yes

-p-class	Ticket class	1 = 1st, 2 = 2nd, 3 = 3rd

-sex	Sex	

-Age	Age in years	

-sibsp	# of siblings / spouses aboard the Titanic	

-parch	# of parents / children aboard the Titanic	

-ticket	Ticket number	

-fare	Passenger fare	

-cabin	Cabin number	

-embarked	Port of Embarkation

I added some new columns into the data to better clarifies relationships between columns and the columns it self

-alive	indicate wether or not the passenger were alive (yes,no) instead of (1,0)

-alone	indicate wether or not passenger had combanions

-who	split passengers to male,famale,child(under 15 years old)

-class	that indicates the passenger class (First,Second,Third) instead of (1,2,3)

-embark_town	shows name of the embarked town insted of S,C,Q in embarked column

I filled the missing values in age column by the average age fo the passengers with the same title in their names 

as they are more likely to be in the same age.

I also droped some 3 records that are outliers in the fare column and 2 missing values in embarked column with tot 5 records are droped.

I deopped some un nessesary columns that  i replaced them with another column or i didnt use in the analysis and visualization these columns are

[PassengerId, Ticket, Cabin , Pclass, Parch, SibSp]

So the remining columns are

[survived, name, sex, age, fare, embarked, embark_town, alive, alone, class, who]



## Summary of Findings



>First i wanted to see whe passengers alive to dead so i made a barplot for alive column then i wanted to see the Sex column

and men are more likely to appear in the data, then i wanted to see the class column as i thought it has a big effect on the death chances

and as expected it has as thee Third class had more passengers than other classes as its the chepeast one, passengers age 

had a high increase started from 18 years old with a large apike in the 30-33 range, with some children under 12 years old,

there were three towns and the most town with passengers was Southampton.

Bivariate exploration, I first  checked the class to alive columns and as expected passengers are more likely to die if they were in the Third class

unlike the first class whis had more survirals than died ones, then i tested the who variable with alive and as i thought men are more likely to die

than women,and for alone and alive o found that alone passengers had more chances to die also.

Multivariate exploration, i found that most of the men whom died where in the third class and most of the women whom survived where in the first

and second classes, also i found that you are more likely to live if you are younger in age which dosent depend on the class 

as if you are in the first class but old in age then u are more likely to die than younger one.



Passengers whom died are more than whom were alive after the crash, women are more likely to live than men,

Passengers in the third class are more likely to die than first and second class, most of the female passengers are in the second and first class

that may be why they had more chances to live, you re more likely to live of you are younger in age even if u are in the first class.

Main Factors that make passenger die(Man,Alone,old,Third class) the deadly features.

In my opinion

-Alone old man in the third class was 100% died

