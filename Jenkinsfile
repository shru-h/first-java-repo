pipeline{
        agent any
        stages{
            stage("stage1 : checkout stage"){
                steps{
                    git branch :'main' , url: 'https://github.com/shru-h/first-java-repo'
            
                }
            }
            stage("stage2 : compile the code"){
                steps{
                    sh "mvn compile"
                }
            }
            stage("stage3 : unit test"){
                steps{
                    sh "mvn test"
                }
            }
            stage("stage4 : QA"){
                steps{
                    sh "mvn pmd:pmd"
                }
            }
            stage("stage5 : package"){
                steps{
                    sh "mvn package"
            }
    
        }
    }
}
