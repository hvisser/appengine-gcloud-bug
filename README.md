This is a simple test project to demonstrate a bug I ran into when running this App Engine project using `gcloud preview app run`.
To reproduce:

* run the app from Gradle by using `./gradlew appengineRun` --> open up `http://localhost:8080`, you should see a Hello world welcome
* Quit the process and prepare the app to be ran by `gcloud` using `./gradlew appengineStage`
* run the app using gcloud: `gcloud preview app run build/`