This repository is for installing Elasticsearch 1.7 on Mac since Homebrew removes unmaintained versions. Elasticsearch on Mac can be used with SugarCRM instances hosted on the Mac or remote instances can be pointed to it.

```
brew install sugabyte/homebrew-elasticsearch-17/elasticsearch@1.7
nano /usr/local/opt/elasticsearch\@1.7/config//elasticsearch.yml
brew services start sugabyte/elasticsearch-17/elasticsearch@1.7
curl -X GET 'http://localhost:9200'
```
