.. image:: https://badge.waffle.io/erlio/vernemq.png?label=ready&title=Ready 
 :target: https://waffle.io/erlio/vernemq
 :alt: 'Stories in Ready'
VerneMQ: A Distributed MQTT Broker
==================================

VerneMQ is an Apache2 licensed distributed `MQTT <http://www.mqtt.org>`_ broker, developed in `Erlang <http://www.erlang.org>`_.

MQTT used to stand for MQ Telemetry Transport, but it no longer is an acronym. It is an extremely simple and lightweight publish/subscribe messaging protocol, that was invented at IBM and Arcom (now Eurotech) to connect restricted devices in low bandwidth, high-latency or unreliable networks.

VerneMQ implements the MQTT 3.1 and 3.1.1 specifications, integration of MQTT-SN is planned. Currently the following features are implemented:

* QoS 0, QoS 1, QoS 2
* Basic Authentication and Authorization
* Bridge Support
* $SYS Tree for monitoring and reporting
* TLS (SSL) Encryption
* Dynamic Topics
* Websockets Support
* Cluster Support
* SNMP Monitoring
* Logging (Console, Files, Syslog)
* Reporting to Graphite
* Extensible Plugin architecture
* Multiple Sessions per ClientId
* Session Balancing
* Message load regulation
* Message load shedding (for system protection)
* Offline Message Storage (based on LevelDB)
* Queue can handle messages FIFO or LIFO style.

Where to find more
------------------

Below you'll find a basic introduction to building and starting VerneMQ. For more
information about the binary package installation, configuration, and administration 
of VerneMQ, please visit our documentation at `VerneMQ Documentation <http://verne.mq/docs>`_ 
or checkout the product page `VerneMQ <http://verne.mq>`_ if you require more
information on the available support options.

Quick Start
-----------

This section assumes that you have a copy of the VerneMQ source tree. To get
started, you need to first build VerneMQ.

Building VerneMQ
~~~~~~~~~~~~~~~~

Note: VerneMQ requires Erlang 17.x to be installed on your system. Erlang 18 is
currently not supported.

Assuming you have a working Erlang installation, building VerneMQ should be as
simple as:

.. code-block:: ini

    $ cd $VERNEMQ
    $ make rel

Starting VerneMQ
~~~~~~~~~~~~~~~~

Once you've successfully built VerneMQ, you can start the server with the following
commands:

.. code-block:: ini

    $ cd $VERNEMQ/_build/default/rel/vernemq
    $ bin/vernemq start

Note that the ``$VERNEMQ/_build/default/rel/vernemq`` directory is a complete, 
self-contained instance of VerneMQ and Erlang. It is strongly suggested that you
move this directory outside the source tree if you plan to run a production 
instance.

Important links
~~~~~~~~~~~~~~~~

* \#vernemq on freenode IRC
* `VerneMQ User Mailing List <http://verne.mq/mailman/listinfo/vernemq-list_verne.mq>`_ 
* `VerneMQ Documentation <http://verne.mq/docs>`_ 
* `Follow us on Twitter (@vernemq)! <https://twitter.com/vernemq>`_ 

