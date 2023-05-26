pipeline {
    agent any 
    stages {
        stage("vcs") {
           steps {
               git url: 'https://github.com/spring-projects/spring-petclinic.git',
                   branch: 'main'
           }
       }
       stage("MAVEN_GOAL") {
          steps {
            sh "mvn package"
        }  
       }
             
    }
}
