node {
    stage "Checkout"
        checkout scm
  withMaven(
        maven: 'maven' )
    stage "Build"
    sh "mvn clean build "
    
    stage "test"
    sh "mvn test"
    
    stage "Packaging"
    sh "mvn clean Package"
    
    stage "Deploy to Azure"
    echo "XXXXXX"    
}
