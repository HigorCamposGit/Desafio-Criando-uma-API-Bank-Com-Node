# Desafio: Criando uma API de Bank com Node.js e TypeScript

Projeto desenvolvido como parte dos desafios práticos da **Formação TypeScript Fullstack Developer** com Node.js, Express e TypeScript da Digital Innovation One (DIO).

## 🚀 O que foi feito

Neste projeto, construímos e evoluímos uma API backend para gerenciamento de usuários (CRUD), aplicando padrões de arquitetura limpa (separação entre Controllers e Services), tipagem estricta com TypeScript e testes unitários robustos com Jest.

### Principais Funcionalidades e Implementações:
* **Criação de Usuários (`POST /user`)**: Com validação obrigatória dos campos `name` e `email`.
* **Listagem de Usuários (`GET /user`)**: Retorna todos os usuários cadastrados no banco de dados em memória (`db`).
* **Exclusão de Usuários (`DELETE /user`)**: Lógica implementada no serviço e exposta via controller e rotas para remoção segura por nome.
* **Testes Unitários (`Jest`)**: Cobertura completa testando cenários de sucesso, validações de campos obrigatórios e chamadas de métodos do serviço com mocks isolados.

---

## 🛠️ Desafios Concluídos

1. **Testes Unitários Pendentes no Controller**:
   * Validação da resposta de erro (`400 Bad Request`) caso o usuário não informe o `name`.
   * Verificação se a função `getAllUsers` está sendo chamada corretamente.
2. **Validação para o Campo E-mail**:
   * Implementação de regra no `UserController` bloqueando a criação caso o e-mail não seja informado.
   * Criação do respectivo teste unitário para validar o cenário de erro de e-mail ausente.
3. **Refatoração e Implementação da Rota de Deleção**:
   * Desenvolvimento do método `deleteUser` no `UserService`.
   * Integração do método no `UserController` com validações.
   * Atualização do arquivo de rotas (`routes.ts`) e criação do teste unitário de exclusão.

---

## 💻 Tecnologias Utilizadas

* **Node.js**
* **TypeScript**
* **Express**
* **Jest** (Testes unitários)
* **Ts-node-dev**

---

## 👥 Créditos e Agradecimentos

* **Instrutora**: [Nathally Souza (@nathsouzadev)](https://github.com/nathsouzadev)
* **Repositório Base**: [digitalinnovationone/desafio04-ts](https://github.com/digitalinnovationone/desafio04-ts)
* **Desafio realizado por**: [Higor de Campos](https://github.com/HigorCamposGit)

--- 

## 🤝 Conecte-se Comigo

<p align="center">
  <img src="https://github.com/HigorCamposGit.png" width="100px" style="border-radius: 50%;" alt="Foto de Higor de Campos" /><br />
  <b>Projeto atualizado por:</b> <a href="https://github.com/HigorCamposGit">Higor de Campos</a>
</p>

---
