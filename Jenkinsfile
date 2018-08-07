node {

properties([
 pipelineTriggers([
  [$class: 'GenericTrigger',
   genericVariables: [
    [expressionType: 'JSONPath', key: 'variable1', value: 'expression1'],
    [expressionType: 'JSONPath', key: 'variable2', value: 'expression2']
   ],
   regexpFilterText: 'hej',
   regexpFilterExpression: ''
  ]
 ])
])

stage("build") {
 sh '''
 echo Build
 '''
}

}
