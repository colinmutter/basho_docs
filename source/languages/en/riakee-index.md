---
title: Riak Enterprise
project: riakee
version: 0.10.0+
document: tutorial
toc: true
index: true
audience: beginner
keywords: []
simple: true
versions: false
---

<div class="note">
<div class="title">Riak Enterprise only</div>
This documentation applies only to Riak Enterprise, Basho's commercial
extension to <a href="http://docs.basho.com/riak/latest/">Riak</a>. If
you'd like to talk to us about using Riak Enterprise, please <a
href="http://info.basho.com/Wiki_Contact.html" target="_blank">let us
know</a>
</div>

Riak Enterprise is a commercially distributed product built on Riak
(Apache 2.0-licensed) that extends Riak's capabilities with
[[Multi-Datacenter Replication|Multi Data Center Replication:
Architecture]], [[SNMP monitoring|SNMP Configuration]],
[[JMX-Monitoring]], and 24x7 support.

When Multi-Datacenter Replication is enabled, one cluster acts as a
**source cluster**. The source cluster replicates its data to one or
more **sink clusters** through a [[full or realtime sync|Multi Data
Center Replication: Architecture]] process. Data transfer is
unidirectional by default (source &rarr; sink). Bidirectional
synchronization can be achieved, however, by configuring a pair of
connections _between_ clusters.

Multi-Datacenter features can serve a variety of purposes, including but
not limited to the following:

* data locality
* disaster recovery
* global load balancing
* active backups
* secondary analytics clusters
* meeting regulatory requirements
