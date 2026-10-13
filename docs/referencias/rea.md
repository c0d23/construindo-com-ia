# REA — referência técnica

Referência salva em 13/10/2026 para avaliação futura. Este arquivo é uma nota com links e análise documental, **não um fork nem um backup do código-fonte**.

## Origem e versão observada

- Projeto: https://github.com/morluto/rea
- Como funciona: https://github.com/morluto/rea#how-rea-works
- Commit observado: https://github.com/morluto/rea/commit/4c838469477f0b6ea844c235f78534a55118ddca
- Release consultada: https://github.com/morluto/rea/releases/tag/rea-agents-6.4.0 — publicada em 11/10/2026.
- Licença do código do REA: MIT. Preservar os avisos exigidos pela licença. Ferramentas e componentes de terceiros têm termos próprios.
- Licença: https://github.com/morluto/rea/blob/4c838469477f0b6ea844c235f78534a55118ddca/LICENSE

## O que faz

CLI e servidor MCP local que fornecem evidências de inspeção para agentes de IA. Conforme o fluxo, usa análise de aplicativos nativos, JavaScript/Electron, .NET e comportamento de navegador. O agente interpreta as evidências e pode propor uma implementação; a ferramenta não garante reconstrução integral nem correta.

Código de referência: https://github.com/morluto/rea/blob/4c838469477f0b6ea844c235f78534a55118ddca/src/cli/applicationCommands.ts

## Quando avaliar

- Entender uma funcionalidade não documentada em software próprio ou autorizado.
- Mapear entradas, validações e saídas de uma aplicação legada.
- Reconstruir regras com rastreabilidade e criar casos de regressão.

Para uma planilha, o primeiro passo mais direto é estudar fórmulas, validações, tabelas de referência e macros, quando existirem. Não foi identificado suporte específico documentado de Excel/VBA nos pontos revisados. REA não é um conversor de Excel em ERP.

## Fluxo de trabalho proposto

1. Delimitar um processo e confirmar autorização.
2. Identificar entradas, regras, saídas e referências de origem.
3. Separar comportamento observado, hipótese e dúvida.
4. Validar regras com quem opera o processo; comportamentos antigos também podem estar errados.
5. Criar exemplos e casos de borda com resultados esperados.
6. Implementar e conferir contra esses casos em ambiente isolado.

## Requisitos e limites

A documentação consultada declara Node.js 22.19+ na linha 22, 24.11+ na linha 24 ou 26+, além de npm. Os mecanismos de análise têm dependências próprias. Conferir novamente antes de qualquer instalação.

A branch main pode documentar recursos posteriores ao pacote publicado: https://github.com/morluto/rea/blob/main/docs/installation.md#released-package-and-main

Resultados podem ser incompletos. Evidências enviadas ao agente podem chegar ao provedor do modelo: execução local não equivale a confidencialidade integral. Inspeção dinâmica pode alterar estado. Usar apenas alvos próprios ou autorizados e respeitar licenças e dados.

Limites declarados pelo projeto: https://github.com/morluto/rea/blob/main/DISCLAIMER.md

## Estado desta referência

Somente documentação e trechos de código foram consultados. Nada instalado ou executado. Cópia independente do repositório ainda pendente; esta nota não preserva o código se a origem ficar indisponível.
