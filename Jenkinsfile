node {
  try {
    stage('checkouts') {
        deleteDir()
        sh 'id'
        stage('Jenkinsfile utility')
        git 'https://github.com/rahulmula/ProjectTest.git'
        def rootDir = pwd()
        def ci_method = load "jenkins_class.groovy"
        ci_method.ci_build_steps()
    }
    stage('Static code analysis')
    {
      echo "Test the code"
    }
    stage('Build')
    {
      echo "Build the code"
    }
    }
    }
