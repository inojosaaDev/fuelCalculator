# ⛽ 10D Challenge | Escola Nova Era Tech | Calculadora de Combustível/Fuel Calculator

Fiz este projeto com o auxílio do professor Roque, da Escola Nova Era Tech. Ele consiste em um aplicativo Android, desenvolvido em Kotlin, que calcula quanto você vai gastar de combustível em uma viagem a partir do preço do litro, do consumo do veículo e da distância percorrida.

## 🧩 Tecnologias e conceitos utilizados

Este projeto utiliza **fundamentos do Android tradicional**:

- Kotlin
- Android SDK (minSdk 24, targetSdk 37)
- Activities
- UI com XML (com ConstraintLayout)
  - TextView
  - EditText
  - Button
- Material Components (`MaterialToolbar`)
- Toolbar
- Navegação entre telas com Intent
- Passagem de dados entre telas com Bundle
- Organização básica de layouts e telas
- Gradle com Kotlin DSL

Os dados são passados de uma tela para a próxima por meio de `Intent` (`putExtra` / `getExtra`), que guarda esses valores em um `Bundle`.

## 📱 Como funciona

O app guia o usuário por um fluxo simples de telas:

1. **Início**: apresentação do app e botão para começar.
2. **Preço do combustível**: valor do litro (ex.: 5,89).
3. **Consumo do veículo**: quantos quilômetros o carro faz por litro (km/l).
4. **Distância da viagem**: quantos quilômetros serão percorridos.
5. **Resultado**: custo total da viagem e um resumo dos dados informados, com opção de fazer um novo cálculo.

### Cálculo

```
litros necessários = distância ÷ consumo
custo total        = litros necessários × preço por litro
```

**Exemplo:** 600 km, consumo de 12 km/l e gasolina a R$ 5,00 o litro

- Litros necessários: 600 ÷ 12 = 50 L
- Custo total: 50 × 5,00 = **R$ 250,00**

## 📸 Screenshots

> Adicione aqui capturas de tela do app (pasta `screenshots/` no repositório).

| Início | Preço | Consumo | Distância | Resultado |
|:------:|:-----:|:-------:|:---------:|:---------:|
| ![Início](screenshots/inicio.png) | ![Preço](screenshots/preco.png) | ![Consumo](screenshots/consumo.png) | ![Distância](screenshots/distancia.png) | ![Resultado](screenshots/resultado.png) |

## 📚 Sobre o projeto

Projeto desenvolvido para praticar desenvolvimento Android com Kotlin: navegação entre Activities, passagem de dados com `Intent` e construção de layouts em XML.

## 🏁 Resultado final

Ao concluir o **10D Challenge**, o resultado é:

- ✅ Um aplicativo Android funcional
- ✅ Um projeto publicado no GitHub
- ✅ Base sólida de lógica de programação
- ✅ Primeiro contato real com desenvolvimento Android

Este projeto representa o início da minha jornada no ecossistema Android dentro da **Escola Nova Era Tech** 🚀

## 📄 Licença

Este projeto está sob a licença **MIT**. Consulte o arquivo LICENSE para mais detalhes.

## 🤝 Contribuições

Contribuições são bem-vindas! Este é um projeto de aprendizado e fico feliz em receber sugestões, correções e melhorias.

## 👤 Autor

Feito por **Matheus Gomes**, desenvolvedor mobile (Android | Kotlin).

- GitHub: [@inojosaaDev](https://github.com/inojosaaDev)
- LinkedIn: [in/matheus-inojosa](https://www.linkedin.com/in/matheus-inojosa/)
