<h1 align="center">
    <img alt="Rocketseat" title="Rocketseat" src=".github/rocketseat.png" width="60px" />
</h1>

<p align="center">
  <a href="#rocket-tecnologias">Tecnologias</a>&nbsp;&nbsp;&nbsp;|&nbsp;&nbsp;&nbsp;
  <a href="#-projeto">Projeto</a>&nbsp;&nbsp;&nbsp;|&nbsp;&nbsp;&nbsp;
    <a href="#-rotas">Rotas</a>&nbsp;&nbsp;&nbsp;|&nbsp;&nbsp;&nbsp;
  <a href="#-como-rodar">Como rodar</a>&nbsp;&nbsp;&nbsp;|&nbsp;&nbsp;&nbsp;
  <a href="#-como-contribuir">Como contribuir</a>&nbsp;&nbsp;&nbsp;
  </p>

<br>

## API Node.js

## 🚀 Tecnologias

Esse projeto foi desenvolvido com as seguintes tecnologias:

- [Node.js](https://nodejs.org/en/) - v14.4.0
- [Yarn](https://yarnpkg.com/) - 1.22.4
- [Npm](https://www.npmjs.com/) - 6.14.5
- [Docker](https://docs.docker.com/engine/reference/commandline/ps/) - 19.03.8
- [MongoDB](https://www.mongodb.com/)


## 💻 Projeto

API Happy para agendamento de visitas a orfanatos.

## 👩🏿‍💻 Rotas

- **`POST /orphanages`**: Rota para cadastra orfanatos;
Envio
```
name=Lar dos meninos 3
longitute=-49.6394107
latitude=-27.2112735
about=Sobre o orfanato
instructions=Venha visitar.
opening_hours=Das 8h até as 18h
open_on_weekends=true
```
Retorno
```
{
    "name": "Lar dos meninos 3",
    "latitude": "-27.2112735",
    "longitude": "-49.6394107",
    "about": "Sobre o orfanato",
    "instructions": "Venha visitar.",
    "opening_hours": "Das 8h até as 18h",
    "open_on_weekends": true,
    "images": [],
    "id": 14
}
```

- **`GET /orphanages`**: Rota que lista todos os orfanatos;
Retorno
```
[
    {
        "id": 6,
        "name": "Lar das meninas",
        "latitude": -27.2104339,
        "longitude": -49.629111,
        "about": "Sobre o orfanato.",
        "instructions": "Venha visitar.",
        "opening_hours": "Das 8h até as 18h",
        "open_on_weekends": false,
        "images": [
            {
                "id": 3,
                "url": "http://localhost:3333/uploads/1602798242974-99926566-Edi1XzDkRePh7IPFDWrVL2ZelVX7QNnX-cropped-5x7-browser.png",
                "adaptada": "http://192.168.0.44:3333/uploads/1602798242974-99926566-Edi1XzDkRePh7IPFDWrVL2ZelVX7QNnX-cropped-5x7-browser.png"
            },
            {
                "id": 4,
                "url": "http://localhost:3333/uploads/1602798242977-95944351_2662996407276695_2841122244988502016_n.jpg",
                "adaptada": "http://192.168.0.44:3333/uploads/1602798242977-95944351_2662996407276695_2841122244988502016_n.jpg"
            }
        ]
    },
    {
        "id": 8,
        "name": "Lar dos meninos",
        "latitude": -27.2112735,
        "longitude": -49.6394107,
        "about": "Sobre o orfanato",
        "instructions": "Venha visitar.",
        "opening_hours": "Das 8h até as 18h",
        "open_on_weekends": false,
        "images": [
            {
                "id": 5,
                "url": "http://localhost:3333/uploads/1602799292677-99926566-Edi1XzDkRePh7IPFDWrVL2ZelVX7QNnX-cropped-5x7-browser.png",
                "adaptada": "http://192.168.0.44:3333/uploads/1602799292677-99926566-Edi1XzDkRePh7IPFDWrVL2ZelVX7QNnX-cropped-5x7-browser.png"
            },
            {
                "id": 6,
                "url": "http://localhost:3333/uploads/1602799292681-95944351_2662996407276695_2841122244988502016_n.jpg",
                "adaptada": "http://192.168.0.44:3333/uploads/1602799292681-95944351_2662996407276695_2841122244988502016_n.jpg"
            }
        ]
    } 
]
```

- **`GET /orphanages/:id`**: Rota que mostra o detalhe do orfanato;
Retorno
```
{
    "id": 10,
    "name": "Orfanato do bem",
    "latitude": -27.209009516865084,
    "longitude": -49.6378412505805,
    "about": "adfasdfsd",
    "instructions": "dafadsf",
    "opening_hours": "fadsfdsa",
    "open_on_weekends": false,
    "images": [
        {
            "id": 9,
            "url": "http://localhost:3333/uploads/1602818423845-EcQYE51XQAIsiDM.jpg",
            "adaptada": "http://192.168.0.44:3333/uploads/1602818423845-EcQYE51XQAIsiDM.jpg"
        },
        {
            "id": 10,
            "url": "http://localhost:3333/uploads/1602818423846-Eg15D7NWAAEph8X.jpg",
            "adaptada": "http://192.168.0.44:3333/uploads/1602818423846-Eg15D7NWAAEph8X.jpg"
        }
    ]
}
```

## 🚀 Como Rodar

- Clone o projeto.
- Entre na pasta do projeto e rode yarn install (pode usar npm install de acordo com a sua configuração).
- yarn dev para rodar o projeto (localhost:3333).

## 🤔 Como contribuir

- Faça um fork desse repositório;
- Cria uma branch com a sua feature: `git checkout -b minha-feature`;
- Faça commit das suas alterações: `git commit -m 'feat: Minha nova feature'`;
- Faça push para a sua branch: `git push origin minha-feature`.

Depois que o merge da sua pull request for feito, você pode deletar a sua branch.

## 📝 Licença

Esse projeto está sob a licença MIT.
