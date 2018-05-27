Comments
=====

### `GET /v2/comments.json`

| Parameter                       | Required | Example                                                                                                                                           |
| ------------------------------- | -------- | ------------------------------------------------------------------------------------------------------------------------------------------------- |
| `id: number`                    | false    | `GET /v2/comments.json?id=1`  will get the comment with the id 1.|
| `author: string`                | false    | `GET /v2/comments.json?author=luc`  will get all comments from luc|


**Status Codes**

- `200 OK` will be returned if found
- `404 Not Found` will be returned if no news are found
