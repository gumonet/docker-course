# Despliega un servidor apache con PHP y agrega un certificado SSL

`$ docker build -t apache:bootstrap . `
`$ docker run -d -p 80:80`

## Crear certificado SSL
`openssl req -x509 -nodes -days 365 -newkey rsa:2048 -keyout docker.key -out docker.crt` 
Add common name: localhost