# Copyright (c) 2015 The Virtual Vulcano authors. All rights reserved.
# Use of this source code is governed by a BSD-style license that
# can be found in the LICENSE.md file.

FROM debian:wheezy
MAINTAINER Virtual Vulcano <virtualvulcano@gmail.com>

RUN apt-get update -y
RUN DEBIAN_FRONTED=noninteractive apt-get install -y proftpd

ADD provision/proftpd.conf /etc/proftpd/proftpd.conf
RUN chown root:root /etc/proftpd/proftpd.conf

CMD /usr/sbin/proftpd --nodaemon
