pipeline {

  agent any 
  stages {
    stage("Build"){
      steps {
        echo "Hello jenkins, this my first pipeline !!"
      } 
  }    
    stage("Test"){
      steps {
        echo "Testing ..!!"
        sh echo "hello world !"
      }
  }
      stage("deploy"){
      steps {
        echo "Deploying ..!!"
      }
  }
}
}
