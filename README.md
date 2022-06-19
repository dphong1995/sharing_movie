<div align="center">
  <h3 align="center">Shorten URL</h3>

  <p align="center">
    <br />
    <a href="https://shorten-url-mono.vercel.app/">View Demo</a>
    ·
    <a href="https://dphong1995/shorten_url_mono/issues">Report Bug</a>
  </p>
</div>

<!-- GETTING STARTED -->
## Getting Started

To get a local copy up and running follow these simple example steps.

### Prerequisites

* Docker - an open platform for developing, shipping, and running applications.
    * https://docs.docker.com/engine/install/

### Start server

1. Clone the repo
   ```sh
   git clone https://github.com/dphong1995/shorten_url_mono.git
   ```
2. Start containers
   ```sh
   docker-compose up
   ```

### Run Test
1. Start containers
   ```sh
   docker-compose up
   ```
2. Prepare test db
   ```sh
   docker-compose exec be rails db:reset db:prepare RAILS_ENV=test
   ```
3. Run test
    ```sh
    docker-compose exec be rails test
    ```

### Scalability
* Use service cluster (k8s, ecs) and load balancer to deploy the container.
* Use database cluster.
* Use redis for caching.
