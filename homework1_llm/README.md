## Steps

1. Create virtual environment
```shell
poetry shell
```
2. Install Dependencies
```shell
poetry install
```
3. Authenticate Openai
```shell
export OPENAI_API_KEY="xxx"
```

4.  open jupyter notebook
5.  **Run Elasticsearch in Docker (user: elastic):**

```bash
docker run -it --rm --name elasticsearch -p 9200:9200 -p 9300:9300 -e "discovery.type=single-node" -e "xpack.security.enabled=false" docker.elastic.co/elasticsearch/elasticsearch:8.4.3
