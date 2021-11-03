# Future-Academy

Olá!

  

O intuito deste repositório é armazenar e receber as contribuições de usuários da Future Academy.

  

No momento, aceitamos contribuições de novos assuntos e diálogos que o nosso chatbot ainda não saiba!

  

## Como contribuir:

O usuário deve dar um pull request na pasta novosDialogos.


São necessários 2 arquivos:

1. Arquivo JSON com o novo #Intent e suas amostras de perguntas do usuário (No mínimo 10, escritas das mais diversa formas). Por favor, seguir exatamente o padrão abaixo.

EX:

cloudIntent.json
```json

{
"examples": [
{"text": "o que é cloud"},
{"text": "O que é cloud?"},
{"text": "você sabe o que é cloud?"},
{"text": "eu queria saber o que é cloud computing"},
{"text": "voce sabe sobre cloud computing"},
{"text": "me fale um pouco sobre cloud computing"}
]
}
```


2. Arquivo JSON com o novo #Dialog e as falas. Atente-se que ao criar o diálogo na plataforma do Watson Assistant, é possível copiá-lo em formato JSON. Por favor, seguir exatamente o padrão abaixo.
	
EX:

cloudDialog.json

```json


{
  "output": {
    "generic": [
      {
        "values": [
          {
            "text": "Cloud é computação em nuvem"
          },
          {
            "text": "Quando utilizamos sites como Google Drive, estamos utilizando um armazenamento que não é nosso, isso é computação em nuvem"
          },
          {
            "text": "A IBM oferece diversos serviços em nuvem gratuitos"
          }
        ],
        "response_type": "text",
        "selection_policy": "sequential"
      }
    ]
  }
}


```