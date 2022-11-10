@Library("shared-libs") _

pipeline {
    agent any

    stages {
        
        stage('Build_Project') {
            steps {
                echo 'Building whole project here!'
                sayHello()
                saySuccess()
//                 sayFailure()
            }
            post {
                success {
                    echo 'Succeeded in Build_Project Stage.'
                }
                failure {
                    echo 'Failed in Build_Project Stage.'
                }
            }
        }
        
        stage('Parallel Stage') {
            parallel {
                stage('Test_A') {
                    steps {
                        echo 'Testing_A on project here!'
                        sayHello()
                        saySuccess()
                    }
                    post {
                        success {
                            echo 'Succeeded in Test_A Stage.'
                        }
                        failure {
                            echo 'Failed in Test_A Stage.'
                        }
                    }
                }
                
                stage('Test_B') {
                    steps {
                        echo 'Test_B on project here!'
                        sayHello()
                        saySuccess()
                    }
                    post {
                        success {
                            echo 'Succeeded in Test_B Stage.'
                        }
                        failure {
                            echo 'Failed in Test_B Stage.'
                        }
                    }
                }
                
                stage('Test_C') {
                    steps {
                        echo 'Test_C on project here!'
                        sayHello()
                        saySuccess()
                    }
                    post {
                        success {
                            echo 'Succeeded in Test_C Stage.'
                        }
                        failure {
                            echo 'Failed in Test_C Stage.'
                        }
                    }
                } 
                
            }
        }
    
        stage('Test_D') {
            steps {
                echo 'Test_D on project here!'
                sayHello()
                saySuccess()
            }
            post {
                success {
                    echo 'Succeeded in Test_D Stage.'
                }
                failure {
                    echo 'Failed in Test_D Stage.'
                }
            }
        } 
        
        stage('Test_E') {
            steps {
                echo 'Test_E on project here!'
                sayHello()
                saySuccess()
            }
            post {
                success {
                    echo 'Succeeded in Test_E Stage.'
                }
                failure {
                    echo 'Failed in Test_E Stage.'
                }
            }
        }
        
        stage('Build_Deliverable') {
            steps {
                echo 'Building Deliverables here!'
                sayHello()
                saySuccess()
            }
            post {
                success {
                    echo 'Succeeded in Build_Deliverable Stage.'
                }
                failure {
                    echo 'Failed in Build_Deliverable Stage.'
                }
            }
        }
        
        stage('Deploy_Dev') {
            steps {
                echo 'Deploying on Dev environment here!'
                sayHello()
                saySuccess()
            }
            post {
                success {
                    echo 'Succeeded in Deploy_Dev Stage.'
                }
                failure {
                    echo 'Failed in Deploy_Dev Stage.'
                }
            }
        }
        
        stage('Deploy_Prod') {
            steps {
                echo 'Deploying on Prod environment here!'
                sayHello()
                saySuccess()
            }
            post {
                success {
                    echo 'Succeeded in Deploy_Prod Stage.'
                }
                failure {
                    echo 'Failed in Deploy_Prod Stage.'
                }
            }
        }  
    
    }
}
