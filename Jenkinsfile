node {

    stage('build') {
        try {
            sh 'echo "build in progress"'
        } 
        catch (Exception e) {
            sh 'echo "build failed"'
            throw e
        }
    }

    stage('test') {
        if (env.BRANCH_NAME == 'feat') {
            sh 'echo "skip testing"'
        } 
        else {
            sh 'echo "test in progress"'
        }
    }

}