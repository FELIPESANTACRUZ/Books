# My Books 
 API em Graphql de livros 

/* npm run dev */
http://localhost:4000/

__________________________________________________

mutation{
  create(id: "a",title: "Harry Potter", author: "JK", publishedAt: 1999){
    title
  }
}
__________________________________________________

query{
  books {
    id
    title
  }
}
__________________________________________________
query{
  book(id: "b") {
    title
  }
}
__________________________________________________
mutation($deleteId: ID!) {
  delete(id: "a")
}
__________________________________________________
mutation {
  update(id: "b" ,publishedAt: 2014) {
    title
    publishedAt
  }
}
