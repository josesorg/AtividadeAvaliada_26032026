# Avaliação — Engenharia de Software
**Sistema Integrado de Gestão de Farmácia — MVP Definido pelo Estudante**

Aluno: José Eduardo de Paula Sorg  
RA: 24000304  
Data: 26/03/2026  

---

# 1. Definição do MVP
Meu MVP é sobre o processo de venda que vem desde a identificação ou cadastro do cliente até podendo chegar a uma emissão do comprovante, incluindo principalmente a verificação de estoque junto com o tratamento de vendas a prazo.

Explique claramente:

- O que está **dentro** do MVP
-O sistema possibilita o registro de vendas à vista, a busca de produtos por nome ou código, a verificação do estoque em tempo real, o cadastro de clientes durante o atendimento, a atualização automática do estoque, a emissão de comprovantes e a validação de receitas médicas quando necessário.
- O que está **fora** do MVP
- O sistema não abrange o controle completo de compras com fornecedores, o gerenciamento de contas a pagar, a geração de relatórios gerenciais avançados, a transferência de estoque entre unidades, nem o controle financeiro detalhado, como fluxo de caixa completo e a gestão integrada de múltiplas unidades.
- Por que você fez essas escolhas
- Essas decisões foram tomadas para concentrar o desenvolvimento no fluxo de vendas, que representa a operação central da farmácia, possibilitando testar o sistema de forma ágil e gerar resultados úteis já nas primeiras entregas.

Exemplo de início:  
> “Meu MVP cobre o processo de venda desde a identificação/cadastro do cliente até a emissão do comprovante, incluindo tratamento de estoque insuficiente.”

---

# 2. Regras de Negócio (mínimo: 5)
Liste e descreva **cada RN** de forma clara.

**RN01 —*Não é permitido vender produtos sem estoque disponivel.*  
**RN02 —*Toda venda deve atualizar automaticamente o estoqui da unidade.*  
**RN03 —*Vendas a prazo devem gerar automaticamente um registro em contas a receber.*  
**RN04 —*Clientes devem estar cadastrados para realizar compras a prazo.*  
**RN05 —*O valor total da venda deve ser calculado pelo sistema.*  

(Adicione mais se quiser.)

---

# 3. Requisitos Funcionais (mínimo: 8)
Liste os requisitos funcionais do seu MVP.

**RF01 —*O sistema deve permitir o cadastro para os clientes.*  
**RF02 —*O sistema deve trazer a permissão para produtos por nome, código ou fabricante.*  
**RF03 —*O sistema deve mostrar a exibição das informações do produto (preço, descrição e estoque).*  
**RF04 —*O sistema deve registrar vendas.*  
**RF05 —*O sistema deve verificar a disponibilidade do estoque antes da venda.*  
**RF06 —*O sistema deve permitir vendas à vista e a prazo.*  
**RF07 —*O sistema deve emitir comprovante de venda.*  
**RF08 —*O sistema deve atualizar o estoque automaticamente após a venda.*  

(Adicione mais se quiser.)

---

# 🛡 4. Requisitos Não Funcionais (mínimo: 4)
Liste os RNFs do sistema conforme seu MVP.

**RNF01 —*O sistema deve trazer as respostas das operações em até 2 segundos.*  
**RNF02 —*O sistema deve manter a garantia de segurança por meio de autenticação de usuários.*  
**RNF03 —*O sistema deve estar disponivel cerca de 99% do tempo.*  
**RNF04 —*O sistema deve possuir uma interface simples e intuitiva.*  

(Adicione mais se quiser.)

---

# 5. Casos de Uso (mínimo: 10)
### Inserir **diagrama de casos de uso geral**, demonstrando claramente:
- os 10 casos
- relação entre eles e atores
- pelo menos 3 includes
- pelo menos 3 extends
<img width="359" height="156" alt="image" src="https://github.com/user-attachments/assets/baf23256-5f08-4419-890b-7c64f3892e66" />

---

# 6. Documentação dos Casos de Uso
Para **cada caso de uso**, utilize o template abaixo:
---

## **UC01 — Identificar Cliente**
**Ator(es):*Atendente*  
**Descrição:*Localiza um cliente no sistema.*  
**Pré-condições:*Sistema em funcionamento*  
**Pós-condições:*Cliente identificado ou não encontrado*  

### Fluxo Principal
1. Atendente informa dados do cliente
2. Sistema realiza busca
3. Sistema exibe resultado
4.  

