<p align="center">
  <img src="/api/public/logo.svg" width="90px" float="center"/>
</p>
<h1 align="center">COVID-19 Brazil API</h1>
<p align="center">
  <strong>Notificação de casos de doença pelo coronavírus 2019 (COVID-19) no Brasil</strong>
</p>

[English version](./README-US.md) 🇺🇸

## Motivo 🤔

Fornecer uma API JSON com dados atualizados sobre o avanço do coronavírus no Brasil, assim como em outros países.

## Datasets 💽

- [CSSEGISandData](https://github.com/CSSEGISandData/COVID-19)
- [Ministério da Saúde](http://plataforma.saude.gov.br/novocoronavirus)

## Showcase 🎯

- [APP COVID-19 Estatísticas 📱](https://github.com/robsonsilv4/covid19_statistics)

## Servidor de desenvolvimento 🚀

Clonando o projeto:

```
git clone https://github.com/devarthurribeiro/covid19-brazil-api.git
```

Navegando até a pasta do projeto:

```
cd covid19-brazil-api/api
```

Baixando as dependências do projeto

```bash
yarn
```

Rodando o projeto

```bash
yarn dev
```

Visite [http://localhost:3000](http://localhost:3000) com o seu navegador para ver o resultado.

## Endpoints 🔌

Todas chamadas devem usar a url base:

```
https://covid19-brazil-api.now.sh
```

#### Consultar dados de casos por estado

```
// GET /api/report/v1

{
"data": [
    {
      "uid": 35,
      "datetime": "2020-03-18T20:00:00.000Z",
      "uf": "SP",
      "state": "São Paulo",
      "cases": 164,
      "deaths": 1,
      "suspects": 5047,
      "refuses": 709,
    }
    //...
   ]
}
```

#### Consultar dados de casos de todos países

```
// GET /api/report/v1/countries

{
"data": [
    {
      "country": "Brazil",
      "cases": 523,
      "confirmed": 529,
      "deaths": 4,
      "recovered": 2,
      "updated_at": "2020-03-19T02:53:32.000Z"
    }
    //...
   ]
}
```

#### Consultar dados de casos por país

```
// GET /api/report/v1/:country

// resultado para /api/report/v1/brazil
{
  "data": {
    "country": "Brazil",
    "cases": 523,
    "confirmed": 529,
    "deaths": 4,
    "recovered": 2,
    "updated_at": "2020-03-19T02:53:32.000Z"
  }
}
```

#### Consultar status da API

```
// GET /api/status/v1

{
  "status": "ok",
  "date": "2020-03-18T12:37:59.227Z",
  "environment": "production",
  "aws": {
    "region": "us-west-1",
    "function_version": "$LATEST"
  }
}
```

## License 📄

This project is licensed under the [MIT License](https://opensource.org/licenses/MIT) - see the [LICENSE](LICENSE) file for details.

## Contribuidores

<table>
  <tr>
    <td align="center"><a href="https://github.com/Lukazovic"><img src="https://avatars0.githubusercontent.com/u/54550926?s=460&u=cdeeac652ce0597a986fbdcff6e249ad27a1f1da&v=4" width="100px;" alt=""/><br /><sub><b>Lucas Vieira</b></sub></a><br /><a href="https://github.com/devarthurribeiro/covid19-brazil-api/commits?author=Lukazovic" title="Code">💻</a></a></td>
  <tr>
</table>

## Autor

<table>
  <tr>
    <td align="center"><a href="https://github.com/devarthurribeiro"><img src="https://avatars1.githubusercontent.com/u/12974798?s=460&u=6a69934913c6f56d74fdf9c80793881d4cfb7bf6&v=4" width="100px;" alt=""/><br /><sub><b>Arthur Ribeiro</b></sub></a><br /><a href="https://github.com/devarthurribeiro/covid19-brazil-api/commits?author=devarthurribeiro" title="Code">💻</a> <a href="#devarthurribeiro" title="Design">🎨</a></td>
  <tr>
</table>
