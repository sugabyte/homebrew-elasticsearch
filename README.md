## homebrew-elasticsearch17

This repository is for installing Elasticsearch 1.7 on Mac since Homebrew removes unmaintained versions. Elasticsearch on Mac can be used with SugarCRM instances hosted on the Mac or remote instances can be pointed to it.

The original brew formula can be found in this commit: https://github.com/Homebrew/homebrew-core/blob/2c2d329c132dd0c67ccedbeeb2337a3ed0807a56/Formula/elasticsearch%401.7.rb

### Install, start up, configure and check that it is working

```
brew install sugabyte/homebrew-elasticsearch-17/elasticsearch@1.7
nano /usr/local/opt/elasticsearch\@1.7/config//elasticsearch.yml
brew services start sugabyte/elasticsearch-17/elasticsearch@1.7
curl -X GET 'http://localhost:9200'
```

### Stop the Elasticsearch 1.7 service and remove it

```
brew services stop sugabyte/elasticsearch-17/elasticsearch@1.7
brew remove sugabyte/homebrew-elasticsearch-17/elasticsearch@1.7
```
