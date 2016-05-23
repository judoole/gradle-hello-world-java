node {
    checkout scm
    stage 'Assemble'
    sh './gradlew clean assemble --parallel'
    
    stage 'Unit-Test'
    sh './gradlew test --parallel'
    step([$class: 'JUnitResultArchiver', testResults: 'build/test-results/**/*.xml'])
}
