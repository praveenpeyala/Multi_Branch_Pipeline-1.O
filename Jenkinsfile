node('master') 
{
    stage('Job - Pvn-War-File branch') 
    {
        echo 'Hello Mr. Praveen....Welcome to World of MBP...Here is the Prvn-War-File-Project !!!'
    }
}

node('master')
{
    stage('S1-Cont. Downld')
    {
        git 'https://github.com/praveenpeyala/Prvn-WAR-file.git'
    }
}

node('master')
{
    stage('S2-Cont. Build')
    {
        sh 'mvn clean package'
    }
}
