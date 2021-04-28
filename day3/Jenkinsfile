pipeline {
agent any
stages {
stage('Maven Compile'){
steps{
echo 'Project compile stage'
bat label: 'Changing Directory...',script: '''cd day3'''
bat label: 'Compilation running', script: '''mvn compile'''
}
}
stage('Unit Test') {
steps {
echo 'Project Testing stage'
bat label: 'Test running', script: '''mvn test'''
}
}
stage('Maven Package'){
steps{
echo 'Project packaging stage'
bat label: 'Project packaging', script: '''mvn package'''
}
}
}
}
