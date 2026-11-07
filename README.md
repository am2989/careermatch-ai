# CareerMatch AI — ATS Resume Optimizer

**Transforme o seu currículo na candidatura certa.**

O CareerMatch AI é uma aplicação web desenvolvida no âmbito de um desafio da [Digital Innovation One (DIO)](https://www.dio.me/), com o objetivo de ajudar candidatos a adaptar os seus currículos às exigências das ofertas de emprego e melhorar a sua apresentação perante sistemas ATS (Applicant Tracking Systems).

A aplicação compara o conteúdo de um currículo com a descrição de uma vaga, identifica palavras-chave correspondentes e em falta, apresenta uma estimativa de compatibilidade e disponibiliza uma versão otimizada do currículo.

Link: https://career-fit-canvas.lovable.app
---

## 1. Problema identificado

Um dos desafios enfrentados por quem procura emprego é conseguir que o seu currículo ultrapasse os primeiros filtros dos processos de recrutamento.

Muitas empresas utilizam sistemas ATS (Applicant Tracking Systems) para analisar, organizar e classificar candidaturas antes de estas chegarem aos recrutadores.

Um currículo pode apresentar uma experiência profissional relevante e, ainda assim, não destacar adequadamente as competências e palavras-chave procuradas numa determinada oportunidade.

O CareerMatch AI procura responder a este problema, facilitando a adaptação do currículo a cada oferta de emprego.

## 2. Objetivo do projeto

Desenvolver uma aplicação simples e intuitiva que permita:

- Comparar um currículo com uma descrição de vaga.
- Identificar palavras-chave e competências em comum.
- Detetar requisitos relevantes que não aparecem no currículo.
- Apresentar uma estimativa de compatibilidade.
- Sugerir melhorias na apresentação da experiência profissional.
- Gerar uma versão do currículo mais organizada e ATS-friendly.
- Disponibilizar uma versão preparada para exportação em PDF.

**Princípio fundamental:** melhorar a forma como o candidato apresenta as suas qualificações, sem inventar experiências profissionais, competências, certificações ou formação académica.

## 3. Funcionalidades

### Análise de compatibilidade

O utilizador pode inserir o conteúdo do seu currículo e a descrição da vaga que pretende analisar.

A aplicação apresenta uma análise com:

- Percentagem estimada de compatibilidade.
- Palavras-chave encontradas.
- Palavras-chave em falta.
- Sugestões de melhoria.

### Identificação de palavras-chave

A aplicação compara os dois textos e identifica termos profissionais e competências relevantes para a oportunidade.

Os resultados são apresentados visualmente para facilitar a identificação dos pontos fortes e das áreas que podem necessitar de melhoria.

### Geração de currículo otimizado

Com base no currículo original e na descrição da vaga, é apresentada uma versão reorganizada e melhorada.

A estrutura contempla:

1. Nome e contacto.
2. Perfil profissional.
3. Competências.
4. Experiência profissional.
5. Formação académica.
6. Certificações.
7. Idiomas.

### Pré-visualização e exportação

O utilizador pode visualizar a versão otimizada do currículo, rever o conteúdo e preparar o documento para exportação em PDF.

---

## 4. Como funciona a aplicação

O funcionamento segue um fluxo simples:

1. **Inserção da vaga:** o utilizador cola a descrição da oportunidade.
2. **Inserção do currículo:** o utilizador cola o conteúdo do seu currículo atual.
3. **Análise:** a aplicação compara os dois textos e identifica correspondências.
4. **Resultados:** é apresentada a compatibilidade estimada, as palavras-chave encontradas e as que estão em falta.
5. **Otimização:** é gerada uma versão melhorada do currículo.
6. **Exportação:** o utilizador pode rever e preparar o documento para PDF.

### Critérios de análise

A estimativa de compatibilidade considera os seguintes pesos:

| Critério | Peso |
|---|---:|
| Competências e palavras-chave | 70% |
| Experiência e responsabilidades | 20% |
| Formação e qualificações | 10% |
| **Total** | **100%** |

Os resultados são apresentados de acordo com os seguintes intervalos:

| Compatibilidade | Classificação |
|---|---|
| 80%–100% | Excelente compatibilidade |
| 60%–79% | Boa compatibilidade |
| 40%–59% | Compatibilidade moderada |
| 0%–39% | Compatibilidade reduzida |

**Nota:** a percentagem é uma estimativa baseada na comparação textual e não representa uma classificação oficial de um sistema ATS empresarial.

---

## 5. Tecnologias utilizadas

O projeto foi desenvolvido com o apoio do Lovable, utilizando as seguintes tecnologias e ferramentas previstas na implementação:

- **Lovable:** criação e desenvolvimento da aplicação.
- **React:** construção da interface.
- **TypeScript:** estruturação do código.
- **Tailwind CSS:** estilização e organização visual.
- **shadcn/ui:** componentes da interface.
- **Lucide Icons:** elementos gráficos e ícones.
- **JavaScript:** lógica de análise e comparação textual.

A aplicação foi concebida como um MVP (Minimum Viable Product), sem necessidade de autenticação ou integração com serviços externos pagos.

---

## 6. Design System

Foi escolhido o **shadcn/ui** como design system para garantir uma interface consistente, moderna e intuitiva.

### Paleta de cores

| Cor | Código | Utilização |
|---|---|---|
| Azul-claro | `#8CCDF0` | Botões e destaques |
| Azul suave | `#DCEFFC` | Elementos secundários |
| Fundo azul muito claro | `#F4F9FD` | Fundo da aplicação |
| Branco | `#FFFFFF` | Cartões e áreas de conteúdo |
| Amarelo-claro | `#FFF1B8` | Alertas e sugestões |
| Azul-escuro | `#20354A` | Texto principal |

A interface foi pensada para proporcionar uma experiência simples, profissional e responsiva.

---

## 7. Mega Prompt e desenvolvimento com IA

O desenvolvimento começou com a criação de um megaprompt para o Lovable, descrevendo a aplicação, o seu objetivo, as funcionalidades, o design system e a identidade visual.

O prompt inicial foi posteriormente simplificado para concentrar os recursos disponíveis no núcleo do desafio.

### Principais decisões durante o desenvolvimento

- Redução da aplicação para uma única página.
- Eliminação do login e do registo de utilizadores.
- Remoção de dashboards e funcionalidades secundárias.
- Eliminação da necessidade de APIs pagas e integrações externas.
- Priorização da análise de compatibilidade.
- Priorização da geração de um currículo otimizado.
- Simplificação da arquitetura para facilitar a publicação.

### Mega Prompt utilizado na versão final

```text
Build a polished, modern and responsive single-page web application
called CareerMatch AI.

Use shadcn/ui, Tailwind CSS and Lucide icons.

Color palette:
- Light blue: #8CCDF0
- Soft blue: #DCEFFC
- Background: #F4F9FD
- White: #FFFFFF
- Pale yellow: #FFF1B8
- Dark navy: #20354A

All interface text must be in European Portuguese.

The application must allow users to:

1. Paste a job description.
2. Paste their existing CV.
3. Analyze compatibility between both texts.
4. Display a compatibility percentage.
5. Identify matching and missing keywords.
6. Provide practical recommendations.
7. Generate an improved ATS-friendly CV.
8. Preview and edit the generated CV.
9. Export the CV as PDF.

Use JavaScript-based text analysis.

Calculate an indicative score using:
- Skills and keyword matching: 70%.
- Relevant experience: 20%.
- Education and qualifications: 10%.

Never invent professional experience, skills,
qualifications or certifications.

Use a clean, professional, single-column
ATS-friendly CV layout.

No login, registration, backend or paid APIs.

Build a functional single-page MVP focused
on the core workflow:

Paste CV → Paste job description →
Analyze → View compatibility →
Generate optimized CV → Export PDF.

Prioritize usability, responsive design
and visual quality.
```

---

## 8. Limitações e possíveis melhorias futuras

Esta versão representa um MVP desenvolvido para demonstrar o conceito e o funcionamento da solução.

Existem várias possibilidades de evolução:

- Integração de modelos de Inteligência Artificial para melhorar a personalização dos currículos.
- Análise semântica mais avançada das descrições das vagas.
- Exportação de currículos também em formato DOCX.
- Histórico de análises e versões de currículos.
- Criação de perfis de utilizador.
- Integração com plataformas de emprego.
- Recomendações personalizadas para desenvolvimento de competências.

Estas funcionalidades poderão ser implementadas em versões futuras.

---

## 9. Demonstração da aplicação

**Aplicação publicada:** https://career-fit-canvas.lovable.app

### Screenshots

Adiciona aqui imagens da aplicação para demonstrar o seu funcionamento.

#### Página principal

![Página principal do CareerMatch AI](<img width="1842" height="856" alt="image" src="https://github.com/user-attachments/assets/4c860a0a-c0d7-40fc-a168-9afeb27f1308" />
)

#### Análise de compatibilidade

![Resultados da análise de compatibilidade](<img width="1446" height="717" alt="image" src="https://github.com/user-attachments/assets/631dad6b-4723-4f04-9a7c-9514b4d8510c" />
)

#### Currículo otimizado

![Pré-visualização do currículo otimizado](<img width="1493" height="801" alt="image" src="https://github.com/user-attachments/assets/7bb26dfb-dd2e-4687-9b70-e7505badf937" />
)

---

## 10. Como executar o projeto localmente

Para executar o projeto no teu computador:

```bash
# Clonar o repositório
git clone https://github.com/am2989/career-fit-canvas

# Entrar na pasta do projeto
cd TEU-REPOSITORIO

# Instalar dependências
npm install

# Iniciar o ambiente de desenvolvimento
npm run dev
```

Abre o endereço local apresentado no terminal para visualizar a aplicação.

---

## 11. Publicação

A aplicação foi desenvolvida com o Lovable e publicada através da respetiva funcionalidade de publicação.

**Link da aplicação:** https://career-fit-canvas.lovable.app/

**Repositório GitHub:** https://github.com/am2989/careermatch-ai/

---

## 12. Considerações finais

O CareerMatch AI nasceu da identificação de um problema real nos processos de recrutamento: a dificuldade em apresentar um currículo alinhado com os requisitos específicos de cada oportunidade.

Este projeto permitiu explorar o desenvolvimento de aplicações web com ferramentas de Inteligência Artificial, experimentar a utilização de um design system e transformar uma ideia numa solução digital.

Mais do que criar uma aplicação visual, o objetivo foi desenvolver um conceito com utilidade prática, que possa evoluir para uma ferramenta de apoio a quem procura novas oportunidades profissionais.

**Projeto desenvolvido no âmbito do desafio da Digital Innovation One (DIO).**

---

*CareerMatch AI — O seu talento merece chegar ao recrutador.*
