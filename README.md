# django-rabbitmq-celery
Code example to communicate two different Django Projects through RabbitMq as Broker and Celery as Task Runner

Default User for rabbitmq server is django and also the password.
The Rabbitmq vhost is rabbit
By default user django has the "management" role.

If you want change this, you need to enter to the rabbitmq-server container to bash command line and write:

rabbitmqctl add_user user_you_want user_password<br>
rabbitmqctl add_vhost v_host_name_you_want<br>
rabbitmqctl set_permissions -p v_host_name_you_want user_you_want ".*" ".*" ".*"<br>
rabbitmqctl set_user_tags user_you_want management<br>
<br>

To run the project and launch all containers type:<br><br>

<b>docker-compose up</b>
