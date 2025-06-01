# Projeto ELLP - Ensino Lúdico de Lógica e Programação  
**Plataforma de Gestão de Voluntários e Certificados para Extensão Universitária**

---

## **Alunos**
- Douglas Silva Ribeiro - 2209039
- Mateus Eduardo - 2145308
- Vitor Kenji Moribe Tominaga - 1805967

---

##**Trello**
https://trello.com/invite/b/68229385354718db1d2f6bed/ATTI4139b833b420c838fcca1acb1f49a18645742AD6/oficina-2

---

## **Objetivo**  
Desenvolver um sistema integrado para gerenciar alunos voluntários e atividades do projeto ELLP da UTFPR, facilitando a organização de oficinas educativas e a emissão automatizada de certificados. O projeto visa promover o ensino de lógica e programação para comunidades de forma lúdica, garantindo eficiência administrativa e transparência nas atividades de extensão.

---

## **Funcionalidades**  

- **Cadastro de Alunos**:  
  - Campos obrigatórios: nome, e-mail institucional, curso, R.A.  
  - Validação de duplicidade (e-mail/matrícula).  
  - **Edição de Dados**: Atualização de informações pessoais.  
  - **Exclusão de Aluno**: Confirmação via modal para evitar remoção acidental.  

- **Cadastro de Oficinas**: 
  - Campos: título, descrição, data, local, carga horária, aluno voluntário responsável.  
  - **Edição de Oficinas**: Atualizar informações.  
  - **Exclusão de Oficinas**: Verificação de certificados vinculados antes da exclusão.  

- **Geração de PDF**:  
  - Template personalizável com logo da UTFPR, dados do aluno, atividades realizadas e carga horária total.  

---

## **Tecnologias Utilizadas**  

| **Front-end**       | **Back-end**       | **Banco de Dados** | **Testes**          |  
|----------------------|--------------------|---------------------|---------------------|  
| Next.js              | Node.js + Express             | SQLite              | Jest (unitários/integração) |  
| Tailwind CSS         | Não definido (geração de PDF) |     | Cypress (E2E)       |  

---

## **Estratégia de Automação de Testes do Sistema**

| Tipo de Teste       | Exemplos de Cenários                          | Ferramenta         |  
|---------------------|-----------------------------------------------|--------------------|  
| **Testes Unitários** | Validação de funções de cálculo de carga horária. | Jest               |  
| **Testes de API**    | CRUD de alunos/oficinas via endpoints da API. | Jest + Supertest   |  
| **Testes E2E**       | Fluxo completo: entrada no sistema → cadastro → login → cadastro de oficina → oficina → certificado. | Cypress            |
---

## **Arquitetura do Sistema**

![Descrição da Imagem](https://github.com/OficinaDeIntegracao2/artefatos/blob/main/arquitetura.png?raw=true)
