

pipeline {
    agent any
    triggers {
    GenericTrigger(
     genericVariables: [
      [key: 'ref', value: '$.ref']
     ],
    )
  }
    stages {
      stage('Bootstrap n Transpile') {
        steps {
          sh 'echo $ref'
          
        }
      }
    }
}
