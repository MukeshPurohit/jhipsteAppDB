node {
    stage('Database Build TBD') {
        echo 'Building....'
        def exists = fileExists 'flyway-commandline-5.0.2-linux-x64.tar.gz'
        if (exists) {
            echo 'flyway-commandline-5.0.2-linux-x64.tar.gz already exist and skipping re-downloading...'
        } else {
            echo 'flyway-commandline-5.0.2-linux-x64.tar.gz does not exist at server. Downloading new copy...'
            sh 'wget https://repo1.maven.org/maven2/org/flywaydb/flyway-commandline/5.0.2/flyway-commandline-5.0.2-linux-x64.tar.gz'
            sh 'tar -xvf flyway-commandline-5.0.2-linux-x64.tar.gz'
        }
        
        sh 'checkout scm https://github.com/MukeshPurohit/jhipsterSampleDB.git'
        
        sh 'checkout scm https://github.com/MukeshPurohit/jhipsterSampleApp_v1.git'
        
        dir ('/var/lib/jenkins/workspace/jhipster_App_DB_pipeline/flyway-5.0.2') {
            sh 'ls -lart'
            sh 'mv flyway flyway.sh'
            sh 'chmod 777 *.*'
            sh './flyway.sh info'
        }   
        
       
    }
    stage('Database Test TBD') {
        echo 'Building....'
    }
    stage('Database Deploy TBD') {
        echo 'Deploying....'
    }
    stage('Database Build TBD') {
        echo 'Building....'
    }
    stage('Database Test TBD') {
        echo 'Building....'
    }
    stage('Database Deploy TBD') {
        echo 'Deploying....'
    }
}
