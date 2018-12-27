def workspace;
node
{
    stage('checkout'){
        checkout([$class: 'GitSCM', branches: [[name: '*/master']], doGenerateSubmoduleConfigurations: false, extensions: [], submoduleCfg: [], userRemoteConfigs: [[credentialsId: 'jfile', url: 'https://github.com/ismailmalik/Jfiles.git']]])
        workspace =pwd()
    }
    stage('Static Code Analysis'){
        echo "Static Code Analysis"
    }
    stage('Build'){
        echo "Build the code"
    }
    stage('Unit Test'){
        echo "Unit Test"
    }
    stage('Delivery'){
        echo "Deliver the code"
    }
}
