# Consulta CEP API

Esta é uma API simples para consulta de informações de endereço com base no CEP (Código de Endereçamento Postal) usando o serviço da ViaCEP.

## Tecnologias Utilizadas

- Java
- Spring Boot
- Spring Web
- RestTemplate

## Endpoints

### Consulta CEP

Realiza a consulta de um CEP e retorna as informações de endereço.

- **URL**: `/consulta-cep/{cep}`
- **Método**: `GET`
- **Parâmetros**:
  - `cep`: O CEP a ser consultado (somente números).
- **Resposta**: Um objeto JSON contendo as informações do endereço.

### Exemplo de Requisição

```bash
GET /consulta-cep/01001000


Exemplo de Resposta
------------------------------
```
json

{
  "cep": "01001-000",
  "logradouro": "Praça da Sé",
  "complemento": "lado ímpar",
  "unidade": "",
  "bairro": "Sé",
  "localidade": "São Paulo",
  "uf": "SP",
  "ibge": "3550308",
  "gia": "1004",
  "ddd": "11"
}
```
