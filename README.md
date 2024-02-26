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

 <div align="center">
<img src="https://github.com/lucasmargui/Python_Vendas_Notificacao_Sms/assets/157809964/348e4054-d246-4cd7-a5e6-a2c805e8bbcc" style="width:100%">
</div>







 ### From

 Utilização de um numero comprado que será responsável para enviar o SMS para o destinatário
```
  message = client.messages.create(
            to="+55xxxxxxxxxxxxxxx",
            from_="xxxxxxxxxxxxxxxx",
            body=f'No mês {mes} alguém bateu a meta. Vendedor: {vendedor}, Vendas: {vendas}')
```

 <div align="center">
<img src="https://github.com/lucasmargui/Python_Vendas_Notificacao_Sms/assets/157809964/6bfc113f-e0d7-4b5f-a6ca-3e6be255249f" style="width:100%">
</div>

