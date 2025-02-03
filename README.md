# Validador de Cartão de Crédito

Este projeto é um validador de cartões de crédito desenvolvido como parte de uma entrega para a DIO. Ele identifica a bandeira do cartão de crédito com base no número fornecido.

## Índice
- [Instalação](#instalação)
- [Uso](#uso)
- [Funcionalidades](#funcionalidades)
- [Contribuição](#contribuição)
- [Licença](#licença)

## Instalação
Para utilizar este projeto, você pode simplesmente clonar o repositório e executar o código localmente.

```sh
git clone https://github.com/seu-usuario/Validador_Cartao_DIO.git
cd Validador_Cartao_DIO
```

## Uso
Para usar o validador de cartão de crédito, você pode executar o arquivo `index.js` com Node.js. Certifique-se de ter o Node.js instalado em sua máquina.

```sh
node src/index.js
```

Você também pode importar a função `validarCartaoCredito` em seu próprio projeto JavaScript.

### Exemplo de Uso

```javascript
const { validarCartaoCredito } = require('./src/index');

const numeroCartao = "5026 6834 6144 5746";
const bandeira = validarCartaoCredito(numeroCartao);

console.log(`A bandeira do cartão é: ${bandeira}`);
```

## Funcionalidades
- Validação de números de cartões de crédito.
- Identificação das seguintes bandeiras:
  - Visa
  - MasterCard
  - American Express
  - Diners Club
  - Discover
  - EnRoute
  - JCB
  - Voyager
  - Hipercard
  - Aura

## Contribuição
Sinta-se à vontade para contribuir com este projeto. Para isso, siga os passos abaixo:

1. Faça um fork do projeto.
2. Crie uma branch para sua feature:
   ```sh
   git checkout -b feature/nova-feature
   ```
3. Commit suas alterações:
   ```sh
   git commit -m 'Adiciona nova feature'
   ```
4. Faça o push para a branch:
   ```sh
   git push origin feature/nova-feature
   ```
5. Abra um Pull Request.

## Licença
Este projeto está licenciado sob a Licença MIT. Veja o arquivo `LICENSE` para mais detalhes.