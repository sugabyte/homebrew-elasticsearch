```
brew install sugabyte/homebrew-elasticsearch-17/elasticsearch@1.7
nano /usr/local/opt/elasticsearch\@1.7/config//elasticsearch.yml
brew services start sugabyte/elasticsearch-17/elasticsearch@1.7
curl -X GET 'http://localhost:9200'
```
