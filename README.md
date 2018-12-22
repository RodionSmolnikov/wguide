# wguide

Gradle: 5.0
ktor:1.0.1
docker (linux container):2.0.0.0-win81 
kotlin:1.3

## Running

Execute this command in the repository's root directory to run this sample:

```bash
gradle build
```

To build and run a docker image:

```bash
gradlew build
docker build .  -t wguide:v1
docker run -m512M --cpus 2 -it -p 8080:8080 --rm wguide:v1
```
 
And navigate to [http://localhost:8080/](http://localhost:8080/) to see the sample home page.  

