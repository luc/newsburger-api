News
=====

### `GET /v2/news.json`

| Parameter                       | Required | Example                                                                                                                                           |
| ------------------------------- | -------- | ------------------------------------------------------------------------------------------------------------------------------------------------- |
| `page: number`                  | false    | `GET /v2/news.json?page=2`  will get page two of the available entries |
| `since: date`                   | false    | `GET /v2/news.json?since=1527450408` will get all news created after the unix timestamp.|
| `ids: number`                    | false    | `GET /v2/news.json?id=1,2,3`  will get the news with the id 1.|
| `per_page: number`              | false    | `GET /v2/news.json?per_page=50`  will limit results to 50 per page.|
| `language: string`              | false    | `GET /v2/news.json?language=lb`  will get all news of language lb.|
| `category: string`              | false    | `GET /v2/news.json?category=Politics`  will get all news of category politics. 

### `GET /v2/news/666.json`

### `PUT /v2/news/666/actions/click`

### `GET /v2/feeds/666/news.json`



**Status Codes**

- `200 OK` will be returned if found
- `404 Not Found` will be returned if no news are found
