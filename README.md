logstash-modsecurity
====================


 Example Modsecurity audit log ingestor
 configuration for Logstash

 author bitsofinfo.g[at]gmail.com
 
 built/tested w logstash v1.2.1 

 @see http://logstash.net/
 @see https://github.com/SpiderLabs/ModSecurity/wiki/ModSecurity-2-Data-Formats
 @see https://bitsofinfo.wordpress.com

 @license http://www.apache.org/licenses/LICENSE-2.0 

 @notes NOTE: this is not perfect and I am no Ruby expert
        however this worked when processing quite a bit of
        high volume mod-sec logs with lots of different
        variations in what A-K sections were and were not
        present. At a minimum its a good starting point
        to start tackling a complex log format.

 Be careful w/ the custom ruby filter blocks and be aware
 of https://logstash.jira.com/browse/LOGSTASH-1375

 This config file for whatever reason will not run
 if you try to add the "-- web" option onto the logstash
 flat jar. This has been reported to the developers. 
 Recommend you run this without the "-- web" option and just
 hook up Kibana separately.



