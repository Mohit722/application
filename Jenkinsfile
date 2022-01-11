pipeline{
  agent any
  enviroment{
    def value = readProperties file: 'some.properties'
    person = "${value.name}"
    deployTo = "${value.env}" 
  }
  stages{
    stage('echo name'){
      steps{
        echo "${person}"
        echo "${deployTo}
      }
    }
  }
}
