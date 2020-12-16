Application Containerization and Microservice Orchestration

In this tutorial we will learn about basic application containerization using Docker and running various components of an application as microservices. We will utilize Docker Compose for orchestration during the development. This tutorial is targeted for beginners who have the basic familiarity with Docker. If you are new to Docker, we recommend you check out Docker for Beginners tutorial first.

We will start from a basic Python script that scrapes links from a given web page and gradually evolve it into a multi-service application stack. The demo code is available in the Link Extractor repo. The code is organized in steps that incrementally introduce changes and new concepts. After completion, the application stack will contain the following microservices:

A web application written in PHP and served using Apache that takes a URL as the input and summarizes extracted links from it
The web application talks to an API server written in Python (and Ruby) that takes care of the link extraction and returns a JSON response
A Redis cache that is used by the API server to avoid repeated fetch and link extraction for pages that are already scraped
