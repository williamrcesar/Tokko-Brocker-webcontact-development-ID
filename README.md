# Tokko-Brocker-webcontact-development-ID
Simply add the parameter "developments" to your POST body – even if it's not in the official docs, it works!
```
curl -X POST "https://www.tokkobroker.com/api/v1/webcontact/?key=YOUR_API_KEY" \
  -H "Content-Type: application/json" \
  -d '{
    "name": "John Doe",
    "cellphone": "1234567890",
    "phone": "",
    "email": "john@example.com",
    "work_name": "Doe Investments",
    "text": "I\'m interested in your projects.",
    "properties": "",
    "tags": "[\"Type: Investor\", \"Luxury\"]",
    "agent_mail": "agent@tokko.com",
    "developments": "12345"
}'
```


## ENGLISH

Despite the official Tokko Broker documentation not mentioning it, you can include the "development ID" using the field `developments` in your request body.

**Fields to include in a POST to /webcontact:**  
(The request body must be a JSON object with the following parameters. At least one contact information field must be filled: `phone`, `email`, or `cellphone`.)

| Parameter     | Type   | Description                                                    |
|---------------|--------|----------------------------------------------------------------|
| name          | string | Name of the contact                                            |
| cellphone     | string | Cellphone of the contact                                       |
| phone         | string | Phone of the contact                                           |
| email         | string | E-mail of the contact                                          |
| work_name     | string | Name of the business of the contact                            |
| text          | string | Text of the form                                               |
| properties    | string | List of property IDs related to this contact form (e.g. "[1]") |
| tags          | string | List of tags related to this contact form (e.g. "["AdSense","Investor"]") |
| agent_mail    | string | Email of the user who will receive the lead                    |
| developments  | string | Development/enterprise ID :warning: _(undocumented, but functional)_ |



**JSON example:**
```
{
"name": "John Doe",
"cellphone": "1234567890",
"phone": "",
"email": "john@example.com",
"work_name": "Doe Investments",
"text": "I'm interested in your projects.",
"properties": "",
"tags": "["Type: Investor ", "Luxury"]",
"agent_mail": "agent@tokko.com",
"developments": "12345"
}
```
[Official documentation](https://developers.tokkobroker.com/docs/contact)
[Official playground](https://www.tokkobroker.com/api/playground#!/web_contact/web-contact_post_0)

***

## ESPAÑOL

Aunque la documentación oficial de Tokko Broker no lo mencione, puedes incluir el "ID del desarrollo" usando el campo `developments` en el cuerpo del request.

**Campos permitidos para el POST a /webcontact:**  
(El cuerpo debe ser un objeto JSON con los siguientes parámetros. Al menos uno entre `phone`, `email` o `cellphone` debe estar presente.)

| Parámetro     | Tipo   | Descripción                                                    |
|---------------|--------|----------------------------------------------------------------|
| name          | string | Nombre del contacto                                            |
| cellphone     | string | Celular del contacto                                           |
| phone         | string | Teléfono del contacto                                          |
| email         | string | Email del contacto                                             |
| work_name     | string | Nombre del negocio del contacto                                |
| text          | string | Texto del formulario                                           |
| properties    | string | Lista de ID de propiedades relacionadas (ej: "[1]")      |
| tags          | string | Lista de tags de este contacto (ej: "["AdSense","Investor"]")  |
| agent_mail    | string | Email del usuario que recibirá el lead                         |
| developments  | string | ID de desarrollo   :warning: _(no documentado, pero funciona)_ |


**Ejemplo JSON:**
```json
{
"name": "John Doe",
"cellphone": "1234567890",
"phone": "",
"email": "john@example.com",
"work_name": "Doe Investments",
"text": "I'm interested in your projects.",
"properties": "",
"tags": "["Type: Investor ", "Luxury"]",
"agent_mail": "agent@tokko.com",
"developments": "12345"
}
```
[Documentación oficial](https://developers.tokkobroker.com/docs/contact)
[Official playground](https://www.tokkobroker.com/api/playground#!/web_contact/web-contact_post_0)
***

## PORTUGUÊS

Apesar de a documentação oficial do Tokko Broker não citar, você pode incluir o “ID do empreendimento” usando o campo `developments` no corpo da requisição.

**Campos aceitos para POST em /webcontact:**  
(O corpo da requisição deve ser um objeto JSON com os seguintes parâmetros. Pelo menos um entre `phone`, `email` ou `cellphone` deve ser informado.)

| Parâmetro     | Tipo   | Descrição                                                     |
|---------------|--------|----------------------------------------------------------------|
| name          | string | Nome do contato                                               |
| cellphone     | string | Celular do contato                                            |
| phone         | string | Telefone do contato                                           |
| email         | string | E-mail do contato                                             |
| work_name     | string | Nome da empresa/negócio do contato                            |
| text          | string | Texto da mensagem                                             |
| properties    | string | Lista de IDs de propriedades relacionadas (ex: "[1]")  |
| tags          | string | Lista de tags referentes ao contato (ex: "["AdSense","Investidor"]") |
| agent_mail    | string | E-mail do usuário que receberá o lead                           |
| developments  | string | ID do empreendimento :warning: _(não documentado, mas funcional)_ |

**Exemplo de JSON:**
```json
{
"name": "John Doe",
"cellphone": "1234567890",
"phone": "",
"email": "john@example.com",
"work_name": "Doe Investments",
"text": "I'm interested in your projects.",
"properties": "",
"tags": "["Type: Investor", "Luxury"]",
"agent_mail": "agent@tokko.com",
"developments": "12345"
}
```
[Documentação oficial](https://developers.tokkobroker.com/docs/contact)
[Official playground](https://www.tokkobroker.com/api/playground#!/web_contact/web-contact_post_0)

***

Se desejar adaptar para markdown puro, exemplos mínimos, ou outra formatação, só avisar!

[1](https://developers.tokkobroker.com/docs/developments)
