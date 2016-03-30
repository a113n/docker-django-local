FROM 4113n/base
MAINTAINER Allen Yu "mail@allenyu.info"

RUN apt-get update && apt-get install -qq -y rabbitmq-server
RUN /usr/sbin/rabbitmq-plugins enable rabbitmq_management
RUN rabbitmqctl add_user admin admin
RUN rabbitmqctl set_user_tags admin administrator
RUN service rabbitmq-server start

EXPOSE 5672 15672 4369
