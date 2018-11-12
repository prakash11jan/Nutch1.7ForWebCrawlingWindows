Steps to follow
1. install cygwin for windows to mock linux environment (https://www.cygwin.com/)
2. download my project
3. copy into cygwin home directory (eg: C:\cygwin64\home)
4.install apache solr 6.5.1
5. create a solr core called "nutch"
6. copy the schema-solr4.xml content from {NUTCH_HOME}/conf directory to solr managed-schema file (C:\cygwin64\home\solr\solr-6.5.1\server\solr\nutch\conf)
7. open cygwin as adminstartor
8. take a look at seed.txt file (C:\cygwin64\home\nutch1.7\apache-nutch-1.7\urls\seed.txt)
9. change the URL which want to crawl
10.start the solr server
11.in cygwin navigate to {NUTCH_HOME} directory and 
12. execute ./bin/crawl urls/ testCrawl/ http://127.0.0.1:8983/solr/yourcore 1
    eg : ./bin/crawl urls/ testCrawl/ http://127.0.0.1:8983/solr/nutch 1
    
13. once it done. hit solr url: http://127.0.0.1:8983/solr and check.

14. the crwled output should be indexed

