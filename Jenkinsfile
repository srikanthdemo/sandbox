pipeline {
  agent any
  options([pipelineTriggers([cron('* * * * *')])])
  //triggers { cron('* * * * *') }
  /*
  triggers {
    GenericTrigger(
     genericVariables: [
      [key: 'ref', value: '$.ref']
     ],
     causeString: 'Triggered on $ref',
     
     token: 'abc123',
     
     printContributedVariables: true,
     printPostContent: true,
    
     regexpFilterText: '$ref',
     regexpFilterExpression: 'refs/heads/' + BRANCH_NAME
    )
  } 
  */
  stages {
    stage('Some step') {
      steps {
        sh "echo $ref"
      }
    }
  }
}
