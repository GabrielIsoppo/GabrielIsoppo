# 🏥 Rounds-Uti

Aplicativo focado em facilitar a rotina de um médico que trabalha em múltiplos hospitais e Unidades de Terapia Intensiva (UTIs). O projeto resolve o problema de organização e centralização de dados de pacientes, evitando desgaste com múltiplos sistemas, um para cada hospital.


## 🚀 Principais Funcionalidades

* **Modo Offline total:** Todo o fluxo do aplicativo funciona sem internet. O médico pode iniciar o plantão, cadastrar pacientes, registrar novos hospitais/UTIs e dar altas ou óbitos de forma 100% offline.
* **Sincronização inteligente (Sync):** Assim que o dispositivo detecta uma conexão com a internet, os dados salvos localmente são sincronizados automaticamente com o servidor (back-end), mantendo as informações seguras.
* **Gerenciamento Multi-Hospitalar:** Permite alternar facilmente entre diferentes hospitais e UTIs, organizando o painel de pacientes de acordo com o local de atendimento do dia.


## 🛠️ Tecnologias e Ferramentas Utilizadas

* **Front-end / Mobile:** React Native, TypeScript, Expo
* **Back-end & API:** PHP, Laravel
* **Gerenciamento de Estado & Cache:** React Query (TanStack Query) e Context API
* **Armazenamento Seguro Local:** MMKV (criptografia de dados sensíveis dos pacientes) e AsyncStorage
* **Ferramentas & Infraestrutura:** Git, GitHub, Docker


## 👥 Minha Contribuição no Projeto

Como o projeto foi desenvolvido em equipe, foquei meus esforços na engenharia do aplicativo **Mobile**, atuando nas seguintes frentes:
* **Desenvolvimento de Telas:** Projetei e implementei componentes de interface utilizando React Native, TypeScript e Expo, focando na experiência de uso do médico.
* **Resolução de Bugs (Debug):** Fiquei responsável por corrigir bugs de lógica do aplicativo e inconsistências no fluxo do modo offline.
* **Ajustes de Sincronização:** Trabalhei na manutenção e refatoração da comunicação entre o armazenamento seguro local (MMKV/AsyncStorage) e as regras de cache do React Query para garantir que os dados não fossem perdidos.


## 🧠 Desafios Técnicos e Aprendizados

### Criação de componente de seleção customizado (Dropdown)
* **O problema:** Necessidade de um componente de seleção de opções que se integrasse ao visual do aplicativo, mas mantendo a usabilidade nativa.
* **A solução:** Criei um componente personalizado combinando um campo de texto estilizado com um gatilho de clique TouchableOpacity. Ao interagir com o campo, o estado de visibilidade é alterado, exibindo uma de opções logo abaixo. Isso garantiu um componente leve, flexível e totalmente controlado.

### Gerenciamento de dados na tela de diagnóstico
* **O problema:** A tela de diagnóstico precisava lidar com campos fixos de dados e, ao mesmo tempo, permitir que o médico adicionasse perguntas e observações opcionais de forma dinâmica, que existiam apenas no escopo do mobile antes do envio.
* **A solução:** Em vez de poluir a tela principal com dezenas de variáveis de estado soltas, centralizei o fluxo de criação das perguntas opcionais em uma estrutura de dados dinâmica dentro de um componente de modal. Isso reduziu a complexidade da criação da pergunta, injetando o novo dado na lista principal apenas quando o médico confirmava a ação.

### Sincronização e fluxo do Modo Offline
* **O problema:** Garantir que o médico possa usar o aplicativo normalmente sem internet e que os dados sejam salvos na ordem certa para o servidor quando a conexão voltar.
* **A solução:** Atualmente, estamos trabalhando na correção dessa comunicação com o back-end, focando em criar uma fila de requisições eficiente. O objetivo é fazer com que o aplicativo guarde as ações feitas offline e as envie uma por uma assim que houver sinal, garantindo que nenhum dado do paciente seja perdido ou salvo de forma errada.


👥 Projeto desenvolvido em equipe.
💻 Contribuições mobile e documentação por **Gabriel de Souza Isoppo** — Entre em contato no [LinkedIn](https://www.linkedin.com/in/gabriel-de-souza-isoppo-a7630739b/).

##### 🤖 *Nota: Esta documentação utilizou inteligência artificial estritamente para a estruturação do template (Markdown) e revisão ortográfica das descrições autorais.*