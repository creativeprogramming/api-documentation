# Collections Resources

    DELETE collections/:ID

## Description
Deletes collection.

***

## Requires authentication
**[OAuth][]**

***

## Return format
A JSON object with **collections** — An indexed array of Collection objects in **[short format][]**.:

***

## Errors
None

***

## Example
**Request**

    GET v1/collections

**Return**
``` json
  {
    collections: [
      {
        id: 289621,
        title: "Film set",
        position: 0,
        created_at: "2012-05-24T10:13:34-04:00",
        path: "film_set",
        photos: [
          {
            id: 7903457,
            name: "Sugar beach Toronto",
            rating: 0,
            created_at: "2012-05-24T10:13:51-04:00",
            category: 0,
            image_url: "http://pcdn.500px.net/7903457/242b9680955c0198bb0eb0eed3331ac899825d13/4.jpg",
            votes_count: 0,
            position: 0
          },
          {
            id: 7905188,
            name: "St Lawrence Market Toronto",
            rating: 0,
            created_at: "2012-05-24T11:22:46-04:00",
            category: 3,
            image_url: "http://pcdn.500px.net/7905188/9e1fcf034f7492c92d0f98e504d80c0b80e15990/4.jpg",
            votes_count: 0,
            position: 1
          }
        ]
      },
      {
        id: 298603,
        title: "Bikes set",
        position: 0,
        created_at: "2012-06-07T13:15:26-04:00",
        path: "bikes_set",
        photos: [
          {
            id: 7651996,
            name: "bike",
            rating: 48.7,
            created_at: "2012-05-16T11:47:12-04:00",
            category: 26,
            image_url: "http://pcdn.500px.net/7651996/bfc9a0ae7cfaed28ebc947c2d4cd79e60a04934d/4.jpg",
            votes_count: 2,
            position: 999
          }
        ]
    ]
  }
```

[OAuth]: https://github.com/500px/api-documentation/tree/master/authentication
[Feature]: https://github.com/500px/api-documentation/blob/master/basics/formats_and_terms.md#500px-photo-terms
[short format]: https://github.com/500px/api-documentation/blob/master/basics/formats_and_terms.md#short-format-1