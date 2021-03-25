pipeline {
    //small change 2
    //pls work
    agent any

    stages {
//         stage('Build') {
//             steps {
//                 git 'https://github.com/ScarlettQnR/test2'
//                 bat 'mvn clean compile'
//             }
//         }
//

        stage('build') {
        steps{

         def cmd_exec(command) {
                    return bat(returnStdout: true, script: "${command}").trim()
                }


        git 'https://github.com/ScarlettQnR/test2'
              cmd_exec('echo "Buils starting..."')
              cmd_exec('mvn clean compile')
        }




//
//         stage('Test') {
//             steps{
//                 bat 'mvn test'
//             }
//
//             post{
//                 always {
//                     junit '**/target/surefire-reports/TEST-*.xml'
//                 }
//             }
//         }
//         stage('Publish'){
//             steps{
//                 bat 'mvn package'
//             }
//             post{
//                 success{
//                     archiveArtifacts 'target/*.jar'
//                 }
//             }
//     }
}
}
}