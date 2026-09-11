# 🎬 O antes, o depois e a tal borda

[← Voltar pra bancada](../README.md)

O primeiro vídeo já foi publicado no YouTube. O link entra aqui em breve.

O assunto é um problema que estava me incomodando no CRM: espaço demais entre os cards e travamentos na navegação do Kanban.

## Dois problemas na mesma tela

O vazio entre os cards era fácil de enxergar. O espaço reservado para cada card tinha uma altura mínima, mesmo quando o conteúdo era menor. A correção passou a acompanhar a altura do card.

Já os engasgos exigiram outra investigação. O Kanban já montava os cards próximos da área visível, então não bastava dizer “é só não renderizar os mil de uma vez”.

Uma das mudanças investigadas foi o contorno das colunas: de tracejado para contínuo. Ela apareceu como uma contribuição para a melhora da rolagem nos testes daquele cenário. A atualização também teve mudanças na medição e no tratamento visual dos cards.

## A borda resolveu tudo sozinha?

Não dá pra concluir isso comparando o pacote completo de duas versões. Eu senti uma melhora no uso depois da atualização, mas não vou transformar essa observação numa regra de que toda borda tracejada deixa qualquer sistema lento.

Pra separar a contribuição de cada mudança, seria preciso comparar os casos de forma controlada. O antes e depois do vídeo serve para apresentar a história e o comportamento da demonstração.

## Como preparei a demonstração

Separei duas versões do Kanban, com a mesma massa de mil leads fictícios, para abrir localmente no Windows. Esse ambiente não depende do banco da operação e não reproduz toda a carga do sistema real.

Não coloquei lentidão artificial no “antes”. Se um engasgo não aparecer naquela máquina, isso também faz parte do resultado. Os dados e o código privado do cliente não estão disponíveis neste repositório público.

## O próximo bastidor

Quero gravar uma tarefa passando pela torre no Mac, pela execução no Windows e pela revisão no GitHub. A parte interessante é acompanhar uma decisão concreta, inclusive quando a primeira entrega volta para correção.

Esse próximo episódio ainda não foi gravado. Enquanto isso, deixei aqui uma explicação das [ferramentas que uso](ferramentas-da-bancada.md) e dos [cuidados de segurança](seguranca.md).
