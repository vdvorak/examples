The origin cluster in this case is a |ccloud| cluster, and |crep| admin client needs to know how to connect to this origin cluster, which can be configured by using the prefix ``src.kafka.`` for these connection configuration parameters.

.. sourcecode:: bash

   src.kafka.bootstrap.servers=<bootstrap-servers-destination>
   src.kafka.ssl.endpoint.identification.algorithm=https
   src.kafka.security.protocol=SASL_SSL
   src.kafka.sasl.mechanism=PLAIN
   src.kafka.sasl.jaas.config=org.apache.kafka.common.security.plain.PlainLoginModule required username="<api-key-destination>" password="<api-secret-destination>";

