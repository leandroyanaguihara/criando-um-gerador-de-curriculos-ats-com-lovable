# MatchCV — Matchmaking Inteligente de Vagas e Currículos ATS

<p align="center">
  <strong>Encontre oportunidades compatíveis com seu perfil e prepare currículos personalizados para cada vaga.</strong>
</p>

<p align="center">
  <a href="#-sobre-o-projeto">Sobre</a> •
  <a href="#-funcionalidades">Funcionalidades</a> •
  <a href="#-como-funciona">Como funciona</a> •
  <a href="#-desenvolvimento-com-lovable">Desenvolvimento</a> •
  <a href="#-mega-prompt">Mega Prompt</a>
</p>

---

## 📌 Sobre o projeto

O **MatchCV** é uma aplicação web desenvolvida para facilitar a busca por oportunidades profissionais e melhorar a apresentação de candidatos em processos seletivos.

Um dos principais problemas enfrentados por quem procura emprego é a dificuldade de identificar vagas realmente compatíveis com suas experiências e competências. Além disso, muitas empresas utilizam sistemas ATS (*Applicant Tracking Systems*) para realizar a triagem inicial de currículos, tornando importante a utilização de documentos bem estruturados e alinhados aos requisitos das oportunidades.

A proposta do MatchCV é unir essas duas necessidades em uma única plataforma.

Por meio de inteligência artificial, a aplicação analisa a descrição de uma vaga, compara seus requisitos com o perfil profissional do candidato e gera uma versão personalizada do currículo, priorizando experiências, competências e palavras-chave relevantes.

O objetivo não é apenas criar currículos visualmente bonitos, mas produzir documentos estratégicos, profissionais e compatíveis com boas práticas de leitura por sistemas ATS, sem inventar ou distorcer informações do candidato.

## 🎯 Problema que a aplicação resolve

A aplicação busca solucionar três dificuldades principais:

- **Dificuldade em encontrar vagas compatíveis:** candidatos frequentemente encontram oportunidades que não correspondem às suas experiências ou qualificações.
- **Currículos genéricos:** utilizar o mesmo currículo para diferentes oportunidades pode dificultar a identificação dos requisitos relevantes.
- **Compatibilidade com ATS:** documentos com estruturas inadequadas ou sem palavras-chave pertinentes podem apresentar dificuldades durante a triagem automatizada.

O MatchCV conecta o perfil profissional às exigências de cada oportunidade, oferecendo uma análise de compatibilidade e uma versão personalizada do currículo.

## ✨ Funcionalidades

- Cadastro e gerenciamento de informações profissionais.
- Importação de currículos em PDF e DOCX.
- Cadastro de vagas por descrição ou URL.
- Extração e interpretação dos requisitos das oportunidades.
- Análise inteligente de compatibilidade entre candidato e vaga.
- Identificação de competências correspondentes e lacunas profissionais.
- Recomendações para melhorar a apresentação do candidato.
- Geração de currículos personalizados para cada oportunidade.
- Otimização estrutural para boas práticas ATS.
- Editor de currículos.
- Exportação de documentos em PDF e DOCX.
- Biblioteca de versões personalizadas.
- Análise de qualidade estrutural de currículos.
- Acompanhamento de candidaturas.

## ⚙️ Como funciona

O funcionamento da aplicação foi pensado para acompanhar o processo desde a identificação de uma oportunidade até a preparação do currículo personalizado.

### 1. Entrada da oportunidade

O usuário pode inserir uma oportunidade de emprego por meio de:

- Descrição completa da vaga.
- URL da oportunidade.
- Cadastro manual.

A aplicação utiliza inteligência artificial para interpretar o conteúdo e identificar as principais informações.

### 2. Extração dos requisitos

A descrição é estruturada para identificar:

- Cargo e empresa.
- Responsabilidades.
- Requisitos obrigatórios.
- Requisitos desejáveis.
- Competências técnicas.
- Competências comportamentais.
- Experiência profissional exigida.
- Formação acadêmica.
- Tecnologias e ferramentas.
- Idiomas.

### 3. Análise de compatibilidade (Job Matching)

Após estruturar a vaga, o sistema compara os requisitos identificados com as informações profissionais fornecidas pelo candidato.

A análise considera os seguintes critérios e pesos iniciais:

