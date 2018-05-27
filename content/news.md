News
=====

Get News
--------

### `GET /v2/news.json`

| Parameter                       | Required | Example                                                                                                                                           |
| ------------------------------- | -------- | ------------------------------------------------------------------------------------------------------------------------------------------------- |
| `page: number`                  | false    | `GET /v2/entries.json?page=2`  will get page two of the available entries                                                                         |
| `since: date`                   | false    | `GET /v2/entries.json?since=2013-02-02T14:07:33.000000Z` will get all entries created after the iso 8601 timestamp.                               |
| `ids: number(s)`                | false    | `GET /v2/entries.json?ids=1,2,3`  will get the entries with the ids 1, 2 and 3.                                                                   |
| `starred: boolean`              | false    | `GET /v2/entries.json?starred=true`  will get all starred entries.                                                                                |
| `per_page: number`              | false    | `GET /v2/entries.json?per_page=50`  will limit results to 50 per page.                                                                            |
| `mode: enum`                    | false    | `GET /v2/entries.json?mode=extended`  the only mode available is `extended`. This includes more metadata for the entry                            |
| `include_original: boolean`     | false    | `GET /v2/entries.json?include_original=true`  include original entry data if the entry has been updated.                                          |
| `include_enclosure: boolean`    | false    | `GET /v2/entries.json?include_enclosure=true`  include podcast/RSS enclosure data.                                                                |
| `include_content_diff: boolean` | false    | `GET /v2/entries.json?include_content_diff=true`  include a diff of changed content. Result is HTML marked up to show differences. 

**Status Codes**

- `200 OK` will be returned if found
- `404 Not Found` will be returned if no news are found
