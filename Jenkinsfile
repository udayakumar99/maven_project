pipeline
{
  agent any
  stages
  {
    stage("GIT")
    {
      steps
      {
        git branch: 'main', url: 'https://github.com/udayakumar99/maven_project.git'
      }
    }
    stage("clean")
    {
      steps
      {
        sh "mvn clean"
      }
    }
    stage("install")
    {
      steps
      {
        sh "mvn install"
      }
    }
    stage("shellgit1")
    {
      steps
      {
        git branch: 'patch-1', url: 'https://github.com/udayakumar99/maven_project.git'
        sh "bash sample.sh"
      }
    }
    
        
  }
}
