# Fraternidades, vínculos e pertencimento

**Status:** especificação inicial, sujeita a detalhamento.  
**Origem:** definições fornecidas pelo responsável pelo Fraternos em 19/11/2026.  
**Histórico:** 2026-11-19 — registro inicial das regras RN-0001 a RN-0014.

## Contexto

O Fraternos é um sistema para organizar fraternidades franciscanas, registrar suas atividades, compreender seus vínculos e apoiar processos administrativos e estatutários que serão especificados posteriormente. A estrutura deve ser flexível para acomodar exceções.

## Regras registradas

### RN-0001 — Cadastro administrativo de fraternidades
**Status:** vigente.  
Um usuário administrador do sistema poderá cadastrar fraternidades. Os demais critérios e permissões de cadastro ainda não foram definidos.

### RN-0002 — Tipos e níveis de fraternidade
**Status:** vigente.  
Os tipos de fraternidade são Ordem Franciscana Secular (OFS), Juventude Franciscana (JUFRA) e Infância e Adolescência Franciscana (INAFRA). OFS e JUFRA possuem níveis nacional, regional e local. INAFRA possui apenas nível local.

### RN-0003 — Hierarquia de mesmo tipo
**Status:** vigente.  
Fraternidades regionais da OFS pertencem à nacional da OFS; regionais da JUFRA pertencem à nacional da JUFRA. Fraternidades locais da OFS/JUFRA pertencem a regionais do mesmo tipo; na ausência de regional, podem vincular-se diretamente à nacional do mesmo tipo.

### RN-0004 — Subdivisões administrativas opcionais
**Status:** vigente.  
A organização nacional pode possuir **áreas** e a regional pode possuir **distritos**. Áreas e distritos são divisões administrativas opcionais e **não são fraternidades**. A existência dessas subdivisões não exige que todas as unidades subordinadas sejam agrupadas nelas. O detalhamento de seus vínculos será definido posteriormente.

### RN-0005 — Composição das fraternidades locais
**Status:** vigente.  
Fraternidades locais são compostas por pessoas. As regras detalhadas de admissão, categorias e desligamento serão definidas posteriormente.

### RN-0006 — Vínculos fraternos entre JUFRA e OFS locais
**Status:** vigente.  
Habitualmente, uma JUFRA local vincula-se a uma OFS local ou não possui vínculo, e uma OFS local vincula-se a uma JUFRA local ou não possui vínculo. **Existem exceções à cardinalidade habitual em ambos os sentidos**; não impor limite rígido de um vínculo por fraternidade sem especificação adicional.

### RN-0007 — Vínculos da INAFRA com fraternidades locais
**Status:** vigente.  
Uma INAFRA local pode vincular-se a uma JUFRA local, a uma OFS local, a ambas ou a nenhuma. Seu vínculo natural é com a JUFRA, mas a inexistência de JUFRA ou OFS na localidade, ou outras circunstâncias, não impede a existência da INAFRA. Uma JUFRA ou OFS local pode estar vinculada a nenhuma ou várias INAFRAs.

### RN-0008 — Independência territorial dos vínculos fraternos
**Status:** vigente.  
Vínculos entre fraternidades locais JUFRA e OFS são estabelecidos por escolha e contexto histórico/de origem, não necessariamente por coincidência de território ou regional. Uma JUFRA pode vincular-se a uma OFS de outra localidade e até de território regional distinto.

### RN-0009 — Alteração dos vínculos fraternos
**Status:** vigente.  
Vínculos entre fraternidades locais podem ser alterados, por exemplo quando surge uma OFS mais próxima da JUFRA. As condições, aprovações e o histórico detalhado dessas alterações ainda serão especificados.

### RN-0010 — Responsabilidade administrativa pela INAFRA
**Status:** vigente.  
Toda INAFRA local está sob a guarda/responsabilidade de uma JUFRA regional **ou** nacional, responsável por seu acompanhamento e oficialização. Essa responsabilidade é distinta dos vínculos fraternos locais da RN-0007, que podem estar ausentes.

### RN-0011 — Apoio da OFS à INAFRA
**Status:** vigente.  
A OFS regional ou nacional pode acompanhar, nutrir, incentivar ou servir de ponte de comunicação para a JUFRA no acompanhamento da INAFRA, sem substituir a responsabilidade administrativa da JUFRA estabelecida na RN-0010.

### RN-0012 — Pertencimento individual por tipo
**Status:** vigente.  
Uma pessoa pode pertencer a apenas **uma fraternidade local de cada tipo por vez**. A mesma pessoa pode pertencer simultaneamente a uma JUFRA local e a uma OFS local. Outras situações de pertencimento serão detalhadas posteriormente.

### RN-0013 — Transferência entre fraternidades
**Status:** vigente.  
É possível transferir uma pessoa entre fraternidades locais do mesmo tipo. Requisitos, procedimentos e aprovações ainda serão especificados.

### RN-0014 — Histórico de pertencimento
**Status:** vigente.  
O sistema deverá preservar o histórico de transferências e os períodos de pertencimento de cada pessoa às fraternidades, identificando origem e destino das transferências. Datas, estados e demais detalhes serão definidos posteriormente.

## Relações e dependências
- RN-0002 e RN-0003: tipos e hierarquia.
- RN-0004: subdivisões da estrutura administrativa de RN-0003.
- RN-0006, RN-0007, RN-0008 e RN-0009: vínculos fraternos locais, independentes da hierarquia administrativa.
- RN-0007, RN-0010 e RN-0011: vínculo fraterno da INAFRA não equivale à responsabilidade administrativa.
- RN-0012, RN-0013 e RN-0014: pertencimento, transferência e histórico de pessoas.

## Questões ainda não especificadas

Este registro **não** estabelece automaticamente: estatutos e processos; aprovações; cardinalidade máxima das exceções entre OFS e JUFRA; funcionamento interno de áreas/distritos; estrutura de cargos; regras detalhadas de admissão, transferência ou desligamento; e regras de histórico de vínculos fraternos. Antes de implementar qualquer um desses comportamentos, consultar o responsável.

**Atenção:** regras descritas como habituais não devem ser convertidas em restrições absolutas. Havendo dúvida ou aparente conflito com uma nova regra, consultar o responsável antes de decidir.
