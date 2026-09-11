# 🧰 O que essas ferramentas fazem por aqui

[← Voltar pra bancada](../README.md)

Uma coisa é pedir “corrige isso”. Outra é explicar o que está errado, o que precisa continuar funcionando e como a gente vai saber que a correção deu certo.

É nessa diferença que entram Ponytail, Spec Kit e Grill Me. Tô usando essas ferramentas na construção, mas cada uma tem um papel. Não significa que todo terminal roda as três em toda tarefa.

## Ponytail: será que precisa criar tudo isso?

O [Ponytail, de Dietrich Gebert](https://github.com/DietrichGebert/ponytail), orienta o agente a procurar recursos da plataforma, bibliotecas e código já existente antes de construir uma solução nova.

Por aqui, essa ideia aparece quando uma correção pode reaproveitar um componente que já funciona. No CRM, por exemplo, precisávamos oferecer a mudança de etapa em outro lugar da interface. Reutilizar o seletor existente ajudou a manter o comportamento consistente entre as telas.

Minha pergunta nesse momento é: “qual é a menor alteração que atende o pedido inteiro?”

O “inteiro” importa. Tirar validação, tratamento de erro ou acessibilidade só pra diminuir o código não resolve o problema.

## Spec Kit: tirar o pedido da minha cabeça

O [Spec Kit, do GitHub](https://github.com/github/spec-kit), organiza o desenvolvimento a partir de uma especificação. O fluxo inclui definir o que deve ser construído, montar um plano e dividir a implementação em tarefas.

É uma ajuda pra transformar uma ideia solta em trabalho que outra pessoa, ou outro agente, consegue entender. Eu tenho muita ideia ao mesmo tempo. Se tudo vira “faz isso também”, fica difícil saber onde uma tarefa acaba e outra começa.

Um exemplo didático de como estruturar um pedido:

> Quero um botão para voltar ao Kanban. Ao voltar, o funil, o vendedor selecionado e a posição de rolagem precisam continuar como estavam. Tem que funcionar no celular e pelo teclado.

Isso já diz bem mais do que “coloca um botão de voltar”. A configuração do Spec Kit e um caso completo de uso ficam para um episódio próprio; este texto não é um registro de execução de todos os comandos dele.

## Grill Me: a pergunta chata que evita retrabalho

O [Grill Me, do Matt Pocock](https://github.com/mattpocock/skills), conduz uma conversa de perguntas sobre um plano ou uma ideia para esclarecer decisões que ficaram abertas.

É o tipo de conversa que eu quero ter antes de mandar os terminais implementarem. Quando digo “quero notificações”, por exemplo, ainda falta decidir muita coisa:

- A pessoa precisa receber mesmo com o CRM fechado?
- Abrir o aviso significa que ela confirmou ciência?
- Se o compromisso mudar de horário, precisa confirmar de novo?
- O que acontece quando muda o responsável?

Esses são exemplos das dúvidas que apareceram no projeto, não uma transcrição de uma sessão específica da ferramenta.

Responder antes ajuda a evitar que o agente escolha uma regra de negócio por mim. E também evita descobrir, depois de pronto, que a gente estava imaginando coisas diferentes.

## Como as peças se encontram

```text
   ideia ainda meio solta
             |
      perguntas e decisões
             |
      pedido + plano + tarefas
             |
      implementação com escopo
             |
      testes + revisão + ajustes
             |
      aprovação para publicar
```

Esse desenho representa a organização que estou construindo. Não é uma integração automática pronta entre as ferramentas.

Na prática, o GitHub guarda os pedidos e as devolutivas. O Mac fica como torre de controle; os terminais do Windows executam tarefas separadas. Às vezes o teste passa e a revisão ainda encontra um caso que ninguém cobriu. A tarefa volta, recebe o ajuste e precisa ser conferida de novo.

## Créditos e um cuidado antes de instalar

Os projetos originais são [Ponytail](https://github.com/DietrichGebert/ponytail), [Spec Kit](https://github.com/github/spec-kit) e [as skills do Matt Pocock](https://github.com/mattpocock/skills). Este repositório não é mantido por eles e não redistribui suas ferramentas. Estou compartilhando minha experiência de uso.

Para instalar, confira as instruções e a licença no projeto original. Eu também preciso olhar o que uma ferramenta vai executar, quais arquivos pode alterar e a quais credenciais terá acesso. Uma skill continua sendo instrução entregue a um agente; ela não torna qualquer comando automaticamente seguro.

[Continuar: segurança também faz parte da construção →](seguranca.md)
