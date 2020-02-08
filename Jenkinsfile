

pipeline {
    agent any
    triggers {
    GenericTrigger(
     genericVariables: [
      [key: 'ref', value: '$.ref']
     ]
    )
  }
    stages {
      stage('pull reps') {
        steps {
          sh 'echo $ref'
          
        }
      }
    }
}
