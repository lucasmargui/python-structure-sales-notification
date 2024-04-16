<H1 align="center">Sales Notification</H1>
<p align="center">🚀 Project to create a notification structure via SMS for future references</p>

## Resources Used

* Pandas
* Twilio
* Python 3.10

 ## Twilio
 Using credentials to connect to API

```
account_sid = "xxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxx"
auth_token = "xxxxxxxxxxxxxxxxxxxxxxxxxxxxxxx"
client = Client(account_sid, auth_token)
```

 <div align="center">
<img src="https://github.com/lucasmargui/Python_Vendas_Notificacao_Sms/assets/157809964/348e4054-d246-4cd7-a5e6-a2c805e8bbcc" style="width:100%">
</div>


 ### From

 Using a purchased number that will be responsible for sending the SMS to the recipient
```
 message = client.messages.create(
 to="+55xxxxxxxxxxxxxxx",
 from_="xxxxxxxxxxxxxxx",
 body=f'In the month {mes} someone reached the goal. Seller: {seller}, Sales: {sales}')
```

 <div align="center">
<img src="https://github.com/lucasmargui/Python_Vendas_Notificacao_Sms/assets/157809964/6bfc113f-e0d7-4b5f-a6ca-3e6be255249f" style="width:100%">
</div>