| Critério | Peso |
|---|---:|
| Competências técnicas | 30% |
| Experiência profissional | 25% |
| Formação acadêmica | 15% |
| Responsabilidades e atividades | 15% |
| Competências comportamentais | 5% |
| Localização e modalidade | 10% |

O resultado é apresentado em uma pontuação de compatibilidade de 0 a 100%.

Além da pontuação, o sistema identifica:

- Requisitos atendidos.
- Competências parcialmente demonstradas.
- Requisitos não identificados no perfil.
- Pontos fortes do candidato.
- Oportunidades de melhoria.

A análise não deve interpretar automaticamente uma informação ausente como falta de competência.

### 4. Geração do currículo personalizado

Com base na análise, a inteligência artificial utiliza as informações reais do candidato para construir uma versão direcionada à oportunidade.

O processo inclui:

1. Seleção das experiências mais relevantes.
2. Adaptação do resumo profissional.
3. Organização das competências.
4. Reescrita de descrições profissionais.
5. Inclusão de palavras-chave pertinentes, desde que verdadeiras.
6. Organização das seções seguindo boas práticas ATS.

O documento gerado preserva a integridade das informações fornecidas pelo usuário.

**Uma regra fundamental do projeto é não inventar experiências, certificações, habilidades, empresas, datas ou resultados profissionais.**

### 5. Revisão e exportação

Após a geração, o usuário pode revisar e editar o currículo, salvar diferentes versões e exportar o documento em PDF ou DOCX.

Cada versão pode ser associada à oportunidade correspondente, permitindo manter currículos direcionados para diferentes processos seletivos.

---

## 🧠 Desenvolvimento com Lovable

O projeto foi desenvolvido utilizando o **Lovable**, com uma abordagem orientada por engenharia de prompts.

A construção começou com a definição de um megaprompt responsável por estabelecer:

- Objetivo do produto.
- Identidade visual.
- Design System.
- Arquitetura da aplicação.
- Funcionalidades.
- Regras de negócio.
- Estrutura de dados.
- Integração com inteligência artificial.
- Critérios de qualidade.

A escolha do **shadcn/ui** como Design System teve como objetivo manter consistência visual, reutilização de componentes e uma interface moderna.

### Identidade visual

A interface utiliza uma identidade baseada em três cores principais:

| Cor | Código | Aplicação |
|---|---|---|
| Azul-claro | `#60A5FA` | Destaques e ações |
| Branco | `#FFFFFF` | Fundo e superfícies |
| Roxo | `#7C3AED` | Elementos de destaque |

Também foram definidos tons auxiliares para fundos, bordas e textos.

A proposta visual é transmitir tecnologia, confiança e profissionalismo, mantendo uma interface minimalista e intuitiva.

### Tecnologias e ferramentas

| Tecnologia | Finalidade |
|---|---|
| Lovable | Desenvolvimento da aplicação |
| React | Construção da interface |
| TypeScript | Tipagem e organização do código |
| Tailwind CSS | Estilização |
| shadcn/ui | Design System |
| Lucide Icons | Iconografia |
| Lovable Cloud | Recursos de backend e persistência, conforme configuração |
| Inteligência Artificial | Análise de vagas e personalização de currículos |
| GitHub | Versionamento e armazenamento do código |

---

## 📝 Mega Prompt

O desenvolvimento foi orientado por um megaprompt único, responsável por descrever o produto e suas funcionalidades de ponta a ponta.

O prompt original estabeleceu a construção de uma plataforma inteligente de matchmaking de vagas e geração de currículos ATS.

### Principais definições do prompt

- Desenvolvimento de uma aplicação completa do zero.
- Utilização obrigatória do shadcn/ui.
- Identidade visual em azul-claro, branco e roxo.
- Dashboard para acompanhamento de oportunidades.
- Cadastro e interpretação de vagas.
- Motor de matchmaking com pontuação explicável.
- Gerador de currículos personalizados.
- Analisador de compatibilidade ATS.
- Editor e exportação de currículos.
- Biblioteca de versões.
- Rastreador de candidaturas.
- Estrutura de dados organizada.
- Regras de segurança e privacidade.
- Utilização de inteligência artificial para interpretação contextual.

### Evolução do megaprompt

Durante o planejamento, foi identificada uma necessidade de simplificação da experiência inicial.

A primeira versão previa:

- Sistema de autenticação.
- Cadastro de usuários.
- Login.
- Recuperação de senha.
- Onboarding obrigatório.

Posteriormente, o prompt foi revisado para remover completamente essa etapa.

