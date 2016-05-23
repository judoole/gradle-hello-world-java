node {
    stage 'Assemble'
    sh './gradlew.sh assemble --parallel'
    
    stage 'Unit-Test'
    sh './gradlew.sh test --parallel'
}
