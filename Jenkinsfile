@Library('MyLib')

def tools = new org.devops.tools()
pipeline {
  agent 'none'
  stages {
    stage('test') {
      steps {
        script{
          println(tools.getName())
          // vars output
          println(GetNameById())
          // resource
          def data =  libraryResource 'config/config.json'
          println(data)
          // 需要安装pipeline utils plugin
          data_json = readJSON text: data
          println(data_json)
        }
      }
    }
  }
}

