node {
    stage 'Assemble'
    sh './gradlew assemble --parallel'
    
    stage 'Unit-Test'
    sh './gradlew test --parallel'
}
