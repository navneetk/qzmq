
Title: demo/installation
Date: 20121019

<A name="toc1-5" title="Contents" />
# Contents


**<a href="#toc1-10">Installing ZeroMQ Language Bindings</a>**
&emsp;<a href="#toc2-15">Instaling Language Bindings</a>
&emsp;<a href="#toc2-19">Q</a>
&emsp;<a href="#toc2-23">Python</a>
&emsp;<a href="#toc2-40">Perl</a>
&emsp;<a href="#toc2-57">Java</a>

<A name="toc1-10" title="Installing ZeroMQ Language Bindings" />
# Installing ZeroMQ Language Bindings

ZeroMQ is written in C but there are many bindings for other  [languages][languages]. Before running demos, install ZeroMQ and the necessary language bindings.

<A name="toc2-15" title="Instaling Language Bindings" />
## Instaling Language Bindings
ZeroMQ must be installed prior to installing language bindings. See [`how-to-install-zeromq-czmq.md`](../how-to-install-zeromq-czmq.md) for installation instructions.

<A name="toc2-19" title="Q" />
## Q
See [qzmq][qzmq].

<A name="toc2-23" title="Python" />
## Python
Install [pyzmq][pyzmq]:

    sudo easy_install pyzmq

One quick check for successful installation:

    $ python
    >>> import zmq
    >>> help(zmq) # to read the documentation
    >>> zmq.pyzmq_version()
    '2.2.0'
    >>> zmq.zmq_version()
    '2.2.0'
    # either '2.2.0' or '2.2.0.1' is acceptable.

<A name="toc2-40" title="Perl" />
## Perl
Install [ZeroMQ.pm][perl] from CPAN:

    sudo cpan -i ZeroMQ # add -f flag if necessary

One quick check for successful installation:

    $ perl -e 'use ZeroMQ qw/:all/; print "ZeroMQ version is: " . ZeroMQ::version() . "\n";'
    ZeroMQ version is: 2.2.0

Perl demo scripts also need additional modules that can be installed by:

    sudo cpan -i Digest::SHA1
    sudo cpan -i Module::Build
    sudo cpan -i String::Random
    
<A name="toc2-57" title="Java" />
## Java
Currently the demo does not include any Java code.

See [http://www.zeromq.org/bindings:java](http://www.zeromq.org/bindings:java) for installation instructions and documentation of Java bindings.


[qzmq]: https://github.com/jaeheum/qzmq
[issues]: https://github.com/jaeheum/qzmq/issues
[zeromq]: http://www.zeromq.org
[czmq]: http://czmq.zeromq.org
[q]: http://kx.com
[zguide]: http://zguide.zeromq.org
[gitdown]: https://github.com/imatix/gitdown
[broker]: http://zguide.zeromq.org/page:all#A-Request-Reply-Broker
[brokerless]: http://www.zeromq.org/whitepapers:brokerless
[mitm]: http://en.wikipedia.org/wiki/MiTM
[perl]: http://www.zeromq.org/bindings:perl
[pyzmq]: http://www.zeromq.org/bindings:python
[languages]: http://www.zeromq.org/bindings:_start
[gangnam]: http://www.youtube.com/watch?v=9bZkp7q19f0&feature=related
[homebrew]: http://mxcl.github.com/homebrew/
[issue6]: https://github.com/jaeheum/qzmq/issues/6
[yum]: https://access.redhat.com/knowledge/docs/en-US/Red_Hat_Enterprise_Linux/6/html/Deployment_Guide/sec-Managing_Yum_Repositories.html
