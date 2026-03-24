Requisitos para persistência no Firebase Funcionar:

1. O campo comentário está com check de tamanho > 10 posições.

2. No firebase regras liberar escrita:
   rules_version = '2';
service cloud.firestore {
  match /databases/{database}/documents {
    match /contacts/{docId} {
      allow create: if true;
    }
  }
}

3. No vercel as variáveis de ambiente devem estar exatamente assim:
<img width="417" height="753" alt="image" src="https://github.com/user-attachments/assets/5fadaa0d-f4f3-438d-a69d-6551bf55a134" />

Exemplo de README de um WEBSITE
# 🚀 Nome do Projeto

> Uma linha de descrição curta e impactante sobre o que é o site.

---

## 📌 Sumário

1. [💡 Sobre o Projeto](#-sobre-o-projeto)
    * [Ideia](#ideia)
    * [Objetivos](#objetivos)
    * [Justificativa](#justificativa)
2. [🖼️ Project Model Canvas](#️-project-model-canvas)
3. [🏗️ Infraestrutura](#️-infraestrutura)
4. [📅 Cronograma (ProjectLibre)](#-cronograma-projectlibre)
5. [🚀 Deploy e Acesso](#-deploy-e-acesso)

---

## 💡 Sobre o Projeto

### Ideia
Descreva aqui o conceito central do site. Qual problema ele resolve e qual é a proposta principal?

### Objetivos
* **Geral:** O propósito maior do site.
* **Específicos:**
    * Objetivo específico 1.
    * Objetivo específico 2.
    * Objetivo específico 3.

### Justificativa
Por que este site está sendo construído? Explique o valor do projeto para o mercado, para a sociedade ou para o seu aprendizado profissional.

---

## 🖼️ Project Model Canvas

Abaixo está o mapeamento visual do modelo do projeto.

| 🎯 Proposição de Valor | 👥 Segmentos de Clientes | 📢 Canais | 🤝 Relacionamento |
| :--- | :--- | :--- | :--- |
| O que o site entrega de valor? | Quem são os usuários? | Como chegarão ao site? | Como fidelizar o usuário? |

| 🛠️ Atividades-Chave | 🔑 Recursos-Chave | 🤝 Parceiros-Chave |
| :--- | :--- | :--- |
| Desenvolvimento, Design... | Servidores, APIs... | Fornecedores, gateways... |

| 💶 Estrutura de Custos | 💰 Fontes de Receita |
| :--- | :--- |
| Custos de hospedagem, domínio... | Vendas, planos, doações... |

---

## 🏗️ Infraestrutura

Tecnologias e ferramentas utilizadas para tirar o site do papel:

* **Frontend:** [Ex: React, Next.js, HTML5/CSS3]
* **Estilização:** [Ex: Tailwind CSS, Bootstrap]
* **Banco de Dados:** [Ex: PostgreSQL, Supabase, Firebase]
* **Gestão do Projeto:** ProjectLibre
* **Hospedagem / Cloud:** Vercel

---

## 📅 Cronograma (ProjectLibre)

Planejamento e controle de tempo extraídos do software de gestão ProjectLibre.

* **Fase 1: Concepção & Design** * [ ] Definição de escopo e requisitos
    * [ ] Wireframes e Layouts
* **Fase 2: Desenvolvimento** * [ ] Estruturação do banco de dados
    * [ ] Codificação do frontend e backend
* **Fase 3: Testes e Lançamento** * [ ] Homologação e correção de bugs
    * [ ] Lançamento oficial

> 📷 **Dica visual:** Para exibir o Gráfico de Gantt do ProjectLibre, salve um print na pasta do seu projeto e chame-o aqui usando: `![Gráfico de Gantt](./caminho-da-imagem-do-cronograma.png)`

---

## 🚀 Deploy e Acesso

O site está publicado e disponível em ambiente de produção através da infraestrutura da **Vercel**.

🔗 **Clique para acessar:** [https://seu-site.vercel.app](https://seu-site.vercel.app)

---

Feito com 💜 por [Seu Nome](https://github.com/seu-usuario).
npm run dev
