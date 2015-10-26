#custom-page-archetype

##How to build the archetype

```
cd custom-page-archetype
mvn clean install -DskipTests
```

##How to use the archetype

```
mvn archetype:generate \
-DarchetypeGroupId=org.bonitasoft.web \ 
-DarchetypeArtifactId=custom-page-archetype \ 
-DarchetypeVersion=1.0.0-SNAPSHOT \
-DgroupId=org.company.api \
-DartifactId=myCustomPage \
-Dversion=0.0.1-SNAPSHOT
```

###Optionnal archetype parameters


| Parameter         		| Default value                     | Description                                                                            										   |
| --------------------------|-----------------------------------|----------------------------------------------------------------------------------------------------------------------------------|
| -DbonitaVersion   		| 7.0.1                             | You can choose the version of the dependent bonita artifacts. Minimum version is 7.0.1.										   |
| -DcustomPageName      	| myCustomPage               		| Set the name of your api extension. You must enter an url friendly name without blanks. 									       |
| -DcustomPageDisplayName 	| My Custom Page             		| A display name for your api extension (displayed in the portal for the administrator) 										   |
| -DcustomPageDesc         	| My Custom Page description 		| A short description of the purpose of your api extension (displayed in the portal for the administrator) 						   |
| -DpathTemplate    		| myCustomPageApi                   | URL path template. Resulting url: ../API/extension/myRestExtApi 																   |
| -DpermissionNames 		| myCustomPagePermission               | Define permission list (comma separated value), specify permissions a user need to have in order access this REST API >extension |
| -DurlParameters   		| ! (none)                          | Define a list (comma separated value) of url parameters.                                                                         |
 
