# ⛽ Calculadora de Combustível

Aplicativo Android, desenvolvido em Kotlin, que calcula quanto você vai gastar de combustível em uma viagem a partir do preço do litro, do consumo do veículo e da distância percorrida.

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

## 🛠️ Tecnologias

- [Kotlin](https://kotlinlang.org/)
- Android SDK (minSdk 24, targetSdk 37)
- Views em XML com ConstraintLayout
- Material Components (`MaterialToolbar`)
- Gradle com Kotlin DSL

## 🧩 Estrutura do projeto

```
app/src/main/java/com/example/myapplication/
├── MainActivity.kt              # Tela inicial
├── PrecoCombustivelActivity.kt  # Entrada do preço do litro
├── ConsumoLitroActivity.kt      # Entrada do consumo (km/l)
├── DistanciaActivity.kt         # Entrada da distância e cálculo do custo
└── ResultadoActivity.kt         # Exibição do resultado
```

Os dados são passados de uma tela para a próxima por meio de `Intent` (`putExtra` / `getExtra`).

## ▶️ Como executar

**Pré-requisitos:** [Android Studio](https://developer.android.com/studio) instalado e um emulador ou celular Android (Android 7.0 ou superior).

```bash
# 1. Clone o repositório
git clone https://github.com/inojosaaDev/fuelCalculator.git

# 2. Abra a pasta no Android Studio e aguarde o sync do Gradle

# 3. Execute o app (botão Run) em um emulador ou dispositivo
```

## 🚀 Melhorias futuras

- [ ] Validar campos vazios e valores inválidos
- [ ] Aceitar consumo e distância com casas decimais
- [ ] Formatar o resultado em reais (R$ 0,00)
- [ ] Salvar o histórico de cálculos
- [ ] Permitir escolher o tipo de combustível (gasolina, etanol, diesel)
- [ ] Migrar para Jetpack Compose

## 📚 Sobre o projeto

Projeto desenvolvido para praticar desenvolvimento Android com Kotlin: navegação entre Activities, passagem de dados com `Intent` e construção de layouts em XML.

## 👤 Autor

Feito por **Matheus Gomes**, desenvolvedor mobile (Android | Kotlin).

- GitHub: [@inojosaaDev](https://github.com/inojosaaDev)
- LinkedIn: [in/matheus-inojosa](https://www.linkedin.com/in/matheus-inojosa/)
