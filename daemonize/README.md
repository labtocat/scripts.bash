Daemonize scripts for Mac
===========================

Tired of having 4 terminal tabs open to keep the servers
for your project running? Well I was.

This script lets you set up, run and stop scripts (which will be run as daemons).

Usage
------

**Running previously setup daemons:**

<pre>
./daemonize redis,elastic,rabbitmq,mongo
</pre>

**Output:**

<pre>
(✓) redis is running
(✓) elastic is running
(✓) rabbitmq is running
(✓) mongo is running

(Ctrl+C) to Interrupt

[^C]
(✖) redis was stopped
(✖) elastic was stopped
(✖) rabbitmq was stopped
(✖) mongo was stopped
</pre>


**Setting up new daemons:**

<pre>
./daemonize elastic
</pre>

**Output:**

<pre>
[elastic] Command with Full Path (Eg. /usr/bin/elastic /usr/share/elastic.conf): /opt/elasticsearch/bin/elasticsearch
(✓) elastic is running

(Ctrl+C) to Interrupt

[^C]
(✖) elastic was stopped
</pre>