A versão final passou a priorizar o acesso imediato à aplicação, permitindo que o usuário entre diretamente e comece a utilizar suas funcionalidades sem criar uma conta.

Também foram ajustadas as orientações de persistência de dados para contemplar uma experiência sem autenticação, utilizando armazenamento local ou uma estratégia de sessão anônima, conforme os recursos disponíveis.

Essa alteração teve como objetivo reduzir barreiras de entrada e permitir que o usuário experimente o funcionamento da plataforma desde o primeiro acesso.

---

## 🔧 Ajustes solicitados após a primeira geração

Após a definição inicial da aplicação, foram estabelecidas algumas alterações importantes para alinhar o produto à proposta desejada.

### 1. Remoção da autenticação

**Alteração:** remoção de login, cadastro, recuperação de senha e onboarding obrigatório.

**Motivo:** permitir acesso imediato, sem exigir informações pessoais ou criação de conta antes da utilização.

### 2. Persistência compatível com acesso anônimo

**Alteração:** adaptação da arquitetura para permitir armazenamento dos dados sem depender de um usuário autenticado.

**Motivo:** manter a experiência de utilização mesmo sem sistema de contas, considerando as limitações do armazenamento local e a possibilidade de evolução futura.

### 3. Integridade das informações profissionais

**Alteração:** inclusão de regras explícitas para impedir que a inteligência artificial invente experiências, competências, certificações ou resultados.

**Motivo:** garantir que a personalização do currículo melhore a apresentação profissional sem comprometer a veracidade das informações.

### 4. Matchmaking explicável

**Alteração:** definição de critérios e pesos para calcular a compatibilidade entre o perfil e a oportunidade.

**Motivo:** evitar pontuações arbitrárias e permitir que o candidato entenda quais requisitos atende e quais ainda não foram identificados.

### 5. Foco em currículos ATS

**Alteração:** especificação de regras estruturais para os documentos gerados, priorizando layouts lineares, seções convencionais e palavras-chave relevantes.

**Motivo:** melhorar a legibilidade dos documentos por sistemas de recrutamento automatizados.

### 6. Separação entre perfil original e currículos personalizados

**Alteração:** definição de uma biblioteca de versões independentes.

**Motivo:** permitir a criação de vários currículos direcionados sem modificar ou sobrescrever as informações profissionais originais.

---

## 📸 Screenshots

Adicione aqui capturas de tela das principais funcionalidades da aplicação.

### Dashboard

<img width="1920" height="1032" alt="image" src="https://github.com/user-attachments/assets/69157683-fd8f-47d7-8cff-95a47e9cbe95" />


### Análise de compatibilidade

<img width="1920" height="1032" alt="image" src="https://github.com/user-attachments/assets/5380007b-dcbe-4703-afe9-998cdebe71b0" />


### Geração de currículo ATS

<img width="1920" height="1032" alt="image" src="https://github.com/user-attachments/assets/ff6129a6-122d-4bec-9c7a-f4355e12ee95" />


### Vagas

<img width="1920" height="1032" alt="image" src="https://github.com/user-attachments/assets/c806ea7f-d08f-4e52-acab-4d2a1be4f5ae" />


### Biblioteca de currículos

<img width="1920" height="1032" alt="image" src="https://github.com/user-attachments/assets/0d77dc3d-ecc9-4283-a00c-ebbd83de2332" />

---

## 🚀 Aplicação publicada

**Acesse a aplicação:**

https://screenshot-to-soul-3184.lovable.app/

**Repositório GitHub:**

https://github.com/leandroyanaguihara/Criando-um-Gerador-de-Curr-culos-ATS-Friendly-com-Lovable

---

## 📌 Considerações finais

O MatchCV surgiu da proposta de utilizar inteligência artificial para tornar a busca por oportunidades profissionais mais estratégica e personalizada.

Mais do que adaptar palavras-chave, a aplicação busca compreender a relação entre as experiências reais do candidato e os requisitos de cada oportunidade.

O projeto também representa uma experiência prática de desenvolvimento com ferramentas de IA, engenharia de prompts, construção de interfaces com shadcn/ui e organização de uma aplicação web orientada a um problema real.

**Perfil profissional → Matchmaking inteligente → Currículo personalizado → Mais preparo para processos seletivos.**

---

<p align="center">
  Desenvolvido com 💙 e inteligência artificial.
</p>
