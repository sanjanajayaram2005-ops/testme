pipeline {
  agent any
  tools {
    jdk 'jdk'
  }
  stages { 
    stage ('Checkout')
    {
      steps
    {
      git 'https://github.com/sanjanajayaram2005-ops/testme.git'
    }
    }
    stage ('Build')
{
steps
{
 sh 'chmod +x gradlew'
sh './gradlew build'
}
}
    stage ('Test')
{
steps
{
sh './gradlew test'
}
}
stage ('Run')
{
steps
{
sh './gradlew run'
}
}
}
}
