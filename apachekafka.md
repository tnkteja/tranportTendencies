[Download](http://kafka.apache.org/downloads) and `/path/to/gradle jarAll`, with [gradle](https://gradle.org/releases)


## Remember the classic Producer Consumer Problem on a limited shared buffer.

![](http://i0.wp.com/www.eexploria.com/wp-content/uploads/2012/03/Producer-Consumer-problem.png)

The producer cannot write on the until it is consumed to leave some space to write. A consumer cannot read until the producer writes something to read.

![](https://kafka.apache.org/0102/images/log_anatomy.png)

With kafka a use and through buffer with an expiry time, called immutable partition is written by producers and consumed by consumers.
```
Not Sure Why:
============
* number of pertions must be equal to number of consumers in a consumer group for kafka.

```
## References
1. _https://www.quora.com/What-is-the-actual-role-of-ZooKeeper-in-Kafka_
2. _https://sookocheff.com/post/kafka/kafka-in-a-nutshell/_
3. _https://www.confluent.io/blog/how-to-choose-the-number-of-topicspartitions-in-a-kafka-cluster/_
4. _https://www.safaribooksonline.com/library/view/kafka-the-definitive/9781491936153/ch04.html_
