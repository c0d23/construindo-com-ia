# 🔐 Segurança também faz parte da construção

[← Voltar pra bancada](../README.md)

Pra mostrar o antes e depois do Kanban, preparei uma demonstração separada, com mil leads fictícios. Eu precisava comparar duas versões da tela. Não precisava levar a carteira do cliente pra gravação.

Esse é um cuidado bem concreto. Quando o projeto atende uma operação real, tem gente do outro lado daqueles cards.

## O que pode aparecer aqui

Explicações, decisões, exemplos reescritos com dados inventados e resultados que eu consiga mostrar sem expor ninguém.

Código privado do cliente, conversas, credenciais e cópias do banco ficam fora deste repositório. Capturas, vídeos e relatórios também precisam passar por essa conferência. Um teste pode usar dados fictícios e ainda deixar escapar informação de outra aba ou de uma notificação.

Antes de publicar um material, meu checklist é:

- Conferir nomes, telefones, e-mails e mensagens na tela inteira.
- Revisar abas, favoritos, notificações, terminais e arquivos abertos.
- Ocultar dados sensíveis em todos os quadros em que aparecem, inclusive durante transições.
- Rever o vídeo exportado, não só a prévia do editor.
- Não publicar links privados ou artefatos que carreguem mais informação do que o exemplo precisa.

## Um botão escondido não é uma permissão

Imagina alguém que só pode consultar os próprios leads. Esconder uma opção na tela ajuda na experiência, mas a API e o banco também precisam recusar uma tentativa fora desse acesso.

Por isso, quero conferir os dois lados: a ação que a pessoa autorizada consegue fazer e a mesma ação sendo negada para quem não pode. Essa separação entre interface e autorização também aparece nas [recomendações de autorização da OWASP](https://cheatsheetseries.owasp.org/cheatsheets/Authorization_Cheat_Sheet.html).

Um endereço pouco conhecido não substitui essa proteção. O sistema continua precisando validar quem entrou e o que essa pessoa pode acessar.

## Agente trabalhando precisa de limite

Uso terminais separados para dividir as tarefas, com escopo definido e revisão pelo GitHub. Cada alteração precisa deixar claro o que mudou e como foi testado.

Também separo as autorizações. Escrever uma correção não significa poder aplicar mudanças no banco real, instalar qualquer programa ou publicar no site. E teste verde não é sinônimo de “não tem mais nada pra conferir”.

Credenciais de servidor não devem virar parte da interface ou de um exemplo público. Acesso a segredo precisa ser limitado ao trabalho que realmente depende dele. A [referência de gestão de segredos da OWASP](https://cheatsheetseries.owasp.org/cheatsheets/Secrets_Management_Cheat_Sheet.html) aprofunda esses cuidados.

## O laboratório que quero montar 🧪

**Estado atual: em planejamento. Ainda não tenho o laboratório completo instalado e validado.**

A proposta é montar um ambiente separado para aprender segurança enquanto testo hipóteses do CRM. Quero conseguir ver a interface, acompanhar o que o teste tentou fazer e entender por que uma proteção funcionou ou falhou.

O plano inclui:

- Dados e contas inteiramente fictícios, com perfis diferentes.
- Banco e serviços separados da produção.
- Saídas de rede controladas para não mandar mensagem, e-mail ou chamada para alguém de verdade.
- Credenciais exclusivas do ambiente de teste.
- Limites de recursos e uma forma conhecida de encerrar e reconstruir o ambiente.
- Relatórios que mostrem o esperado, o observado e como repetir o caso.

Ter uma pasta chamada “sandbox” não comprova isolamento. Essa separação precisa ser testada antes de começar os experimentos.

## O que quero aprender ali

Começar com perguntas verificáveis: uma sessão encerrada ainda permite alguma ação? Trocar de usuário limpa os dados da tela? Uma requisição repetida gera duplicidade? Uma ação administrativa é recusada para um perfil comum?

Depois, a ideia é seguir cada falha até a correção e repetir o mesmo teste. Sempre em ambiente próprio e autorizado. Este material não é um convite para testar o sistema do cliente ou qualquer sistema de terceiros.

## O que um teste prova, afinal?

| Tipo de teste | O que consigo observar | O que ele não comprova sozinho |
| --- | --- | --- |
| Interface com respostas simuladas | Comportamento dos controles, carregamento e mensagens de erro | Permissões reais do banco |
| Backend isolado com contas fictícias | Regras de acesso e contratos naquele ambiente | Que produção tem exatamente a mesma configuração |
| Comparação de duas versões | Diferenças observadas no mesmo cenário | Qual alteração isolada causou toda a melhora |

Quero trazer os aprendizados conforme acontecerem. Não tenho uma certificação de segurança do CRM pra anunciar, nem vou chamar o planejamento do laboratório de auditoria concluída.

[Continuar: ferramentas da bancada →](ferramentas-da-bancada.md)
