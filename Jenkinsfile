pipeline {
    agent any
    stages {
        stage('build matchengine') {
            when {
                changeset "**/spring-petclinic-config-server/*.*"
            }
            steps {
                echo 'building match engine'
            }
        }
        stage('build posttrade') {
            when {
                changeset "**/spring-petclinic-customers-service/*.*"
            }
            steps {
                echo 'building post trade'
            }
        }
    }
}
