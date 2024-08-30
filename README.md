Build

```docker-compose up -d```

Open

```http://localhost:5601```

Enrollment token

```docker exec -it elasticsearch /usr/share/elasticsearch/bin/elasticsearch-create-enrollment-token -s kibana```

Verification code

```docker exec -it kibana /usr/share/kibana/bin/kibana-verification-code```

Change password for user **elastic**

```docker exec -it elasticsearch /usr/share/elasticsearch/bin/elasticsearch-reset-password -u elastic```

Templates

- Перейдите в раздел Stack Management (Управление стеком) в левом меню.
- Выберите Index Management (Управление индексами) и затем Index Templates (Шаблоны индексов).
- Создайте новый шаблон для индекса ros2-errors-*, который будет соответствовать структуре данных, отправляемых из ROS 2.