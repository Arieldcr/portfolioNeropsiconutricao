# Portfolio Profissional — Ariel de Carvalho Rodrigues
> **Foco:** SRE Developer & Cloud Infrastructure 

Este projeto é um portfólio profissional desenvolvido para a disciplina de **Aplicações para Internet**. O objetivo técnico da versão atual (v2.0) é a implementação de uma arquitetura robusta de **Design Token System** aplicada a um layout moderno e responsivo.

## 🚀 Tecnologias e Ferramentas
- **Frontend:** HTML5, CSS3 Moderno (Custom Properties).
- **Metodologia CSS:** ITCSS (Inverted Triangle CSS) + BEM (Block Element Modifier).
- **Infraestrutura em Estudo:** Docker, Kubernetes, Python, Grafana, Linux.
- **Versionamento:** Git & GitHub.

## 🛠️ Arquitetura Técnica (Entregável Aula 10)

O projeto foi totalmente refatorado na **Aula 10** para atender aos requisitos de auditoria e evolução do sistema visual. A estrutura de CSS foi dividida em camadas de responsabilidade usando `@layer` (Desafio Avançado):

### 1. Sistema de Tokens (`/css/tokens/`)
- **Primitives (`primitives.css`):** Contém a paleta bruta. Todos os tokens primitivos usam o prefixo `_` (ex: `--_blue-400`) para sinalizar que são de uso exclusivo do sistema.
- **Semantic (`semantic.css`):** Mapeia os primitivos para intenções de uso (ex: `--color-action-primary`).
- **Spacing (`spacing.css`):** Escala previsível baseada em múltiplos de **4px**.
- **Typography (`typography.css`):** Tokens para famílias, escalas de tamanho e pesos.

### 2. Camadas de Estilos (`/css/base/` e `/css/components/`)
- **Base:** Reset e estilos globais semânticos.
- **Components:** Estilos encapsulados para `Navbar`, `Hero`, `Cards` e `Footer`, garantindo que **nenhum valor hardcoded** (cor ou tamanho fixo) seja usado diretamente nos componentes.

## 💻 Como visualizar localmente
Para garantir que as diretivas `@layer` e os `@import` externos funcionem corretamente devido às políticas de CORS dos navegadores, recomenda-se:

1. Clonar o repositório.
2. Abrir a pasta no **VS Code**.
3. Utilizar a extensão **Live Server** para rodar o projeto em um servidor local.

## 📝 Checkpoint de Validação (Aula 10)
- [x] Tokens primitivos separados dos semânticos.
- [x] Primitivos prefixados com `_`.
- [x] Escala de espaçamento baseada em 4px.
- [x] Uso de `@layer` para precedência explícita.
- [x] CSS de componente 100% livre de valores hardcoded.

---
Desenvolvido por [Ariel de Carvalho Rodrigues](https://github.com/Arieldcr)
