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
