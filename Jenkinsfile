

pipeline {
    agent any
    triggers {
    GenericTrigger(
     genericVariables: [
      [key: 'ref', value: '$.ref']
     ],
     causeString: 'Triggered on $ref',
     token: 'abc123*',
     printContributedVariables: false,
     printPostContent: false,
     silentResponse: false,
     regexpFilterText: '$ref',
     regexpFilterExpression: 'master$'
    )
  }
    stages {
      stage('pull reps') {
        steps {
          sh 'echo "execelente!"'
          
        }
      }
    }
}
