# Diário de bordo 2º parte 4º bi
Diário de bordo para a segunda parte do segundo bimeste de análise e desenvolvimento de sistemas.

---

<br>

## Banco de dados

### Álgebra relacional

É uma linguagem formal para manipulação de tabelas.
Fornece operações que geram novas relações a partir de relações existentes.

#### Operações Fundamentais

- Seleção - Filtra linhas

- Projeção - Seleciona colunas

- União - Combina tuplas de duas relações.

- Diferença - Retorna tuplas de uma relação que não estão na outra.

- Produto Cartesiano - Combina todas as tuplas de duas relações.

- Renomeação - Dá novo nome a uma relação ou atributo.

#### Operações derivadas

- Junção - Combina tuplas relacionadas

- Interseção - Tuplas comuns a duas relações.

- Divisão - Usada em consultas para todos

### Importância

É uma base formal para o sql onde permite verificar a equivalência entre consultas, fundamentando a otimização de consultas em SGBDs.

## Normalização de Banco de Dados

Principais pontos focados:
- Redução da redundância
- Aumento da integridade
- Melhoria no desempenho
- Facilidade de manutenção

### Normalização de Relações

A normalização tem o processo de decompor relações "ruins" dividindo seus atributos em relações menores. Outra maneira de entender é dizer que a forma normal é "uma regra que tem que ser obedecida pela tabela para que ela seja considerada bem projetada" (HEUSER, 2009).

**Forma normal**: Indica o número de qualidade de uma relação.

As normalizações 2FN, 3FN e BCNF se baseiam em chave de dependências funcionais de uma relação esquema.
4FN e 5FN baseiam-se em chaves e dependências multivaloradas.

### Atividade dia 30/09/2026 - Prática da normalização

Tabela exemplo:

| CodProj | Tipo | Descr | EmpregadosAlocados |
|---|---|---|---|
| LSC001 | Novo Desenv. | Sistema de Estoque | 2146-Joao-CatA1-Sal4000-01/11/91-24h<br>3145-Silvio-CatA2-Sal5500-02/10/91-24h<br>6126-Jose-CatB1-Sal9000-03/10/92-18h<br>1214-Carlos-CatA2-Sal5500-04/10/92-18h<br>8191-Mario-CatA1-Sal4000-01/11/92-12h |
| PAG02 | Manutencao | Sistema de RH | 8191-Mario-CatA1-Sal4000-01/05/93-12h<br>4112-Joao-CatA2-Sal5500-04/01/91-24h<br>6126-Jose-CatB1-Sal9000-01/11/92-12h<br>7721-Paula-CatC1-Sal12000-10/05/93-40h |
| CRM03 | Novo Desenv. | Gestao de Clientes | 3145-Silvio-CatA2-Sal5500-15/02/94-20h<br>1214-Carlos-CatA2-Sal5500-15/02/94-40h<br>9932-Ana-CatB2-Sal9500-20/02/94-40h<br>5543-Lucas-CatA1-Sal4000-01/03/94-20h<br>7721-Paula-CatC1-Sal12000-01/03/94-10h |
| ERP04 | Migracao | Modulo Financeiro | 9932-Ana-CatB2-Sal9500-10/01/95-40h<br>6126-Jose-CatB1-Sal9000-15/01/95-20h<br>8191-Mario-CatA1-Sal4000-15/01/95-40h<br>2146-Joao-CatA1-Sal4000-20/01/95-40h |
| MOB05 | Novo Desenv. | App de Entregas | 5543-Lucas-CatA1-Sal4000-05/06/95-40h<br>4112-Joao-CatA2-Sal5500-10/06/95-20h<br>3145-Silvio-CatA2-Sal5500-10/06/95-20h<br>7721-Paula-CatC1-Sal12000-15/06/95-10h |

Tabela Final com normalizações:

