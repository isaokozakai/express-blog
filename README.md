# Data Structure
```
database name: ciccc
collection name: posts

[{
  "id": string,       //for editting, deleting, voting
  "date": string,     //for date
  "author": string,   //for name
  "title": string,    //for title
  "content": string,  //for blog main content
  "comments": [{      //for comments
    "date": string,
    "name": string, 
    "commentContent": string
  }]
}]
```
# Routing

``GET "/"`` =                     Top Page

``GET /posts/form`` =             Form Page for a new post

``POST /posts`` =                 Create a new post

``GET /posts/:id`` =              Read Page

``GET /posts/:id/form`` =         Form Page for an existing post

``POST /posts/:id/comments`` =      Leave a comment to a post

``PUT /posts/:id/update`` =       Update a post

``DELETE /posts/:id`` =           Delete a post