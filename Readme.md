# Exercício - UFMG - Engenharia de Software 2

Victor Kenji P Abeki - 2020007090

Para responder este exercício, primeiramente, você deve fazer um `fork` deste repositório.
No Moodle, você deve submeter apenas a URL do seu `fork`.

Em seguida, adicione o arquivo gerado `index.html` no seu fork.

Por fim, responda as questões abaixo no seu `fork`: 

1. Repositório selecionado: https://github.com/expressjs/express

2. Gráfico selecionado: Lines of Code (LOC)
  
3. Explicação: 

Esse gráfico (LOC) mostra a evolução da densidade total do código ao longo do tempo, medida como a quantidade de linhas de código no projeto do Express, entre 2020 e 2025. Nele é possível observar uma estabilidade de 2020 até o início de 2022. A partir desse ponto houve um aumento de 20.861 para 23.279 e depois, a partir de 2024, teve a diminuição de 23.309 para 21.265.

![image](https://github.com/user-attachments/assets/ae9bf7a0-0c54-4b7b-9f0b-e7bd7e1046e0)

Ao comparar essas mudanças com os outros gráficos como o "Conditionals", "Loops", "Functions", "Exceptions" e "Comments", verificamos que o padrão é similar, com aumento a partir de 2022 e diminuição a partir de 2024.

As curvas indicadas no GitEvo do repositório Express, exibem um padrão de boas práticas, uma vez que mantêm a estabilidade e complexidade. Além disso, mesmo com o pequeno aumento de complexidade, em 2022, o gráfico mostrou a busca por boas práticas por parte da equipe e a posterior redução dessa complexidade, a partir de 2024.

Realizei a consulta de commits, alterações e atualizações nos docs do repositório, para a melhor análise das mudanças. Assim, verifiquei o seguinte gráfico de frequência de código do repositório nos períodos observados do GitEvo:

![Code frequency](https://github.com/user-attachments/assets/829e00ea-fef5-4e59-8be8-76773196241b)

Foi possível perceber uma adição de linhas em março de 2022, e uma posterior série de alterações a partir de 2024. Em 2022, no docs de histórico (4.18.0 / 2022-04-25), verifiquei que foram modificadas e corrigidas diversas dependências, além de outras partes do código. Ademais, verificando a lista de commits no período de Março, percebi a implementação e modificação de testes, que podem ter contribuído no aumento de LOC, como em:

- https://github.com/expressjs/express/commit/03dc3671874b214f67dacaca90f39a1c389f822e
- https://github.com/expressjs/express/commit/291993d73c0c92c1ccce2dad264c86bdd1b4fe4b.

Em relação a 2024, período que houve a diminuição de LOC e uma leve diminuição no gráfico selecionado para análise, verifiquei commits que faziam a limpeza e remoção de código, atualização de dependências e de arquivos de workflow, e atualizações na documentação. Podemos observar os commits:

- https://github.com/expressjs/express/commit/4e92ac903194b705a121ec49103fd9fcd779a42b
- https://github.com/expressjs/express/commit/bdd81f8670975ef30fd49e92513ef48d35029eaf
- https://github.com/expressjs/express/commit/6c98f80b6ac95b90cff5da6857be4fe21d5e9c4e
- https://github.com/expressjs/express/commit/63992bb1d7da401cdf7dfbb9d45d99c63b69c0e6

## 

[![Express Logo](https://i.cloudup.com/zfY6lL7eFa-3000x3000.png)](https://expressjs.com/)

**Fast, unopinionated, minimalist web framework for [Node.js](https://nodejs.org).**

**This project has a [Code of Conduct][].**

## Table of contents

* [Installation](#Installation)
* [Features](#Features)
* [Docs & Community](#docs--community)
* [Quick Start](#Quick-Start)
* [Running Tests](#Running-Tests)
* [Philosophy](#Philosophy)
* [Examples](#Examples)
* [Contributing to Express](#Contributing)
* [TC (Technical Committee)](#tc-technical-committee)
* [Triagers](#triagers)
* [License](#license)


[![NPM Version][npm-version-image]][npm-url]
[![NPM Downloads][npm-downloads-image]][npm-downloads-url]
[![OpenSSF Scorecard Badge][ossf-scorecard-badge]][ossf-scorecard-visualizer]


```js
import express from 'express'

const app = express()

app.get('/', (req, res) => {
  res.send('Hello World')
})

app.listen(3000)
```

## Installation

This is a [Node.js](https://nodejs.org/en/) module available through the
[npm registry](https://www.npmjs.com/).

Before installing, [download and install Node.js](https://nodejs.org/en/download/).
Node.js 18 or higher is required.

If this is a brand new project, make sure to create a `package.json` first with
the [`npm init` command](https://docs.npmjs.com/creating-a-package-json-file).

Installation is done using the
[`npm install` command](https://docs.npmjs.com/getting-started/installing-npm-packages-locally):

```bash
npm install express
```

Follow [our installing guide](https://expressjs.com/en/starter/installing.html)
for more information.

## Features

  * Robust routing
  * Focus on high performance
  * Super-high test coverage
  * HTTP helpers (redirection, caching, etc)
  * View system supporting 14+ template engines
  * Content negotiation
  * Executable for generating applications quickly

## Docs & Community

  * [Website and Documentation](https://expressjs.com/) - [[website repo](https://github.com/expressjs/expressjs.com)]
  * [GitHub Organization](https://github.com/expressjs) for Official Middleware & Modules
  * [Github Discussions](https://github.com/expressjs/discussions) for discussion on the development and usage of Express

**PROTIP** Be sure to read the [migration guide to v5](https://expressjs.com/en/guide/migrating-5)

## Quick Start

  The quickest way to get started with express is to utilize the executable [`express(1)`](https://github.com/expressjs/generator) to generate an application as shown below:

  Install the executable. The executable's major version will match Express's:

```bash
npm install -g express-generator@4
```

  Create the app:

```bash
express /tmp/foo && cd /tmp/foo
```

  Install dependencies:

```bash
npm install
```

  Start the server:

```bash
npm start
```

  View the website at: http://localhost:3000

## Philosophy

  The Express philosophy is to provide small, robust tooling for HTTP servers, making
  it a great solution for single page applications, websites, hybrids, or public
  HTTP APIs.

  Express does not force you to use any specific ORM or template engine. With support for over
  14 template engines via [@ladjs/consolidate](https://github.com/ladjs/consolidate),
  you can quickly craft your perfect framework.

## Examples

  To view the examples, clone the Express repository:

```bash
git clone https://github.com/expressjs/express.git --depth 1 && cd express
```

  Then install the dependencies:

```bash
npm install
```

  Then run whichever example you want:

```bash
node examples/content-negotiation
```

## Contributing

  [![Linux Build][github-actions-ci-image]][github-actions-ci-url]
  [![Test Coverage][coveralls-image]][coveralls-url]

The Express.js project welcomes all constructive contributions. Contributions take many forms,
from code for bug fixes and enhancements, to additions and fixes to documentation, additional
tests, triaging incoming pull requests and issues, and more!

See the [Contributing Guide](Contributing.md) for more technical details on contributing.

### Security Issues

If you discover a security vulnerability in Express, please see [Security Policies and Procedures](Security.md).

### Running Tests

To run the test suite, first install the dependencies:

```bash
npm install
```

Then run `npm test`:

```bash
npm test
```

## People

The original author of Express is [TJ Holowaychuk](https://github.com/tj)

[List of all contributors](https://github.com/expressjs/express/graphs/contributors)

### TC (Technical Committee)

* [UlisesGascon](https://github.com/UlisesGascon) - **Ulises Gascón** (he/him)
* [jonchurch](https://github.com/jonchurch) - **Jon Church**
* [wesleytodd](https://github.com/wesleytodd) - **Wes Todd**
* [LinusU](https://github.com/LinusU) - **Linus Unnebäck**
* [blakeembrey](https://github.com/blakeembrey) - **Blake Embrey**
* [sheplu](https://github.com/sheplu) - **Jean Burellier**
* [crandmck](https://github.com/crandmck) - **Rand McKinney**
* [ctcpip](https://github.com/ctcpip) - **Chris de Almeida**

<details>
<summary>TC emeriti members</summary>

#### TC emeriti members

  * [dougwilson](https://github.com/dougwilson) - **Douglas Wilson**
  * [hacksparrow](https://github.com/hacksparrow) - **Hage Yaapa**
  * [jonathanong](https://github.com/jonathanong) - **jongleberry**
  * [niftylettuce](https://github.com/niftylettuce) - **niftylettuce**
  * [troygoode](https://github.com/troygoode) - **Troy Goode**
</details>


### Triagers

* [aravindvnair99](https://github.com/aravindvnair99) - **Aravind Nair**
* [bjohansebas](https://github.com/bjohansebas) - **Sebastian Beltran**
* [carpasse](https://github.com/carpasse) - **Carlos Serrano**
* [CBID2](https://github.com/CBID2) - **Christine Belzie**
* [dpopp07](https://github.com/dpopp07) - **Dustin Popp**
* [UlisesGascon](https://github.com/UlisesGascon) - **Ulises Gascón** (he/him)
* [3imed-jaberi](https://github.com/3imed-jaberi) - **Imed Jaberi**
* [IamLizu](https://github.com/IamLizu) - **S M Mahmudul Hasan** (he/him)
* [Phillip9587](https://github.com/Phillip9587) - **Phillip Barta**
* [Sushmeet](https://github.com/Sushmeet) - **Sushmeet Sunger**
* [rxmarbles](https://github.com/rxmarbles) **Rick Markins** (He/him)

<details>
<summary>Triagers emeriti members</summary>

#### Emeritus Triagers

  * [AuggieH](https://github.com/AuggieH) - **Auggie Hudak**
  * [G-Rath](https://github.com/G-Rath) - **Gareth Jones**
  * [MohammadXroid](https://github.com/MohammadXroid) - **Mohammad Ayashi**
  * [NawafSwe](https://github.com/NawafSwe) - **Nawaf Alsharqi**
  * [NotMoni](https://github.com/NotMoni) - **Moni**
  * [VigneshMurugan](https://github.com/VigneshMurugan) - **Vignesh Murugan**
  * [davidmashe](https://github.com/davidmashe) - **David Ashe**
  * [digitaIfabric](https://github.com/digitaIfabric) - **David**
  * [e-l-i-s-e](https://github.com/e-l-i-s-e) - **Elise Bonner**
  * [fed135](https://github.com/fed135) - **Frederic Charette**
  * [firmanJS](https://github.com/firmanJS) - **Firman Abdul Hakim**
  * [getspooky](https://github.com/getspooky) - **Yasser Ameur**
  * [ghinks](https://github.com/ghinks) - **Glenn**
  * [ghousemohamed](https://github.com/ghousemohamed) - **Ghouse Mohamed**
  * [gireeshpunathil](https://github.com/gireeshpunathil) - **Gireesh Punathil**
  * [jake32321](https://github.com/jake32321) - **Jake Reed**
  * [jonchurch](https://github.com/jonchurch) - **Jon Church**
  * [lekanikotun](https://github.com/lekanikotun) - **Troy Goode**
  * [marsonya](https://github.com/marsonya) - **Lekan Ikotun**
  * [mastermatt](https://github.com/mastermatt) - **Matt R. Wilson**
  * [maxakuru](https://github.com/maxakuru) - **Max Edell**
  * [mlrawlings](https://github.com/mlrawlings) - **Michael Rawlings**
  * [rodion-arr](https://github.com/rodion-arr) - **Rodion Abdurakhimov**
  * [sheplu](https://github.com/sheplu) - **Jean Burellier**
  * [tarunyadav1](https://github.com/tarunyadav1) - **Tarun yadav**
  * [tunniclm](https://github.com/tunniclm) - **Mike Tunnicliffe**
  * [enyoghasim](https://github.com/enyoghasim) - **David Enyoghasim**
  * [0ss](https://github.com/0ss) - **Salah**
  * [import-brain](https://github.com/import-brain) - **Eric Cheng** (he/him)
  * [dakshkhetan](https://github.com/dakshkhetan) - **Daksh Khetan** (he/him)
  * [lucasraziel](https://github.com/lucasraziel) - **Lucas Soares Do Rego**
  * [mertcanaltin](https://github.com/mertcanaltin) - **Mert Can Altin**
  
</details>


## License

  [MIT](LICENSE)

[coveralls-image]: https://badgen.net/coveralls/c/github/expressjs/express/master
[coveralls-url]: https://coveralls.io/r/expressjs/express?branch=master
[github-actions-ci-image]: https://badgen.net/github/checks/expressjs/express/master?label=CI
[github-actions-ci-url]: https://github.com/expressjs/express/actions/workflows/ci.yml
[npm-downloads-image]: https://badgen.net/npm/dm/express
[npm-downloads-url]: https://npmcharts.com/compare/express?minimal=true
[npm-url]: https://npmjs.org/package/express
[npm-version-image]: https://badgen.net/npm/v/express
[ossf-scorecard-badge]: https://api.scorecard.dev/projects/github.com/expressjs/express/badge
[ossf-scorecard-visualizer]: https://ossf.github.io/scorecard-visualizer/#/projects/github.com/expressjs/express
[Code of Conduct]: https://github.com/expressjs/express/blob/master/Code-Of-Conduct.md
