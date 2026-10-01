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
