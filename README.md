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

> Breve descrição de uma linha sobre o que é o site (ex: Plataforma de agendamento para barbearias).

---

## 💡 Sobre o Projeto

### Ideia
Descreva aqui o conceito central do site. Qual problema ele resolve? Como ele funciona na prática?

### Objetivos
* **Geral:** Qual o grande objetivo do site?
* **Específicos:**
    * Objetivo específico 1 (ex: Permitir cadastro de usuários).
    * Objetivo específico 2 (ex: Integrar com API de pagamento).
    * Objetivo específico 3 (ex: Ter um design 100% responsivo).

### Justificativa
Por que construir este site agora? Explique o valor do projeto, seja para resolver uma dor real do mercado, para portfólio pessoal ou para fins acadêmicos.

---

## 🖼️ Project Model Canvas

Abaixo está a estruturação visual do modelo de negócio/projeto.

| 🎯 Proposição de Valor | 👥 Segmentos de Clientes | 📢 Canais | 🤝 Relacionamento |
| :--- | :--- | :--- | :--- |
| O que o site oferece de único? | Quem vai usar o site? | Como os usuários acharão o site? | Como reter os usuários? |

| 🛠️ Atividades-Chave | 🔑 Recursos-Chave | 🤝 Parceiros-Chave |
| :--- | :--- | :--- |
| O que precisa ser feito? (Design, Dev) | O que é necessário? (Hospedagem, APIs) | Quem pode ajudar? (Gateway de pagamento) |

| 💶 Estrutura de Custos | 💰 Fontes de Receita |
| :--- | :--- |
| Domínio, APIs pagas, tempo de dev. | Assinaturas, anúncios, doações, etc. |

---

## 🏗️ Infraestrutura e Tecnologias

Ferramentas e tecnologias utilizadas no desenvolvimento do site:

* **Frontend:** React.js / Next.js / HTML & CSS
* **Estilização:** Tailwind CSS / Styled Components
* **Banco de Dados:** PostgreSQL / MongoDB / Supabase
* **Hospedagem:** Vercel

---

## 📅 Cronograma (ProjectLibre)

O planejamento do projeto foi estruturado no **ProjectLibre**. Abaixo estão as fases e os marcos do desenvolvimento:

* **Fase 1: Concepção e Design** (📅 DD/MM a DD/MM)
    * [x] Definição de Requisitos
    * [ ] Wireframes e UI Design no Figma
* **Fase 2: Desenvolvimento** (📅 DD/MM a DD/MM)
    * [ ] Configuração do ambiente e Banco de Dados
    * [ ] Desenvolvimento do Frontend
    * [ ] Integração de APIs
* **Fase 3: Testes e Deploy** (📅 DD/MM a DD/MM)
    * [ ] Homologação e correção de bugs
    * [ ] Deploy em produção

> 💡 *Dica: Você pode tirar um print do gráfico de Gantt do ProjectLibre, salvar a imagem na pasta do projeto e linká-la aqui usando o código: `![Cronograma ProjectLibre](./caminho-da-imagem.png)`.*

---

## 🚀 Deploy e Link Oficial

O deploy contínuo do projeto é feito através da **Vercel**. Você pode acessar a versão estável do site clicando no link abaixo:

🔗 **[Acesse o Site Aqui](https://seu-link-aqui.vercel.app)**

---

## 🛠️ Como rodar o projeto localmente

```bash
# 1. Clone o repositório
git clone [https://github.com/seu-usuario/seu-repositorio.git](https://github.com/seu-usuario/seu-repositorio.git)

# 2. Acesse a pasta
cd seu-repositorio

# 3. Instale as dependências
npm install

# 4. Rode o projeto
npm run dev
