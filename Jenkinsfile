
pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                echo 'Building Employee Salary Calculator'
            }
        }

        stage('Calculate Salary') {
            steps {
                script {
                    def basic = 20000
                    def hra = 5000
                    def bonus = 2000
                    def total = basic + hra + bonus

                    echo "Basic Salary: ${basic}"
                    echo "HRA: ${hra}"
                    echo "Bonus: ${bonus}"
                    echo "Total Salary: ${total}"

                    if (total == 27000) {
                        echo 'Salary Test Passed'
                    } else {
                        error 'Salary Test Failed'
                    }
                }
            }
        }

        stage('Deploy') {
            steps {
                echo 'Salary Calculator Ready'
            }
        }
    }
}