### Fluxos Alternativos / Exceções
- FA01 —  Cliente não encontrado → permitir cadastro
- FA02 —  

### Relacionamentos
- **Include:** (listar quando aplicável)  
- **Extend:*Cadastrar Cliente* 

### Inserir o diagrama de atividades do Caso de Uso, demonstrando tudo o fluxo princial e alternativos/exceções.
<img width="359" height="295" alt="image" src="https://github.com/user-attachments/assets/e08bf06c-f54d-417a-8671-6a24049143e1" />

---

> Repita essa estrutura para **todos os seus casos de uso** (mínimo 10).

## **UC02 — Cadastrar Cliente**
**Ator(es):*Atendente*  
**Descrição:*Cadastra um novo cliente*  
**Pré-condições:*Cliente não encontrado*  
**Pós-condições:*Cliente cadastrado*  

### Fluxo Principal
1. Inserir dados do cliente 
2. Validar informações
3. Salvar cadastro
4.  

### Fluxos Alternativos / Exceções
- FA01 —  Dados inválidos → solicitar correção
- FA02 —  

### Relacionamentos
- **Include:** (listar quando aplicável)  
- **Extend:** (listar quando aplicável) 

### Inserir o diagrama de atividades do Caso de Uso, demonstrando tudo o fluxo princial e alternativos/exceções.
<img width="250" height="312" alt="image" src="https://github.com/user-attachments/assets/c7777887-64d8-42f2-ab71-e5d87f2a8936" />

---

> Repita essa estrutura para **todos os seus casos de uso** (mínimo 10).

## **UC03 — Consultar Produto**
**Ator(es):*Atendente*  
**Descrição:*Busca produtos no sistema*  
**Pré-condições:*Sistema ativo*  
**Pós-condições:*Lista de produtos exibida*  

### Fluxo Principal
1. Informar nome ou código
2. Sistema retorna resultados
3. 
4.  

### Fluxos Alternativos / Exceções
- FA01 — Produto não encontrado
- FA02 —  

### Relacionamentos
- **Include:** (listar quando aplicável)  
- **Extend:** (listar quando aplicável) 

### Inserir o diagrama de atividades do Caso de Uso, demonstrando tudo o fluxo princial e alternativos/exceções.
<img width="299" height="312" alt="image" src="https://github.com/user-attachments/assets/fe7eb462-bf24-4016-8e92-dbe5a00076cf" />

---

> Repita essa estrutura para **todos os seus casos de uso** (mínimo 10).

## **UC04 — Verificar Estoque**
**Ator(es):*Sistema*  
**Descrição:*Verifica quantidade disponível*  
**Pré-condições:*Produto selecionado*  
**Pós-condições:*Quantidade exibida*  

### Fluxo Principal
1. Consultar estoque
2. Retornar quantidade
3. 
4.  

### Fluxos Alternativos / Exceções
- FA01 — Estoque insuficiente
- FA02 —  

### Relacionamentos
- **Include:** (listar quando aplicável)  
- **Extend:** (listar quando aplicável) 

### Inserir o diagrama de atividades do Caso de Uso, demonstrando tudo o fluxo princial e alternativos/exceções.
<img width="337" height="257" alt="image" src="https://github.com/user-attachments/assets/833d7429-99d5-4c86-a07e-1da5a274b751" />

---

> Repita essa estrutura para **todos os seus casos de uso** (mínimo 10).

## **UC05 — Registrar Venda**
**Ator(es):*Atendente*  
**Descrição:*Registra itens da venda*  
**Pré-condições:*Cliente identificado*  
**Pós-condições:*Itens adicionados à venda*  

### Fluxo Principal
1. Selecionar produto
2. Informar quantidade
3. Adicionar item
4.  

### Fluxos Alternativos / Exceções
- FA01 — Estoque insuficiente
- FA02 —  

### Relacionamentos
- **Include:*Consultar Produto, Verificar Estoque*  
- **Extend:*Validar Receita* 

### Inserir o diagrama de atividades do Caso de Uso, demonstrando tudo o fluxo princial e alternativos/exceções.
<img width="271" height="367" alt="image" src="https://github.com/user-attachments/assets/3cf0c54b-368d-47cb-ba6d-bcdad217c442" />

---

> Repita essa estrutura para **todos os seus casos de uso** (mínimo 10).

