# 🏎️ iRacer — As melhores ligas e corridas do jogo ofical da F1 na palma da sua mão! 🔥

|    Tela de Login     |     Lista de corridas      |      Resultados da Corrida       |      Criação de Corrida      |
| :------------------: | :------------------------: | :------------------------------: | :--------------------------: |
| ![](./img/login.png) | ![](./img/racing-list.png) | ![](./img/edit-race-results.png) | ![](./img/race-creation.png) |

Olá, meu caro amigo(a)! Meu nome é Felipe Rocha, e você está presenciando o projeto mais ambicioso (e incrível haha!) que eu tenho atualmente — o iRacer.

Eu sou apaixonado por automobilismo, especialmente por F1, por videogames e, claro, por programação. Nele eu achei uma forma de unir essas três paixões em algo extraordinário.

## O que é o iRacer?

Antes de falar o que ele é, vou explicar pra você o problema que ele resolve. No jogo da F1, há campeonatos. Estes campeonatos são gerenciados por pessoas, que precisam, de corrida em corrida, guardar as suas informações (quem venceu, pódio, volta mais rápida etc), e elas geralmente fazem isso no Excel. Elas também precisam, após as corridas, atualizar a tabela geral da liga.

Este é um processo que é beeeem chato, e que desestimula as pessoas a criarem os seus próprios campeonatos, uma vez que elas precisam dedicar um bom tempo para atualizar os seus dados corretamente — e essa dificuldade aumenta exponencialmente com o número de participantes.

Maaas, para a felicidade de todos (rs) eu criei o iRacer. Ele calcula toda a tabela geral da liga automaticamente se baseando nos resultados das corridas, ou seja, ele tira uma camada de complexidade muito grande das costas do dono do campeonato — que é o gerenciamento e condensamento dos resultados das corridas. Além disso, ele guarda todas as estatísticas de cada piloto em seu próprio perfil. Por exemplo, se eu venci uma corrida e fiz a volta mais rápida, eu ganho +1 vitória e +1 volta mais rápida em meu perfil de piloto:

|     Detalhes da Corrida     |       Perfil de Piloto        |
| :-------------------------: | :---------------------------: |
| ![](./img/race-details.png) | ![](./img/driver-profile.png) |

## Processo de Criação e Finalização de uma Corrida 🏁

O iRacer suporta tanto a criação de ligas, como mencionei anteriormente, quanto a de corridas isoladas. A primeira funcionalidade ainda está em desenvolvimento, mas logo deve ser concluída!

Portanto, vamos ver como funciona o processo de criação de uma corrida.

### Primeiro passo: Definição de circuito e configurações ⚙️

|      Seleção de Circuito       |    Configurações da Corrida    |    Configurações da Corrida    |     Criação de Corrida (sucesso)     |
| :----------------------------: | :----------------------------: | :----------------------------: | :----------------------------------: |
| ![](./img/track-selection.png) | ![](./img/race-settings-1.png) | ![](./img/race-settings-2.png) | ![](./img/race-creation-success.png) |

### Segundo passo: Entrada de participantes por meio do Código de Convite 🔑

| Entrada na Corrida (Cód. de Convite) | Solicitação de Entrada na Corrida |
| :----------------------------------: | :-------------------------------: |
|      ![](./img/race-entry.png)       |    ![](./img/pendent-race.png)    |

### Terceiro passo: Aprovação de pilotos pendentes ⌛

|      Corridas Pendentes      |       Pilotos Pendentes        | Corrida Após Aprovação de Piloto (iFMRocha) |
| :--------------------------: | :----------------------------: | :-----------------------------------------: |
| ![](./img/pendent-races.png) | ![](./img/pendent-drivers.png) |  ![](./img/race-after-driver-approval.png)  |

### Quarto passo: Finalização da corrida ✔️

|          Opções da Corrida          | Confirmação de Finalização da Corrida |       Finalização da Corrida       |
| :---------------------------------: | :-----------------------------------: | :--------------------------------: |
| ![](./img/race-details-options.png) |  ![](./img/finish-race-confirm.png)   | ![](./img/finish-race-success.png) |

### Quinto passo: Edição dos resultados da corrida 📝

|    Opções da Corrida (finalizada)    |       Edição dos Resultados        | Atribuição de Volta Mais Rápida e/ou Pole Position |        Salvamento das Alterações         |
| :----------------------------------: | :--------------------------------: | :------------------------------------------------: | :--------------------------------------: |
| ![](./img/finished-race-options.png) | ![](./img/edit-race-results-2.png) |        ![](./img/pole-and-fastest-lap.png)         | ![](./img/race-results-after-saving.png) |

Agora, os resultados da corrida — grid final, piloto que fez a volta mais rápida e a pole position — foram salvos. Muito simples, não é? E o melhor de tudo: nada de Excel!
Em um futuro próximo, onde as ligas estaraão implementadas, esses resultados serão condensados e a tabela do campeonato será construída automaticamente.

## Funcionalidades Implementadas (Done ✅)

✅ Autenticação (email/senha e Google OAuth)

✅ Criação e edição de corridas

✅ Entrada em corridas (como piloto titular ou reserva)

✅ Captura dos resultados de uma corrida (grid final, pódio, volta mais rápida e pole position)

✅ Registro das estatísticas do usuário (títulos, vitórias, pódios, pole positions e voltas mais rápidas) em seu Perfil de Piloto

✅ Validações em todos os formulários implementados até agora

## Funcionalidades a Serem Implementadas (To Do 🚀)

🚀 Criação e edição de ligas

🚀 Geração de resultados de uma liga (campeonato de construtores e de pilotos) baseando-se em suas corridas

## Tecnologias Utilizadas 🛠

**Front-end:** React Native, Expo, Apollo Client (com GraphQL), TypeScript, Styled Components.

**Back-end:** NestJS, GraphQL, TypeScript, Docker, Jest & SuperTest (E2E tests).

**DevOps:**: CI/CD para testar, buildar e fazer o deploy do back-end para a AWS ECS (com Docker; ECR) e/ou Heroku; CI/CD para testar, buildar e fazer deploy do front-end para o Expo (expo publish).
