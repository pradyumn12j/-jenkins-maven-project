pipeline
{
    agent any
    stages
    {
        stage("hey there")
        {
            steps{withMaven(globalMavenSettingsConfig: '', jdk: 'JAVA_HOME', maven: 'MAVEN_HOME', mavenSettingsConfig: '', traceability: true) {
                sh 'mvn install'

}}
        }
        //stage('deploy to tomcat server')
//{steps { sshagent(credentials: ['test'])
//{
//	sh 'scp -o StrictHostKeyChecking=no java-test/target/hello-app-1.0.jar ec2-user@172.31.18.254:/usr/share/tomcat/webapps'

//s} }}

    }
}