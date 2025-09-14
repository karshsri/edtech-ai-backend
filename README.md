
Component	                          Purpose
.NET Core Web API                  	Backend framework for building scalable RESTful services
OpenAI Embeddings API              	Converts text into high-dimensional vectors for semantic comparison
Qdrant Vector DB	                  Stores and searches embeddings using cosine similarity
Postman	                            Used to test and validate API endpoints
Docker Desktop	                    Intended to run Qdrant locally in a containerized environment
Controllers: Handle HTTP requests (EmbeddingController)

Services: Generate embeddings via OpenAI (EmbeddingService)

Qdrant Client: Store and search vectors (QdrantClient)

Models: Define request and response formats (EmbedRequest, SearchRequest, SearchResult)

Program.cs: Configures dependency injection and middleware

Error and handelling : 
docker: error during connect...	Docker Desktop not running or misconfigured	Installed Docker Desktop, enabled WSL 2, restarted service
Failed to determine the https port for redirect	HTTPS redirection middleware active without HTTPS config	Disabled UseHttpsRedirection() in Program.cs for local testing
