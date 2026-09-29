# Guia de Estudos: SOLID, Arquitetura e Design Patterns 🚀

Bem-vindo ao meu repositório de estudos de programação! Aqui estão resumidos os principais conceitos de arquitetura de software para criar códigos limpos, flexíveis e fáceis de manter.

---

## 1. O que significa SOLID?
* **S - Single Responsibility (Responsabilidade Única):** Cada componente ou função deve ter apenas um motivo para mudar[cite: 1]. Não misture lógica de API, estado e interface no mesmo sítio[cite: 1].
* **O - Open/Closed (Aberto/Fechado):** O código deve estar aberto para extensão, mas fechado para modificação[cite: 1, 2]. Adicionamos novas funcionalidades sem mexer no código antigo (ex: usando o padrão *Strategy*).
* **L - Liskov Substitution (Substituição de Liskov):** Componentes especializados devem poder substituir os componentes base sem quebrar o contrato ou causar erros inesperados[cite: 1].
* **I - Interface Segregation (Segregação de Interfaces):** Os clientes não devem ser forçados a depender de propriedades ou métodos que não utilizam[cite: 2].
* **D - Inversão de Dependência:** Módulos de **alto nível** (regras de negócio/interface) não devem depender de módulos de **baixo nível** (detalhes técnicos/APIs). Ambos devem depender de abstrações[cite: 2].

---

## 2. Alto Nível vs. Baixo Nível
* **Alto Nível:** É a camada mais próxima do utilizador e das regras de negócio (o "quê" o sistema faz). Exemplo: Um ecrã de perfil ou uma regra de carrinho de compras.
* **Baixo Nível:** É a camada de infraestrutura e detalhes técnicos (o "como" o sistema faz). Exemplo: Chamadas diretas a bibliotecas como `axios` para buscar dados na base de dados[cite: 2].

---

## 3. Design Patterns (Padrões de Projeto)
São soluções testadas para problemas comuns. O **Strategy Pattern**, por exemplo, ajuda a eliminar `if/else` gigantescos, mapeando comportamentos em objetos limpos e fáceis de expandir[cite: 1].