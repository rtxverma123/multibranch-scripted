node{
    if (env.BRANCH_NAME == 'master'){
        stage('Build master'){
            echo 'Builing the code'
            sh 'docker build -t rtxverma123/myubuntu .'
        }

    }

    if (env.BRANCH_NAME == 'deploy'){
        stage('Deploy code'){
            echo 'Deploying the code'
            sh 'kubectl apply -f deploy.yaml'

        }
    }
}