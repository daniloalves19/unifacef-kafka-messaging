# unifacef-kafka-messaging
Projeto da Pós da Unifacef em desenvolvimento web para a disciplina de Mensageria/Streams


1. Entre na pasta do projeto e inicie no terminal o Kafka
```
docker-compose up -d
```

2. Inicie o projeto pelo comando abaixo
```
./mvnw spring-boot:run
```

3. utilize o Postman ou outro programa do gênero e realize uma requisição do tipo POST na url
```
localhost:8080/v1/orders
```

4. Envie no body da requisição
```
{
    "orderId":"45854",
    "paymentType":"Cartão",
    "value":800
}
```

5. Verifique no terminal o consumo desta requisição
```
Order: Order(orderId=45854, paymentType=Cartão, value=800)
```