node('master') 
{
    stage('Job - Calc-Webapp branch') 
    {
        echo 'Hello Mr. Praveen....Welcome to World of MBP...Here is the Calc-Webapp-Project !!!'
    }
}

node('master')
{
    stage('S1-Cont. Downld')
    {
        git 'https://github.com/praveenpeyala/calcwebapp.git'
    }
}

node('master')
{
    stage('S2-Cont. Build')
    {
        sh 'mvn clean package'
    }
}
