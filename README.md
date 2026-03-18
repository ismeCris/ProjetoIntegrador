# 📦 Sistema de Estoque e Vendas em C
**Projeto Acadêmico**

![C](https://img.shields.io/badge/language-C-blue.svg)
![License](https://img.shields.io/badge/license-MIT-green.svg)
 
 
> Sistema simplificado desenvolvido em **C** para gerenciamento de produtos, controle de estoque e processamento de vendas. O projeto utiliza a estrutura de **listas duplamente encadeadas** para garantir eficiência na manipulação dos dados em memória.

---

## 🚀 Funcionalidades

- **📌 Gestão de Produtos:** Cadastro, atualização e exclusão (CRUD).
- **📋 Visualização:** Listagem completa do estoque atual.
- **🛒 Módulo de Vendas:** Registro de transações com baixa automática no estoque.
- **🧾 Cupom Fiscal:** Geração detalhada da nota de compra.
- **💳 Financeiro:** Sistema de pagamento flexível (à vista ou parcelado).
- **💾 Persistência:** Salvamento automático de dados em arquivo `.txt`.

---

## 🛠️ Compilação e Execução

Para rodar o projeto, você precisará de um compilador C (como o GCC).

1. **Compile o projeto:**
gcc main.c funcoes.c -o sistema

2. **Execute o programa:**
./sistema

---

## 💾 Arquivo de Dados

Os dados dos produtos são armazenados de forma persistente no arquivo:
> `produtos.txt`

*O sistema verifica a existência deste arquivo ao iniciar; caso não seja encontrado, um novo será criado automaticamente.*

---

## 💳 Regras de Negócio (Pagamento)

O sistema aplica automaticamente descontos ou acréscimos baseados na modalidade escolhida:

### 💵 Pagamento à Vista
| Valor da Compra | Desconto |
| :--- | :--- |
| Até R$ 50,00 | **5%** |
| De R$ 50,01 a R$ 100,00 | **10%** |
| Acima de R$ 100,00 | **18%** |

### 🧾 Pagamento Parcelado
| Parcelamento | Acréscimo |
| :--- | :--- |
| Até 3x | **+5%** |
| De 4x até 12x | **+8%** |

---

## 📂 Estrutura do Projeto

.
├── main.c        # Ponto de entrada e menu principal
├── funcoes.c     # Lógica das funcionalidades e manipulação de lista
├── produtos.txt  # Banco de dados em texto plano
└── README.md     # Documentação do projeto

---

## 📌 Melhorias Futuras

- [ ] Implementação de Interface Gráfica (GUI).
- [ ] Integração com banco de dados SQL.
- [ ] Geração de relatórios de vendas diários/mensais.
- [ ] Sistema de autenticação de usuários (Login/Senha).

---

## 👨‍💻 Autor

Desenvolvido por **Cris**
