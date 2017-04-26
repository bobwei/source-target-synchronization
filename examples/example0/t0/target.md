## Target


### Current

currentState = [];

| id  | text | updatedTime |
|:--- |:---- | ----------- |
|     |      |             |


### Next

| id  | text  | updatedTime |
|:--- |:----- | ----------- |
| 1   | text1 | 1           |
| 2   | text2 | 2           |


## Diff

```json
{
  "create": [1, 2],
  "delete": [],
  "update": [],
  "data": {
    "1": {
      "text": "text1",
      "updatedTime": 1
    },
    "2": {
      "text": "text2",
      "updatedTime": 2
    }
  }
}
```
