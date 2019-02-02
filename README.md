# CareerCloudBusinessLogic_Part3

@Author: Medhanie Weldemariam @Date: December 06, 2018 @Place: Toronto, ON

In module, I created the business logic layer.  
This layer defines business specific rules that the application will have to maintain.  
The rules will dictate the parameters of allowed data to be saved in the system.  These rules are listed in the Rules section below.

Rules:
Class	Property	Rule	Code
1.	ApplicantEducationLogic	Major	Cannot be empty or less than 3 characters	107
2.	ApplicantEducationLogic	StartDate	Cannot be greater than today	108
3.	ApplicantEducationLogic	CompletionDate	CompletionDate cannot be earlier than StartDate	109
4.	ApplicantJobApplicationLogic	ApplicationDate	ApplicationDate cannot be greater than today	110
5.	ApplicantProfileLogic		CurrentSalary	CurrentSalary cannot be negative	111
6.	ApplicantProfileLogic		CurrentRate	CurrentRate cannot be negative	112
7.	ApplicantResumeLogic	Resume	Resume cannot be empty	113
8.	ApplicantSkillLogic	StartMonth	Cannot be greater than 12	101
9.	ApplicantSkillLogic	EndMonth	Cannot be greater than 12	102
10.	ApplicantSkillLogic	StartYear	Cannot be less then 1900	103
11.	ApplicantSkillLogic	EndYear	Cannot be less then StartYear	104
12.	ApplicantWorkHistoryLogic	CompanyName	Must be greater then 2 characters	105
13.	CompanyDescriptionLogic	CompanyDescription	CompanyDescription must be greater than 2 characters	107
14.	CompanyDescriptionLogic	CompanyName	CompanyName must be greater than 2 characters	106
15.	CompanyJobDescriptionLogic	JobName	JobName cannot be empty	300
16.	CompanyJobDescriptionLogic	JobDescriptions	JobDescriptions cannot be empty	301
17.	CompanyJobEducationLogic	Major	Major must be at least 2 characters	200
18.	CompanyJobEducationLogic	Importance	Importance cannot be less than 0 	201
19.	CompanyJobDescriptionLogic	JobName	JobName cannot be null	300
20.	CompanyJobDescriptionLogic	JobDescriptions	JobDescriptions cannot be null	301
21.	CompanyJobSkillLogic	Importance	Importance cannot be less than 0	400
22.	CompanyLocationLogic	CountryCode	CountryCode cannot be empty	500
23.	CompanyLocationLogic	Province	Province cannot be empty	501
24.	CompanyLocationLogic	Street	Street cannot be empty	502
25.	CompanyLocationLogic	City	City cannot be empty	503
26.	CompanyLocationLogic	PostalCode	PostalCode cannot be empty	504
27.	CompanyProfileLogic	CompanyWebsite	Valid websites must end with the following extensions – ".ca", ".com", ".biz"	600
28.	CompanyProfileLogic	ContactPhone	Must correspond to a valid phone number (e.g. 416-555-1234)	601
29.	SecurityLoginLogic	Password	Length must be 10 or greater 	700
30.	SecurityLoginLogic	Password	Must contain one of the following characters ("$", "*", "#", "_", "@")	701
31.	SecurityLoginLogic	PhoneNumber	Cannot be blank	702
32.	SecurityLoginLogic	PhoneNumber	Must conform to a phone number pattern (e.g. 416-555-1234)	703
33.	SecurityLoginLogic	EmailAddress	Cannot be empty and must match a valid email address pattern (e.g. someone@shomewhere.com)	704
34.	SecurityLoginLogic	FullName	Cannot be empty	705
35.	SecurityRoleLogic	Role	Cannot be empty	800
36.	SystemCountryCodeLogic	Code	Cannot be empty	900
37.	SystemCountryCodeLogic	Name	Cannot be empty	901
38.	SystemLanguageCodeLogic	LanguageID	Cannot be empty	1000
39.	SystemLanguageCodeLogic	Name	Cannot be empty	1001
40.	SystemLanguageCodeLogic	NativeName	Cannot be empty	1002
