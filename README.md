# Projeto TECHMAN

TechMan é um sistema para cadastro, exclusão e atualização de equipamentos por usuários, desenvolvido para fins de avaliação.

## Visão geral

O projeto inclui diagramas e wireframes para facilitar o entendimento da estrutura e das principais telas do sistema.

### Diagramas

![MerDer](/docs/MERXDER.png)
![DATV CLIENTE](./DOCS/DATVCLIENTE.drawio.png)
![DATV ADMIN](./DOCS/DATVADMIN.drawio.png)

### Telas principais

![Wireframe01](/docs/senha.png)
![Wireframe02](/docs/adm.png)
![Wireframe03](/docs/comentario.png)

## Como testar

1. Instale as ferramentas necessárias:

- [VS Code](https://code.visualstudio.com/)
- [XAMPP](https://www.apachefriends.org/pt_br/index.html)
- [Git](https://git-scm.com/downloads)
- [NodeJS](https://nodejs.org/pt)

2. Clone o repositório e abra no VS Code:

```bash
git clone <https://url>
cd <nomedoarquivo>
code .
```

3. Configure o backend:

```bash
cd api
npm i prisma -g
npm init -y
npm i express cors dotenv
npx prisma init --datasource-provider mysql
```

4. Configure o banco de dados MySQL no arquivo `.env`:

```bash
DATABASE_URL="mysql://root@localhost:3306/techman?schema=public&timezone=UTC"
```

5. Execute a migração inicial do banco:

```bash
npx prisma migrate dev --name init
```

6. (Opcional) Configure seu email para o Git:

```bash
git config --global user.email "seu-email@exemplo.com"
```

---
