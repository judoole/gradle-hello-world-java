node {
    checkout scm
    stage 'Assemble'
    sh './gradlew clean assemble --parallel'
    
    stage 'Unit-Test'
    sh './gradlew test --parallel'
    step([$class: 'JUnitResultArchiver', testResults: 'build/test-results/**/*.xml'])
    
    checkpoint 'about to deploy'
    stage 'Deploy to PROD'
    input message: 'Release to Production', ok: 'Release'
    sh 'We deployed the app'
}
