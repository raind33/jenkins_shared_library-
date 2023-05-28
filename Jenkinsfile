@Library('MyLib')

def tools = new org.devops.tools()
pipeline {
  agent 'none'
  stages {
    stage('test') {
      steps {
        scipt{
          println(tools.getName())
        }
      }
    }
  }
}

