node('master') 
{
    stage('Job - Address-Book branch') 
    {
        echo 'Hello Mr. Praveen....Welcome to World of MBP....Here is the Address-Book-Project !!!'
    }
}

node('master')
{
    stage('S1-Cont. Downld')
    {
        git 'https://github.com/praveenpeyala/addressbook.git'
    }
}

node('master')
{
    stage('S2-Cont. Build')
    {
        sh 'mvn clean package'
    }
}
