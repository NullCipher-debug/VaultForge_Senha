# 🔐 VaultForge - Gerador de Senhas Inteligente

> Um gerador de senhas moderno, seguro e auditado. Não apenas cria senhas, mas corrige e confere cada uma.

![Badge de Status](https://img.shields.io/badge/status-concluído-brightgreen)
![Badge de Licença](https://img.shields.io/badge/licença-MIT-blue)
![Badge de Tecnologia](https://img.shields.io/badge/feito%20com-Next.js%20%26%20TypeScript-black)

### [➡️ Ver Demonstração Ao Vivo](https://darkseagreen-wasp-558967.hostingersite.com/senha/)

![Preview do Projeto](https://via.placeholder.com/800x400?text=<img width="824" height="842" alt="Captura de tela 2026-10-09 000031" src="https://github.com/user-attachments/assets/50a70457-584e-46f2-b4f3-0b9ddd2ad886" />)

---

### 📖 Sobre o Projeto

O VaultForge nasceu para resolver um problema simples: geradores de senha comuns criam senhas como `123456` se você pedir errado.

Este projeto implementa um **sistema de Correção e Conferência em 5 camadas**, que garante que toda senha gerada seja realmente forte, usável e segura contra vazamentos.

Este projeto foi feito para estudar: manipulação de DOM, entropia, APIs de segurança e boas práticas da web moderna.

### ✨ Funcionalidades

- [x] **Geração Multi-Modo:**
    - Aleatória Forte (16-128 caracteres)
    - Passphrase (estilo `corvo-café-trilha-neblina`)
    - PIN e Memorizável
- [x] **Medidor de Força em Tempo Real:** Score de 0-100 + tempo para quebrar
- [x] **Auditoria de Segurança:**
    - Detecta padrões de teclado (qwerty, 1234)
    - Verifica em vazamentos conhecidos (HaveIBeenPwned API)
    - Calcula entropia real
- [x] **Correção Inteligente:** Se o usuário pedir uma senha fraca, o app sugere automaticamente a versão segura
- [x] **Copiar com 1 clique e histórico temporário**

### 🛠️ Tecnologias Usadas

- **Frontend:** Next.js 14, TypeScript, Tailwind CSS
- **Lógica de Segurança:** Web Crypto API (`crypto.getRandomValues`)
- **Ícones:** Lucide React
- **Deploy:** Vercel

### 🚀 Como Rodar Localmente

Se alguém quiser rodar seu projeto, é aqui que você ensina.

```bash
# 1. Clone o repositório
git clone https://github.com/seu-usuario/vaultforge.git

# 2. Entre na pasta
cd vaultforge

# 3. Instale as dependências
npm install

# 4. Rode o projeto
npm run dev


🔒 Como funciona a Conferência?
Toda senha passa por isso antes de ser mostrada:

Sintática: Tem o tamanho certo?
Entropia: Tem pelo menos 60 bits de força?
Política: Não é senha123 ou seu nome?
Usabilidade: Não tem caractere que quebra em sites?
Vazamento: Já apareceu em algum vazamento?
🗺️ Próximos Passos (Roadmap)
 Adicionar modo de compartilhamento seguro com link que expira
 PWA para funcionar offline
 Extensão para o Chrome
👨‍💻 Autor
Feito por Seu Nome
Meu LinkedIn: linkedin.com/in/seu-perfil

📝 Licença
Este projeto está sob a licença MIT.
