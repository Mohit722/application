pipeline{
  agent any
  enviroment{
    def param = readJSON file: 'some.json'
    msg = "${param.Hello}"
  }
  stages{
    stage('Echo'){
      steps{
        echo "$(msg)"
      }
    }
  }
}
