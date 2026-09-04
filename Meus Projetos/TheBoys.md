# 🦸‍♂️ TheBoys

Este foi meu primeiro grande projeto na faculdade. Ele é um programa que simula um mundo com heróis, bases e missões acontecendo ao mesmo tempo. Tudo funciona de forma automática através de uma lista de eventos que decide o que acontece e quando acontece. A simulação roda sozinha e termina quando um evento final é alcançado.

---

## 🚀 Principais Funcionalidades

* **Execução pelo terminal:** Você só precisa executar o projeto e a simulação acontece sozinha, sem precisar que o usuário fique digitando comandos.
* **Relatório estatístico:** Assim que o mundo acaba, o programa exibe na tela várias estatísticas e dados sobre o que aconteceu durante a simulação.   

---

## 🛠️ Tecnologias e Ferramentas Utilizadas

* **Linguagem C:** Para construir toda a lógica e regras do simulador.
* **Make (Makefile):** Disponibilizado pelos professores para facilitar a compilação e testes.
* **Valgrind:** Para testes de vazamentos de memória.

---

## 🧠 Desafios Técnicos e Aprendizados

### Organização do projeto
* **O problema:** Por ser meu primeiro projeto, foi difícil entender como dividir cada parte para evitar que ficassem em um só arquivo
* **A solução:** Primeiro analisei o PDF do enunciado e busquei dividir cada Etapa em um arquivo separado. Depois conversando com o professor, decidi também deixar separado funções auxiliares. Resolver esse problema me ajudou a entender as vantagens e como modularizar um programa.

### Erros de ponteiro/memória
* **O problema:** Ainda estava no processo de entender o uso de ponteiros e como evitar vazamentos de memória.
* **A solução:** A forma que resolvi foi durante a escrita do código redobrar o cuidado quando lidando com ponteiros e alocações de memória. Fora os diversos testes para garantir que não havia vazamentos de memória usando Valgrind. Esse problema me ajudou a entender melhor como ponteiros funcionam e também melhorou meu entendimento do C.