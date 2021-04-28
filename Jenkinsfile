node('master') 
{
    stage('Continuous Download_loans') 
	{
    git 'https://github.com/sunildevops77/maven.git'
	}
    stage('Continuous Build_loans') 
	{
    sh label: '', script: 'mvn package'
	}
    stage('Continuous Deployment_loans') 
	{
sh label: '', script: 'scp /home/ubuntu/.jenkins/workspace/Pipelinepro/webapp/target/webapp.war   ubuntu@172.31.38.27:/var/lib/tomcat8/webapps/qaenv.war'
	}
    
}
