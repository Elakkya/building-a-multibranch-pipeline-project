node(){
    properties([
  pipelineTriggers([
   [$class: 'GenericTrigger',
    genericVariables: [
     [key: 'ref', value: '$.ref'],
     [
      key: 'before',
      value: '$.before',
      expressionType: 'JSONPath', //Optional, defaults to JSONPath
      regexpFilter: '', //Optional, defaults to empty string
      defaultValue: '' //Optional, defaults to empty string
     ]
    ],
     causeString: 'Triggered on $ref',
    // regexpFilterText: '$repository $ref',
   // regexpFilterExpression: 'building-a-multibranch-pipeline-project refs/heads/' + BRANCH_NAME,
     printContributedVariables: true,
     printPostContent: true,
     token: 'abc123',
     silentResponse: false,   
   ]
  ])
 ])
    stage('Build'){
        sh 'echo "Hello world!"'
    }
}
