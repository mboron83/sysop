ansible-playbook site.yml -i hosts.yml -l my_worker -t docker_container --extra-vars "state=absent"

ansible-playbook site.yml -i hosts.yml -l my_worker -t docker_container -e cron=indeksy -e absent=1

docker-compose exec php php /var/www/symfony/bin/console cache:clear --env=prod
