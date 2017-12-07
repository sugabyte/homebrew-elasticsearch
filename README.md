## homebrew-elasticsearch

This repository is for installing old Elasticsearch versions on Mac since Homebrew removes unmaintained versions while SugarCRM still needs them. Elasticsearch on Mac can be used with SugarCRM instances hosted on the Mac or remote instances can be pointed to it.

The original brew formula can be found in this commit: https://github.com/Homebrew/homebrew-core/blob/2c2d329c132dd0c67ccedbeeb2337a3ed0807a56/Formula/elasticsearch%401.7.rb

### Install, start up, configure and check that it is working:

```
brew install sugabyte/homebrew-elasticsearch/elasticsearch@1.7
nano /usr/local/opt/elasticsearch\@1.7/config//elasticsearch.yml
brew services start sugabyte/elasticsearch/elasticsearch@1.7
curl -X GET 'http://localhost:9200'
```

### Stop the Elasticsearch service and remove it:

```
brew services stop sugabyte/elasticsearch/elasticsearch@1.7
brew remove sugabyte/homebrew-elasticsearch/elasticsearch@1.7
```
