# docker-prerender
Dockerized prerender.io (for AngularJS SEO, BackboneJS SEO, or EmberJS SEO) with file-caching enabled

# usage
```bash
git clone https://github.com/daweedm/docker-prerender.git && cd docker-prerender && docker-compose up -d
```

# configuration
You can customize the cache TTL in the `docker-compose.yml` file (default to 10000 seconds).
