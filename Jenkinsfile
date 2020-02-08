

pipeline {
    agent any
    triggers {
    GenericTrigger(
     genericVariables: [
      [key: 'ref', value: '$.ref']
     ],

     causeString: 'Triggered on $ref',

     token: 'abc123*',

     printContributedVariables: true,
     printPostContent: true,

     silentResponse: false,

     regexpFilterText: '$ref',
     regexpFilterExpression: 'refs/heads/master'
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
