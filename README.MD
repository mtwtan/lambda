# Useful code snippets for Lambda Function

## Scratch pad

### Running python scripts locally like in Lambda functions
```
$ python -c 'event="{ 'key': 'value' }";context="{'key': 'value'}";from <name of python script (without .py)> import <name of function in script>;print(<function name>(event,context))'
```
#### Example
```
'event="{ 'who': 'StepF' }";context="{'something': 'another'}";from learnStepFunctions import lambda_handler;print(lambda_handler(event,context))'
```
