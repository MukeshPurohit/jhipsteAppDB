node {
    stage('Database Build TBD') {
        echo 'Building....'
        sh 'java -version'
        sh 'wget https://repo1.maven.org/maven2/org/flywaydb/flyway-commandline/5.0.2/flyway-commandline-5.0.2-linux-x64.tar.gz'
        sh 'mkdir -p flyway && tar -xvf flyway-commandline-5.0.2-linux-x64.tar.gz -C flyway'
        sh 'pwd' 
        sh 'cd /var/lib/jenkins/workspace/jhipster_App_DB_pipeline'
        sh 'flyway info'
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
