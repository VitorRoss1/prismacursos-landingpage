<p align="center">
  <img src="assets/PrismaLogo.png" alt="PrismaCursos Logo" width="180">
</p>

<h1 align="center"><b>🌈 Prisma Cursos</b></h1>

## 📁 Estrutura

```
PrismaCursos/
├── index.html          ← Página principal (abra no navegador)
├── confirmation.html   ← Página secundária (exibe confirmação)
├── css/
│   ├── styles.css      ← Estilos 
│   └── scss/           ← Opcional: para quem quiser usar SCSS
│       ├── styles.scss
│       └── compilar-scss.sh
├── js/
│   └── cursos.js         ← JavaScript
│   └── main.js
│   └── quiz.js
├── assets/             ← Imagens e recursos
└── .gitignore
```

## 🚀 Como Rodar

Abra o `index.html` no navegador. Pronto.

> **VS Code?** Instale a extensão **Live Server** e clique em **Go Live**.

---

## 🔀 Git — Comandos Essenciais

### Primeira vez? Configure seu nome

```bash
git config --global user.name "Seu Nome"
git config --global user.email "seuemail@example.com"
```

### Clonar o repositório

```bash
git clone https://github.com/EduLoboM/Orcestra-2026.1-G04-PrismaCursos.git
cd Orcestra-2026.1-G04-PrismaCursos
```

### Criar sua branch e trabalhar nela

```bash
git checkout -b feature/minha-tarefa    # cria e já entra na branch
```

**Nomes de branch:**

| Prefixo | Uso | Exemplo |
|---------|-----|---------|
| `feature/` | Funcionalidade nova | `feature/pagina-cursos` |
| `fix/` | Correção | `fix/navbar-mobile` |
| `style/` | Visual | `style/cores-footer` |

### Salvar seu trabalho (commit + push)

```bash
git add .
git commit -m "feat: adiciona cards de cursos"
git push origin feature/minha-tarefa
```

### Tipos de commit

| Tipo | Uso | Exemplo |
|------|-----|---------|
| `feat` | Funcionalidade | `feat: cria seção de cursos` |
| `fix` | Correção | `fix: link quebrado no menu` |
| `style` | Visual | `style: ajusta cores do footer` |
| `docs` | Documentação | `docs: atualiza README` |
| `refactor` | Reorganização | `refactor: separa estilos do hero` |
| `chore` | Manutenção | `chore: atualiza gitignore` |

### Atualizar sua branch com a main

```bash
git checkout main
git pull origin main
git checkout feature/minha-tarefa
git merge main
```

### Trocar de branch

```bash
git checkout nome-da-branch
```

### Ver suas branches

```bash
git branch
```

---

## 🔃 Fluxo de Trabalho

```mermaid
graph TD
    A["🔽 git clone do repositório"] --> B["🌿 git checkout -b feature/..."]
    B --> C["✏️ Editar arquivos"]
    C --> D["💾 git add . + git commit"]
    D --> E["🚀 git push origin feature/..."]
    E --> F{"Como integrar?"}
    F -->|"Opção 1"| G["🔃 Abrir Pull Request no GitHub"]
    F -->|"Opção 2"| H["💬 Avisar o responsável pelos merges"]
    G --> I["✅ Merge na main"]
    H --> I
```

1. Faça `push` da sua branch
2. Escolha uma das opções:
   - **Opção 1 — Pull Request:** Vá no GitHub → **Compare & pull request**, descreva o que fez e peça revisão
   - **Opção 2 — Aviso direto:** Avise no grupo quem está responsável pelos merges que a sua branch está pronta
3. Aguarde o merge na `main`

> ⚠️ **Nunca dê commit direto na `main`!** Sempre use branches.

---

## ✅ Dicas Rápidas

- Commits **pequenos e frequentes** > um commit gigante
- Use tags semânticas no HTML (`<header>`, `<main>`, `<section>`, `<footer>`)
- Use as variáveis CSS do `:root` para cores e espaçamentos
- Use `const` e `let` no JS, **nunca** `var`
- **Comunique no grupo** o que está fazendo pra não duplicar trabalho

---

## 🎨 SCSS (opcional)

Se quiser usar SCSS ao invés de CSS puro, edite `css/scss/styles.scss` e compile:

```bash
# Instalar o compilador (uma vez só)
sudo apt install sass          # Linux
brew install sass/sass/sass    # Mac
choco install sass             # Windows

# Compilar
cd css/scss
./compilar-scss.sh             # compila uma vez
./compilar-scss.sh --watch     # recompila automaticamente
```

