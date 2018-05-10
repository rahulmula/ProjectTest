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
    }
    }