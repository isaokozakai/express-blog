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
  }],
  "like": number      //for vote
}]
```
# Routing

``GET "/"`` =                     Top Page

``GET /posts/form`` =             Form Page for a new post

``POST /posts`` =                 Create a new post

``GET /posts/:id`` =              Read Page

``GET /posts/:id/form`` =         Form Page for an existing post

``POST /posts/:id/comments`` =      Leave a comment to a post

``PUT /posts/:id/vote?rating=0`` =  Upvote or downvote a post. rating = 0 means a downvote a post and rating = 1 means upvote a post.

``PUT /posts/:id/update`` =       Update a post

``DELETE /posts/:id`` =           Delete a post

``DELETE /posts`` =               Delete ALL posts(maybe add an 'are you sure?' message :D)

``GET /search?name=Blogname`` =     Search for a specific post by name. Will redirect to GET "/posts/:id" if manages to find a post or back to the same page if it didn't find a post
