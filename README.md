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