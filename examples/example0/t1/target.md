## Target


### Current

currentState = [1, 2];

| id  | text  | updatedTime |
|:--- |:----- | ----------- |
| 1   | text1 | 1           |
| 2   | text2 | 2           |


### Next

| id  | text  | updatedTime |
|:--- |:----- | ----------- |
| 5   | text5 | 5           |
| 6   | text6 | 6           |


## Diff

```json
{
  "create": [5, 6],
  "remove": [1, 2],
  "update": [],
  "data": {
    "5": {
      "text": "text5",
      "updatedTime": 5
    },
    "6": {
      "text": "text6",
      "updatedTime": 6
    }
  }
}
```
