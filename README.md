<div align="center">

# 🛠️ Construindo com IA

Um CRM, dois computadores e bastante coisa pra descobrir.

**Bastidores · tentativas · coisas que finalmente funcionaram**

</div>

## Opa, chega aí 👋

Tô construindo um CRM pra um cliente meu com ajuda de IA e resolvi mostrar o caminho.

É um projeto pra uma operação real. Tem coisa que funciona, coisa que volta pra revisão e coisa que parecia simples até a gente começar a mexer. Um dos primeiros assuntos é justamente esse: uma tela com mil leads, uns espaços enormes entre os cards e uma rolagem que tava me tirando a paciência.

Esse repo vai ser meu caderno de bastidores. A ideia é juntar aqui os exemplos e as explicações que acompanharem os vídeos, sem precisar contar tudo de uma vez.

## Por onde começar 🧭

| Se você chegou querendo entender… | Pode abrir aqui |
| --- | --- |
| O que aconteceu com o Kanban do primeiro vídeo | [O antes, o depois e a tal borda](docs/primeiro-video.md) |
| Pra que servem os nomes de ferramentas que eu mencionei | [Ponytail, Spec Kit e Grill Me](docs/ferramentas-da-bancada.md) |
| Como testar sem colocar o cliente no meio da experiência | [Segurança também faz parte da construção](docs/seguranca.md) |

## A bancada por aqui 💻

```text
       .-----------------------------.
       |         EU + O MAC          |
       |      a torre de controle    |
       |   organizar e revisar       |
       '--------------+--------------'
                      |
                      v
       .-----------------------------.
       |           GITHUB            |
       | pedidos, mudanças, revisões |
       '--------------+--------------'
                      ^
                      |
                      v
       .-----------------------------.
       |           WINDOWS           |
       |    terminais trabalhando    |
       |      execução e testes      |
       '-----------------------------'
```

Os terminais têm cores pra eu não me perder no meio das tarefas. Tem Ciano, Violeta, Âmbar... e cada trabalho precisa ter um responsável.

Nem tudo é automático. Eu continuo coordenando, conferindo o que voltou e aprovando o que vai pro site. Como essa organização funciona merece um vídeo só pra ela.

<details>
<summary>Um detalhe importante sobre o Ciano</summary>

Numa transcrição de voz, ele virou “Luciano”. Então, se aparecer um Luciano trabalhando no Kanban, já sabe de onde veio. 😂

</details>

## Também fazem parte da bancada 🧰

Tô usando **Ponytail**, **Spec Kit** e **Grill Me** nessa construção também. Cada um ajuda numa parte diferente:

| Ferramenta | Como eu penso nela por aqui |
| --- | --- |
| [Ponytail, de Dietrich Gebert](https://github.com/DietrichGebert/ponytail) | Conferir o que já existe e evitar inventar uma solução maior que o problema. |
| [Spec Kit, do GitHub](https://github.com/github/spec-kit) | Organizar o pedido, o plano e as tarefas antes de sair alterando tudo. |
| [Grill Me, do Matt Pocock](https://github.com/mattpocock/skills) | Fazer as perguntas que faltaram antes de tratar uma ideia como se estivesse pronta. |

Não são três modelos de IA, nem botões que garantem código certo. São ferramentas e instruções que ajudam a conduzir o trabalho do agente. [Contei melhor, com exemplos, neste texto.](docs/ferramentas-da-bancada.md)

Tem trabalho de outras pessoas fazendo parte dessa história. Os créditos são de quem criou cada ferramenta; por aqui, eu compartilho minha experiência usando elas.

## Começando a série 🎬

**01 · Kanban, antes e depois: a história da borda** · publicado no YouTube

O espaço entre os cards, a investigação da rolagem e uma borda que entrou na história. Preparei a demonstração com dados fictícios para comparar duas versões fora da operação do cliente. [Os bastidores desse episódio estão aqui.](docs/primeiro-video.md)

**Depois disso: por dentro da torre**

Quero mostrar uma tarefa passando pelo Mac, pelos terminais do Windows e pela revisão. Com um caso concreto fica bem mais fácil de entender.

> O primeiro vídeo já saiu. Vou acrescentar o link aqui; os próximos episódios ainda vão ser gravados.

## E a segurança nessa história? 🔐

Tem cliente de verdade usando o sistema. Então não dá pra tratar todo pedido como autorização pra mexer em tudo.

Uma parte do meu trabalho é justamente separar as coisas: demonstração de operação, teste de publicação, acesso necessário de acesso demais. Os agentes ajudam a implementar e revisar, mas continuam precisando de limites e evidências.

Também estou planejando um laboratório isolado para aprender e testar segurança com dados fictícios. Ele ainda não está pronto. Quero mostrar a montagem e os testes conforme forem acontecendo, sem vender planejamento como resultado.

[Aqui explico esses cuidados e o que quero testar no laboratório.](docs/seguranca.md)

## O que eu quero trazer pra cá 🌱

- Exemplos que você consiga acompanhar junto com os vídeos.
- O que tentamos, o que mudou e o que ainda ficou pendente.
- Jeitos de organizar o trabalho com os agentes sem um atropelar o outro.

Se uma coisa melhorou no meu computador, vou contar como foi testada. Se ainda engasgou, isso também faz parte da história.

## Só um combinado

O CRM é usado numa operação real, então dados de clientes, conversas, senhas e código privado ficam fora daqui. Os exemplos públicos vão usar dados fictícios.

Este espaço acompanha a construção. Não é o código completo do CRM nem acesso ao sistema.

<div align="center">

☕ Aos poucos, eu vou mostrando o que estamos construindo.

</div>
