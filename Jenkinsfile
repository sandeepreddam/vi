pipeline
{
    agent any
    stages
  {
      stage('1')
            {
              steps
              {
                sh 'git clone https://github.com/RavitejaAdepudi/javawar.git'
              }
              
            }
      stage('2')
            {
                steps
                {
                    sh 'export MAVEN_HOME=/opt/apache-maven-3.9.8 && export PATH=$PATH:/opt/apache-maven-3.9.8/bin && mvn -f /var/lib/jenkins/workspace/two/javawar/pom.xml clean'
                }
            }
      stage('3')
      {
          steps
          {
              sh 'mvn tomcat7:deploy'
          }
      }
            
  }
  
}
