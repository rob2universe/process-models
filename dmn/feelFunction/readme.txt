Example usage of input variable and FEEL expressions in input expression and rule

FEEL Functions:
https://camunda.github.io/feel-scala/1.11/feel-expression

{{rest_url}}/decision-definition/key/Decision_UpperCase/evaluate
localhost:8080/engine-rest/decision-definition/key/Decision_UpperCase/evaluate

POST Body:
a)
{
  "variables": {
    "input1": {
      "type": "String",
      "value": "1Bob"
    }
  }
}

b)
{
  "variables": {
    "input1": {
      "type": "String",
      "value": "Pete"
    }
  }
}

Result:
a)
[
    {
        "result": {
            "type": "String",
            "value": "BOB",
            "valueInfo": {}
        }
    }
]

b)
[
    {
        "result": {
            "type": "String",
            "value": "Pete",
            "valueInfo": {}
        }
    }
]
