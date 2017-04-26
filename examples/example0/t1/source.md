## Source


### Current

currentState = [1, 2];

| id  | text  | updatedTime |
|:--- |:----- | ----------- |
| 1   | text1 | 1           |
| 2   | text2 | 2           |


### Next

| id  | text  | updatedTime |
|:--- |:----- | ----------- |
| 1   | text1 | 1           |
| 3   | text3 | 3           |
| 4   | text4 | 4           |


## Diff

```json
{
  "create": [3, 4],
  "delete": [2],
  "update": [],
  "data": {
    "3": {
      "text": "text3",
      "updatedTime": 3
    },
    "4": {
      "text": "text4",
      "updatedTime": 4
    }
  }
}
```
