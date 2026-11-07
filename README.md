# Aula 07 — Entrega Contínua × Implantação Contínua (ISW032)

Repositório-modelo da prática da Aula 07 de Integração e Entrega Contínua
(Fatec Zona Leste — DSM). Ele guarda o site da loja do Bruno e da Camila e uma
esteira (pipeline) que testa, ensaia e publica o site no GitHub Pages.

## Como usar este modelo

1. Clique no botão verde **Use this template** → **Create a new repository**.
2. Em *Owner*, escolha a sua conta. Em *Repository name*, use `aula07-SEUNOME`.
3. Marque **Public** (obrigatório: o aprovador manual e o Pages gratuito só funcionam em repositório público).
4. Siga o Roteiro do Aluno impresso.

## O que cada arquivo faz e para que serve na aula

| Arquivo | O que faz | Para que serve na aula |
|---|---|---|
| `site/index.html` | A página da loja (promoção e número da versão). | É o "produto" que a esteira publica. Você vai trocar a promoção de 10% para 90% para simular o erro da Sexta às 18h. |
| `.github/workflows/pipeline.yml` | A esteira: `testar` → `homologacao` → `producao`. | É a receita do robô. Mostra o portão de aprovação antes da produção. Você não precisa editá-la. |
| `package.json` | Define o comando `npm test`. | Liga o robô aos testes da Aula 05. |
| `desconto.js`, `desconto.test.js` | Função de desconto e seus testes. | O estágio `testar` roda estes testes antes de qualquer publicação. |
| `frete.js`, `frete.test.js` | Função de frete e seu teste. | Segundo conjunto de testes do estágio `testar`. |

## Onde ver o site

Depois da primeira publicação: `https://SEU-USUARIO.github.io/aula07-SEUNOME/`
