# SSH

##SSL Creation

Generate CA key:

		openssl genrsa -out ca.key 2048

Generate CA certificate:

		openssl req -x509 -new -nodes -key ca.key -sha256 -days 1825 -out ca.crt

Create CSR for domain:

		openssl req -newkey rsa:2048 -nodes -keyout domain.key -out domain.csr

Create certificate for domain using CA certificate:

		openssl x509 -req -in domain.csr -CA ca.crt -CAkey ca.key -CAcreateserial -out domain.crt -days 365
