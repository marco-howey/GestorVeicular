# 🚗 Gestor Veicular

Projeto acadêmico de Engenharia de Software voltado à leitura de dados do veículo, ao acompanhamento de seu uso e à organização da manutenção preventiva.

## Sobre o projeto
O Gestor Veicular é desenvolvido na disciplina de Projeto Integrador. A proposta é ajudar o motorista a acompanhar as informações disponíveis do veículo e saber quando realizar as manutenções preventivas, reunindo dados de leitura, registros de serviços e intervalos de manutenção.

A prioridade atual é consolidar esse fluxo com um veículo de teste antes de ampliar o escopo. O desenvolvimento será realizado em etapas pequenas, respeitando o aprendizado da equipe.

## Status atual
**Fase: concepção, design da solução e pesquisa com usuários — 2º período.**

Este repositório contém, por enquanto, a documentação inicial do projeto. As funcionalidades descritas abaixo são planejadas; ainda não há código de aplicação ou instruções de execução disponíveis neste repositório.

As atividades documentadas incluem benchmarking, definição de fluxos e regras de negócio, wireframes e preparação de uma prova de conceito para leitura via OBD-II. Foram criados três formulários de pesquisa, separados por perfil de participante.

## Objetivo da primeira versão
Permitir que a equipe demonstre um fluxo completo: identificar o veículo, consultar os dados disponíveis, registrar manutenções e apresentar avisos de manutenção preventiva compreensíveis.

| Etapa | Funcionalidade planejada | Resultado esperado |
| --- | --- | --- |
| 1 | Cadastro básico do veículo | Registrar modelo, ano, motorização e quilometragem informada pelo usuário. Começar com um veículo. |
| 2 | Leitura via OBD-II | Conectar ao leitor e identificar quais dados o conjunto veículo e leitor permite consultar. |
| 3 | Painel de monitoramento | Exibir os dados com nome, unidade e horário de atualização, indicando desconexões e informações indisponíveis. |
| 4 | Registro de manutenções | Registrar serviço realizado, data e quilometragem. |
| 5 | Plano de manutenção preventiva | Definir intervalos por tempo e quilometragem com base no manual do veículo. |
| 6 | Cálculo da próxima manutenção | Calcular o próximo vencimento a partir do último serviço e dos intervalos cadastrados. |
| 7 | Alertas no sistema | Mostrar manutenções em dia, próximas do prazo e vencidas, explicando o motivo do aviso. |
| 8 | Histórico de manutenção | Organizar e consultar os serviços realizados. |

As etapas 1 a 7 compõem o foco da primeira versão. O histórico organizado complementa esse fluxo.

### Dados do veículo e regras de manutenção
A prova de conceito deverá verificar quais informações estão realmente disponíveis no veículo e no leitor escolhidos. O projeto deve distinguir:

- **Dados lidos do veículo:** informações efetivamente obtidas via OBD-II.
- **Informações manuais:** dados complementares fornecidos pelo usuário, como quilometragem e serviços realizados.
- **Regras e estimativas:** cálculos de prazo baseados no plano de manutenção.

Não se deve presumir que o leitor fornece o odômetro ou mede o desgaste de óleo, filtros, correias e outras peças. Os avisos por tempo e quilometragem representam prazos de manutenção; não representam uma medição física do desgaste nem um diagnóstico conclusivo.

Dados simulados podem apoiar a construção das telas, desde que identificados como simulação. A leitura real deverá ser verificada antes de considerar a função principal consolidada.

### Critérios para avançar
Antes de ampliar o projeto, a equipe deverá conseguir:

- Consultar os dados disponíveis em um veículo e leitor definidos para teste.
- Exibir as informações com clareza e tratar desconexões ou dados ausentes.
- Registrar uma manutenção e calcular seu próximo prazo.
- Demonstrar os estados de manutenção em dia, próxima e vencida.
- Explicar a origem dos dados e o funcionamento dos cálculos.

Cada etapa deve funcionar no cenário combinado, tratar os erros básicos e ser compreendida pelos integrantes.

## Pesquisa com usuários
A pesquisa busca entender rotinas, dificuldades e prioridades relacionadas à manutenção de veículos. Os questionários foram adaptados para três públicos, com **12 perguntas por perfil e um campo opcional de e-mail ou telefone**.

| Público | Formulário |
| --- | --- |
| Motoristas | [Responder à pesquisa para motoristas](https://docs.google.com/forms/d/e/1FAIpQLSecQtwY7CcsVneYeLpUb22o7WoJF01vCl2S1Q-1vY_4vJIdlA/viewform) |
| Mecânicos e responsáveis por oficinas | [Responder à pesquisa para mecânicos e oficinas](https://docs.google.com/forms/d/e/1FAIpQLSdzbsopUWGsyNWx7_sLKikEYc5dHbTomh5M9kBuEw03jP_LCA/viewform) |
| Gestores de frota | [Responder à pesquisa para gestão de frota](https://docs.google.com/forms/d/e/1FAIpQLSfimafUr7tPG1X-lWHeTPNeQkPuuK4OplC5GcM9f9JfU0abHA/viewform) |

A pesquisa com oficinas e gestores de frota também ajuda a compreender possibilidades futuras. Ela não altera a prioridade atual da primeira versão.

## Possibilidades futuras
Depois de consolidar a função principal, a equipe poderá avaliar uma funcionalidade por vez:

1. Notificações no celular.
2. Cadastro de vários veículos.
3. Registro de despesas.
4. Controle de abastecimentos.
5. Relatórios e gráficos.
6. Consulta de oficinas.
7. Comparação de preços.
8. Gestão de frotas.
9. Chat e marketplace de oficinas.

Essas possibilidades não representam funcionalidades implementadas ou compromisso de entrega. Detalhes como raio de busca, atualização de preços e integração com oficinas ainda precisam ser avaliados.

## Links e artefatos
- [Central de artefatos do Gestor Veicular](https://gv.howey.com.br): portal de referência para documentação e materiais visuais.
- [Histórico de protótipos](https://github.com/marco-howey/GestorVeicular/blob/main/PROTOTIPOS.md): versões navegáveis e links do Figma.
- [Repositório no GitHub](https://github.com/marco-howey/GestorVeicular): documentação e futuras etapas de implementação.

## Tecnologias e ferramentas
| Finalidade | Ferramentas previstas na documentação |
| --- | --- |
| Prototipação e UX/UI | Figma e Canva |
| Documentação | Markdown e Microsoft Word |
| Versionamento | Git e GitHub |
| Leitura do veículo | OBD-II, com compatibilidade a verificar na prova de conceito |

A linguagem, o framework, o banco de dados e a arquitetura da aplicação ainda não estão definidos nesta documentação.

## Equipe
- Marco Antonio Alves Duarte
- Victor Gabriel Beserra Melo
- Sarah Eduarda Rodrigues de Paiva

Projeto desenvolvido para a disciplina de **Projeto Integrador do curso de Engenharia de Software**.

## Como contribuir
Nesta fase, contribuições podem ser feitas respondendo às pesquisas ou [abrindo uma issue](https://github.com/marco-howey/GestorVeicular/issues) com sugestões, dúvidas ou ajustes na documentação. Ao propor uma funcionalidade, indique o problema que ela resolve e considere a prioridade da primeira versão.
