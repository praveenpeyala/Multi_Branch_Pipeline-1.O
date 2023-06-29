node('master') 
{
    stage('Job -  Hello-world branch') 
    {
        echo 'Hello Mr. Praveen....Welcome to the World of MBP...Here is the  Hello-world-Project-Pipeline !!!'
    }
}

node('master')
{
    stage('S1-Cont. Downld')
    {
        git 'https://github.com/praveenpeyala/hello-world.git'
    }
}

node('master')
{
    stage('S2-Cont. Build')
    {
        sh 'mvn clean package'
    }
}

node('master')
{
    stage('S3-Cont. Deploy')
    {
        deploy adapters: [tomcat8(credentialsId: '3b8c23a9-21f9-4012-b3a9-f4ae496c4b08', path: '', url: 'http://172.31.35.114:8080/')], contextPath: 'Tomcat-QA-MBP-Hello-World', war: '**/*.war'
    }
}

node('master')
{
    stage('S4-Cont. Test')
    {
        echo 'The war file has passed all the tests...Now you can go for deployment of that war file in Production Server'
    }
}
