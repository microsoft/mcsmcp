swagger: "2.0"
info:
  title: Jokes MCP Server
  description: Get jokes using MCP server. For instance Chuck Norris jokes, Dad jokes and Yo Mama jokes.
  version: "1.0"
host: dummyurl.azurewebsites.net
basePath: /
schemes:
  - https
definitions:
  QueryResponse:
    type: object
    properties:
      jsonrpc:
        type: string
      id:
        type: string
      method:
        type: string
      params:
        type: object
      result:
        type: object
      error:
        type: object
paths:
  /sse:
    get:
      summary: Jokes MCP Server
      parameters:
        - in: query
          name: sessionId
          type: string
          required: false
      produces:
        - application/json
      responses:
        "200":
          description: Immediate Response
          schema:
            $ref: "#/definitions/QueryResponse"
        "201":
          description: Created and will follow callback
      operationId: JokesMCP
      tags:
        - Agentic
        - McpSse
securityDefinitions: {}
security: []
