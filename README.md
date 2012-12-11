# chef-expander

* Documentation: http://docs.opscode.com/
* Tickets/Issues: http://tickets.opscode.com
* IRC: [#chef](irc://irc.freenode.net/chef) and [#chef-hacking](irc://irc.freenode.net/chef-hacking) on Freenode
* Mailing list: http://lists.opscode.com

## Overview ##

Chef Expander replaces the `chef-solr-indexer` daemon that was included with Chef 0.8 and
0.9.

### Dependencies ###

* bunny
* yajl
* eventmachine
* em-http-request
* amqp
* highline

### Monitoring With Nagios ###

A Nagios plugin to monitor queue backlog is included in scripts/ directory as
`check_queue_size`.

To run it with the warning threshold at 250 messages and critical at 500 messages:

```
check_queue_size -w 250 -c 500
```


## Contributing/Development

Before working on the code, if you plan to contribute your changes, you need to
read the
[Opscode Contributing document](http://wiki.opscode.com/display/chef/How+to+Contribute).

You will also need to set up the repository with the appropriate branches. We
document the process on the
[Working with Git](http://wiki.opscode.com/display/chef/Working+with+git) page
of the Chef wiki.

## Reporting Bugs ##

You can search for known issues in
[Opscode Chef's bug tracker][jira]. Tickets should be filed under the
**CHEF** project with the component set to **"Chef Server"**.

[jira]: http://tickets.opscode.com/browse/CHEF

## License ##

|                      |                                          |
|:---------------------|:-----------------------------------------|
| **Copyright:**       | Copyright (c) 2011-2012 Opscode, Inc.
| **License:**         | Apache License, Version 2.0

Licensed under the Apache License, Version 2.0 (the "License");
you may not use this file except in compliance with the License.
You may obtain a copy of the License at

    http://www.apache.org/licenses/LICENSE-2.0

Unless required by applicable law or agreed to in writing, software
distributed under the License is distributed on an "AS IS" BASIS,
WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
See the License for the specific language governing permissions and
limitations under the License.
