pipeline{
    agent any {
        stages
        {
            stage('Checkout')
            {
                steps{
git url:'https://github.com/snehachopra1611/Project_S2.git'
branch : 'main'
                }
            }
                 stage('Test')
            {
                steps{
sh 'test -f index.html'
echo 'File Found'
                }
            }
        }
            post {
                success{
                    echo 'Pipeline Executed Successfully'
                }
                failure{
                    echo 'Pipeline Failed'
                }
            }
        }
    }