## **UC06 — Calcular Total da Venda**
**Ator(es):*Sistema*  
**Descrição:*Calcula valor total*  
**Pré-condições:*Itens adicionados*  
**Pós-condições:*Total calculado*  

### Fluxo Principal
1. Somar valores dos itens
2. 
3. 
4.  

### Fluxos Alternativos / Exceções
- FA01 — Nenhum item
- FA02 —  

### Relacionamentos
- **Include:** (listar quando aplicável) 
- **Extend:** (listar quando aplicável) 

### Inserir o diagrama de atividades do Caso de Uso, demonstrando tudo o fluxo princial e alternativos/exceções.
<img width="176" height="193" alt="image" src="https://github.com/user-attachments/assets/72a4e3ac-abd8-4c82-b3ab-6f779c98081c" />


---

> Repita essa estrutura para **todos os seus casos de uso** (mínimo 10).

## **UC07 — Finalizar Venda**
**Ator(es):*Atendente*  
**Descrição:*Finaliza a venda*  
**Pré-condições:*Venda em andamento*  
**Pós-condições:*Venda concluída*  

### Fluxo Principal
1. Selecionar forma de pagamento
2. Confirmar venda
3. 
4.  

### Fluxos Alternativos / Exceções
- FA01 — Cancelamento da venda
- FA02 —  

### Relacionamentos
- **Include:*Calcular Total*  
- **Extend:*Registrar Conta a Receber* 

### Inserir o diagrama de atividades do Caso de Uso, demonstrando tudo o fluxo princial e alternativos/exceções.
<img width="225" height="451" alt="image" src="https://github.com/user-attachments/assets/38c8c30a-bc37-4302-a8b4-e4bbd07eec3c" />


---

> Repita essa estrutura para **todos os seus casos de uso** (mínimo 10).

## **UC08 — Emitir Comprovante**
**Ator(es):*Sistema*  
**Descrição:*Gera comprovante*  
**Pré-condições:*Venda finalizada*  
**Pós-condições:*Comprovante emitido*  

### Fluxo Principal
1. Gerar comprovante
2. Exibir ou imprimir
3. 
4.  

### Fluxos Alternativos / Exceções
- FA01 — Falha na impressão
- FA02 —  

### Relacionamentos
- **Include:** (listar quando aplicável)
- **Extend:** (listar quando aplicável) 

### Inserir o diagrama de atividades do Caso de Uso, demonstrando tudo o fluxo princial e alternativos/exceções.
<img width="257" height="257" alt="image" src="https://github.com/user-attachments/assets/4b5e61fc-3e4b-4858-95a1-bcd5fe0b42fa" />


---

> Repita essa estrutura para **todos os seus casos de uso** (mínimo 10).

## **UC09 — Registrar Conta a Receber**
**Ator(es):*Sistema*  
**Descrição:*Registra pagamento futuro*  
**Pré-condições:*Venda a prazo*  
**Pós-condições:*Conta registrada*  

### Fluxo Principal
1. Criar registro
2. Definir vencimento
3. 
4.  

### Fluxos Alternativos / Exceções
- FA01 — Erro no registro
- FA02 —  

### Relacionamentos
- **Include:** (listar quando aplicável)
- **Extend:** (listar quando aplicável) 

### Inserir o diagrama de atividades do Caso de Uso, demonstrando tudo o fluxo princial e alternativos/exceções.
<img width="157" height="248" alt="image" src="https://github.com/user-attachments/assets/07492691-ce10-496e-a6d7-55394249dfc0" />

---

> Repita essa estrutura para **todos os seus casos de uso** (mínimo 10).

## **UC10 — Validar Receita**
**Ator(es):*Farmacêutico*  
**Descrição:*Autoriza venda de medicamento controlado*  
**Pré-condições:*Produto controlado*  
**Pós-condições:*Venda autorizada ou negada*  

### Fluxo Principal
1. Analisar receita
2. Autorizar venda
3. 
4.  

### Fluxos Alternativos / Exceções
- FA01 — Receita inválida → negar venda
- FA02 —  

### Relacionamentos
- **Include:** (listar quando aplicável)
- **Extend:** (listar quando aplicável) 

### Inserir o diagrama de atividades do Caso de Uso, demonstrando tudo o fluxo princial e alternativos/exceções.
<img width="235" height="312" alt="image" src="https://github.com/user-attachments/assets/8a1809d4-472c-4ef4-9e18-74d880223c32" />


---

> Repita essa estrutura para **todos os seus casos de uso** (mínimo 10).






