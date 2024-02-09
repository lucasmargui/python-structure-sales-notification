<H1 align="center">Vendas Notificação</H1>
<p align="center">🚀 Projeto de criação de uma estrutura de notificação via sms para referências futuras</p>

## Recursos Utilizados

* Pandas
* Twilio
* Python 3.10

 ## Twilio
  Utilização das credencias para conexão com API

```
account_sid = "xxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxx"
auth_token  = "xxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxx"
client = Client(account_sid, auth_token)
```
 <img src="https://cdn.discordapp.com/attachments/1046824853015113789/1205394190901444638/image.png?ex=65d835d2&is=65c5c0d2&hm=1a0756d8324218c7f1d478e1053b537c8de8b50e43a8e18a31922180c0c4edcc&" alt="">

 


 ### From

 Utilização de um numero comprado que será responsável para enviar o SMS para o destinatário
```
  message = client.messages.create(
            to="+55xxxxxxxxxxxxxxx",
            from_="xxxxxxxxxxxxxxxx",
            body=f'No mês {mes} alguém bateu a meta. Vendedor: {vendedor}, Vendas: {vendas}')
```

 <img src="https://cdn.discordapp.com/attachments/1046824853015113789/1205394519143485480/image.png?ex=65d83620&is=65c5c120&hm=20fb5dda46c77cd53791b64ef24cf583d9fa098c35aa77124fcbc8b6fa3d4afb&" alt="">   
