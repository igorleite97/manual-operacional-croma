echo "# Manual Operacional Interativo — Espaco Croma

Sistema de documentação operacional interativa desenvolvido como projeto de consultoria organizacional.

## Sobre o projeto
Manuais operacionais em formato HTML interativo para os setores internos de uma empresa B2B de tecnologia. Cada setor possui fluxogramas clicáveis, checklists interativos, glossário e espaços para vídeos tutoriais.

## Setores documentados
- Compras (Comercial Privado)
- Logística e Estoque
- Financeiro
- Comercial
- E-commerce
- Outsourcing (Locação)

## Stack
HTML · CSS · JavaScript vanilla — sem frameworks, sem dependências externas.

## Aviso
Todos os dados de clientes, fornecedores e colaboradores presentes nos arquivos são fictícios ou anonimizados. Este repositório representa apenas a estrutura e a metodologia do sistema, não dados reais da empresa contratante.

## Autor
Igor Leite — Consultor Organizacional & Analista de Tecnologia
Transição para Cybersecurity (Offensive Security / Pentest)" > README.md

git add README.md
git commit -m "docs: adiciona README do projeto"
git push
```

**2. Renomear o site no Netlify** — o nome `mellifluous-bublanina` é gerado aleatoriamente. Para ter um link mais profissional: no painel do Netlify clique em `Site configuration` → `Site details` → `Change site name` → coloque `manual-croma` ou `manual-operacional-croma`. O link vira `manual-croma.netlify.app`.

**3. Conectar GitHub ao Netlify** — isso é opcional mas poderoso: sempre que você fizer `git push`, o Netlify atualiza o site automaticamente. No painel do Netlify clique em `Project configuration` → `Build & deploy` → `Link repository` → selecione o repositório `manual-operacional-croma`. A partir daí `git push = site atualizado`.

---

Com isso o pipeline completo fica assim:
```
Você edita o .html no VS Code
        ↓
git add . && git commit -m "..." && git push
        ↓
Netlify atualiza automaticamente em ~10 segundos
        ↓
Link no OptiWork Papers reflete a versão mais recente