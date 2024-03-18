
# Android Component for displaying Error and Messages.
 
This library contains various functions like message(parameters), error(parameters), internetError(parameters)etc.
### Deployment
 
To get a Git project into your build:
 
#### Step 1. Add the JitPack repository to your build file
 
Add it in your root build.gradle at the end of repositories:
 
```bash
  dependencyResolutionManagement {
		repositoriesMode.set(RepositoriesMode.FAIL_ON_PROJECT_REPOS)
		repositories {
			mavenCentral()
			maven { url 'https://jitpack.io' }
		}
	}
```
 
#### Step 2. Add the dependency
 
```bash
dependencies {
	        com.github.cbb-intelliswift:ErrorMessagesAndroid:1.1.1'
}
 
```
 
### Importent things to remember
 
To use this library we have to make sure that minSDK of app level and module level build.gradle set to 24.
 
 
### Description about the functions
 
This library contains 4 functions.
 
    1. message(parameters)
       This function shows suitable UI for a message.
       We can define this function like below:
 
            fun message (message: String? = null, actionTitle: String? = null, action: ((v: View) - Unit)? = null): State = State(
            status = MESSAGE,
            message = message,
            actionTitle = actionTitle,
            action = action
            )
 
    2. showError(parameters)
       This function shows show suitable UI for an error.
       We can define this function like below:
 
            fun error (message: String? = null, actionTitle: String? = null, action: ((v: View) - Unit)? = null): State = State(
            status = ERROR,
            message = message,
            actionTitle = actionTitle,
            action = action
            )

    3. showInternetError(parameters)
       This function shows suitable UI for an Internet not found error.
       We can define this function like below:
 
            fun internetError (message: String? = null, actionTitle: String? = null, action: ((v: View) - Unit)? = null): State = State(
            status = INTERNET_ERROR,
            message = message,
            actionTitle = actionTitle,
            action = action
            )

    4. showNoData(parameters)
       This function shows suitable UI for Data Not Available.
       We can define this function like below:
 
            fun noData (message: String? = null, actionTitle: String? = null, action: ((v: View) - Unit)? = null): State = State(
            status = NO_DATA,
            message = message,
            actionTitle = actionTitle,
            action = action
            )
