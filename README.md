# What is this? 

This is a server to add a comment to [kafka](https://github.com/Step-henC/flashycards-backend) -> [flashycards ui](https://github.com/Step-henC/flashycards-ui/tree/master). 
This server is for those that do not want to cURL comments to kafka cli. 

To use this server, start up `go run server.go` and open GraphQL playground at `localhost:8090`

Create a comment in the following format:

`mutation CreateComment($input: CommentInput!) {
  createComment(input: { id: "random string", userId: "any name", comment: "anything"}){
    id
    userId
    string
  }
}`
