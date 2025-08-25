node{
    git branch: 'main',  url:'https://github.com/mahmoudmarabeh/SimpleApi.git'
    stage('build'){
        try{
        sh'echo "build stage"'
        }
        catch(Exception ex){
            sh'echo "excption found "'
            throw ex
        }
    }
    stage('test'){
        if (env.BRANCH_NAME == "feature"){
            sh'echo "test stage"'
        }
        else{
            sh'echo "skip test stage"'
        }
    }
}