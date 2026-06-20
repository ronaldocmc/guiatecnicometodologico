# Contratos

Contratos definem o que cada módulo, método, pipeline, agente ou artefato exige, produz e garante.

## Tipos

- Entrada.
- Saída.
- Qualidade.
- Erro.
- Execução.
- Governança.

```json
{
  "modulo": "M_Transformacao",
  "entrada": {"dataset": "obrigatorio", "schema": "obrigatorio"},
  "saida": {"dataset_tratado": "obrigatorio", "log_execucao": "obrigatorio"},
  "qualidade_minima": {"completude": 0.95, "rastreabilidade": true},
  "erros_criticos": ["schema_invalido", "ausencia_de_metadados"]
}
```
