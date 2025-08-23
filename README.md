# Angular Directives - Projeto de Estudo

Este projeto foi desenvolvido como parte do estudo de **Directives** em Angular.  
O objetivo é explorar como criar e aplicar **directives personalizadas**, além de praticar o uso de *standalone components*.

## 🚀 Tecnologias
- Angular
- TypeScript
- HTML & CSS

## 📌 Diretivas Implementadas

### 1. `appLog`
- **Tipo**: Attribute Directive
- **Uso**: `<button appLog>Click me</button>`
- **Função**:  
  - Registra no console quando o elemento é clicado.  
  - Exibe no console o próprio elemento DOM.

---

### 2. `appSafeLink`
- **Tipo**: Attribute Directive (aplicada a links)
- **Uso**: `<a href="https://angular.io" appSafeLink="docs">Angular Docs</a>`
- **Função**:  
  - Pergunta ao usuário se deseja realmente sair da aplicação.  
  - Caso afirmativo, adiciona um query param `?from=docs` ao link.  
  - Incorpora a `LogDirective` como *host directive*.

---

### 3. `appAuth`
- **Tipo**: Structural Directive
- **Uso**:  
  ```html
  <div *appAuth="'admin'">
    Conteúdo visível apenas para administradores
  </div>
  ```
- **Função**:  
  - Exibe ou esconde elementos com base na permissão do usuário.
  - Faz integração com AuthService para verificar permissões.
 
## ▶️ Executando o Projeto

```bash
# Instalar dependências
npm install

# Rodar servidor de desenvolvimento
ng serve

# Acessar no navegador
http://localhost:4200/
```

## 🎯 Objetivo

O propósito deste projeto não é ser uma aplicação completa, mas sim um **laboratório de aprendizado**, focado na criação e uso de **directives em Angular**.
