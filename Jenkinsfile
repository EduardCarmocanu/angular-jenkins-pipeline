pipeline{
    agent{
        label "any"
    }
    stages{
        stage("Prerequisites"){
            steps{
                echo "getting prerequisites"
                sh "npm install"
            }
        },
        stage("lint") {
            steps{
                echo "linting files"
                sh "ng lint"
            }
        }
        stage("test") {
            steps{
                echo "testing application"
                sh "npm run test"
            }
        }
    }
}