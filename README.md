Requisitos da Aplicação

# RF

- [x] O usuário deve poder criar uma nova transação
- [x] O usuário deve poder obter um resumo da sua conta
- [x] O usuário deve poder listar todas as transações que já ocorreram
- [x] O usuário deve poder visualizar uma transação única

# RN

Condições, coisas que podem acontecer, que a nossa aplicação vai validar

- [x] A transação pode ser do tipo crédito, que somará ao valor total, ou débito, que subtrairá do valor total
- [x] Deve ser possível identificarmos os usuários entre as requisições (não teremos autenticação ainda)
- [x] O usuário só pode visualizar transações o qual ele criou

# RNF

Aqui podemos entrar na parte técnica, para alcançar a lista acima.

# Tipos de Teste

- Unitários => Testar apenas uma unidade da sua aplicação, uma pequena parte, de forma totalmente isolada, temos em maior quantidade
- Integração => Quando testamos a comunicação entre duas ou mais unidades
- End to End (Ponta a Ponta) => Testes simulam um usuário operando na nossa aplicação (um fluxo completo) // No Back-end, o usuário é o front, então devemos simular chamadas HTTP, websockets, e outras camadas que se comunicam com o front

# Pirâmides de Testes

Cada teste tem uma dificuldade e suas exigências, o primeiro tipo de teste a ser implementado, deveria ser:

Testes E2E, porque eles não dependem de nenhuma tecnologia // São lentos, devem se ter poucos
Integração, devem ser ter um pouco mais
E devemos ter muitos testes unitários

Podemos usar Jest.js.io, ou Vitest

Vitest usa por baixo dos panos o esbuild, mesma ferramentas por trás do tsx, e do vite, é um builder muito rápido de ts para js

Teste é composto por enunciado, operação e a validação
