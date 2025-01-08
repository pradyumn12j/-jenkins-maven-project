pipeline
{
    agent any
    stages
    {
        stage('Build') {
            steps {
                sh 'mvn -f hello-app/pom.xml -B -DskipTests clean package'
            }
        }
        stage("hey there")
        {
            steps{withMaven(globalMavenSettingsConfig: '', jdk: 'JAVA_HOME', maven: 'MAVEN_HOME', mavenSettingsConfig: '', traceability: true) {
                sh 'mvn test'

}}
        }
    }
}