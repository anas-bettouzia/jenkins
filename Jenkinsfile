pipeline {
    agent any
    stages {
    stage('MVN SONARQUBR') {
        steps {
            withSonarQubeEnv(installationName: 'sq1') {
                sh './mvnw clean org.sonarsource.scanner.maven:sonar-maven-plugin:3.9.0.2155:sonar'
            }
        }
    }
}

}
