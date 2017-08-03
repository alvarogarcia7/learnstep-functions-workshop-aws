Set up the environment:

```bash
alias sls="./node_modules/serverless/bin/serverless"
```

Deploy:

```
sls deploy
```

Invoke:

```bash
sls invoke stepf --name rpg --data '"hello"'
```

outputs something like:

```
{ executionArn: 'arn:aws:states:eu-west-1:815886228738:execution:RpgStepFunctionsStateMachine-FR4OKHXG1E9U:0db4de16-0c34-422d-b562-6ffbe9e12b95',
  stateMachineArn: 'arn:aws:states:eu-west-1:815886228738:stateMachine:RpgStepFunctionsStateMachine-FR4OKHXG1E9U',
  name: '0db4de16-0c34-422d-b562-6ffbe9e12b95',
  status: 'SUCCEEDED',
  startDate: 2017-08-03T18:04:25.266Z,
  stopDate: 2017-08-03T18:04:25.304Z,
  input: '"hello"',
  output: '"hello"' }
```