> Se não quiser usar SCSS, ignore a pasta `css/scss/` e edite o `css/styles.css` direto.

---

## 👥 Equipe

<table align="center">
  <tr>
    <td align="center">
      <a href="https://github.com/EduLoboM">
        <img src="https://github.com/EduLoboM.png" width="100px;" alt="Eduardo Lobo Moreira"/><br />
        <sub><b>Eduardo Lobo Moreira</b></sub>
      </a>
    </td>
    <td align="center">
      <a href="https://github.com/JuliaTrevizolo">
        <img src="https://github.com/JuliaTrevizolo.png" width="100px;" alt="Júlia Trevizolo"/><br />
        <sub><b>Júlia Trevizolo</b></sub>
      </a>
    </td>
    <td align="center">
      <a href="https://github.com/dev-LucasDpaula">
        <img src="https://github.com/dev-LucasDpaula.png" width="100px;" alt="Lucas Oliveira de Paula"/><br />
        <sub><b>Lucas Oliveira de Paula</b></sub>
      </a>
    </td>
  </tr>
  <tr>
    <td align="center">
      <a href="https://github.com/marianeb08">
        <img src="https://github.com/marianeb08.png" width="100px;" alt="Mariane"/><br />
        <sub><b>Mariane</b></sub>
      </a>
    </td>
    <td align="center">
      <a href="https://github.com/pedrossantoss">
        <img src="https://github.com/pedrossantoss.png" width="100px;" alt="Pedro dos Santos"/><br />
        <sub><b>Pedro dos Santos</b></sub>
      </a>
    </td>
    <td align="center">
      <a href="https://github.com/VitorRoss1">
        <img src="https://github.com/VitorRoss1.png" width="100px;" alt="Vitor Rossi"/><br />
        <sub><b>Vitor Rossi</b></sub>
      </a>
    </td>
  </tr>
</table>

---

## 🎯 Quiz de Escolha de Curso (Gamificação 1)
Para auxiliar o usuário a descobrir qual curso se alinha melhor com seu perfil e interesses, foi implementado um questionário interativo e dinâmico:
* **Fluxo de Navegação:** Composto por **3 perguntas consecutivas** (Nível de Experiência, Tempo Disponível e Área de Interesse), com transições suaves via JavaScript.
* **Barra de Progresso:** Uma barra visual dinâmica indica o avanço do usuário ao longo das etapas (33.3%, 66.6% e 100%).
* **Sistema de Recomendação:** Com base na resposta final sobre a área de preferência, a aplicação sugere um curso específico e exibe a imagem correspondente:
  * 🖥️ **Tecnologia** ➡️ Recomendação do curso de **DevOps** (`assets/quiz/resultado-devops.png`).
  * 🎨 **Design** ➡️ Recomendação do curso de **Design 3D** (`assets/quiz/resultado-design3d.png`).
  * 📈 **Gestão** ➡️ Recomendação do curso de **Gestão Pessoal** (`assets/quiz/resultado-gestao.png`).

---

## 🏷️ Sistema de Desconto Progressivo (Gamificação 2)
Para incentivar a exploração das diferentes seções da página e aumentar o engajamento, criamos uma mecânica de acúmulo de desconto baseada nas interações do usuário:
* **Gatilho de Ativação:** O usuário inicia com **5%** de desconto e ganha **+5% de desconto acumulado** a cada primeira visita/clique em links de navegação específicos:
  * `Cursos`
  * `Quem Somos`
  * `Contato`

---

## 🧪 Validação de Formulário
Garante a integridade e consistência das informações enviadas pelo formulário de cadastro através de validações em tempo real via JavaScript:

<table align="center">
  <thead>
    <tr>
      <th>Campo</th>
      <th>Regra de Validação</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td><b>Todos os campos</b></td>
      <td>Preenchimento obrigatório (Nome, E-mail, Celular, Curso, Assunto).</td>
    </tr>
    <tr>
      <td><b>E-mail</b></td>
      <td>Presença obrigatória de formato válido contendo os caracteres <code>@</code> e <code>.</code></td>
    </tr>
    <tr>
      <td><b>Celular</b></td>
      <td>Deve conter uma sequência numérica estrita de <b>10 ou 11 dígitos</b> (qualquer caractere não numérico, como parênteses ou traços, é ignorado na contagem).</td>
    </tr>
</table>
