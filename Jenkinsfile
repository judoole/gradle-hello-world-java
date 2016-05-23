node {
    git url: 'https://github.com/judoole/gradle-hello-world-java.git'
    stage 'Assemble'
    sh 'gradlew assemble --parallel'
    
    stage 'Unit-Test'
    sh 'gradlew test --parallel'
}
