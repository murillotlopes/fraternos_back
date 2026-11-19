# Instruções para agentes de IA — Fraternos

## Fluxo de trabalho
- Conversar com o responsável para definir propósito, requisitos, regras de negócio e critérios de aceitação antes de implementar.
- Não presumir decisões de negócio. Em caso de dúvida, ambiguidade ou conflito, interromper a implementação afetada, explicar o problema e solicitar decisão explícita.
- Usar Git Flow: `main` é produção; `develop` integra funcionalidades; toda `feature/*` parte de `develop` e retorna por pull request. Não mesclar PRs sem aprovação do responsável.
- Não alterar código fora do escopo aprovado.

## Arquitetura e tecnologias
- Adotar Clean Architecture, arquitetura hexagonal, SOLID, baixo acoplamento e alta testabilidade.
- Manter regras de negócio independentes de frameworks, transporte, persistência e serviços externos; comunicar camadas por contratos/portas.
- Usar versões estáveis e suportadas, preferindo LTS quando aplicável e respeitando compatibilidade.
- Evitar bibliotecas externas para tarefas simples que APIs nativas resolvam com segurança. Adotar bibliotecas consolidadas quando implementar internamente trouxer riscos, como hashing de senhas com Argon2.
- Criar testes proporcionais às mudanças e informar os testes executados e suas limitações.

## Regras de negócio — fonte de verdade
- A documentação canônica de regras de negócio fica no repositório `murillotlopes/fraternos_back`, em `docs/business-rules/README.md` e nos documentos dessa pasta.
- **Antes de propor, alterar ou implementar qualquer regra**, consultar a documentação canônica atualizada no backend e as regras relacionadas.
- Verificar conflitos, contradições, sobreposições, dependências e efeitos sobre regras existentes.
- Havendo conflito, ambiguidade ou informação insuficiente, **perguntar ao responsável e aguardar sua decisão**. Não escolher silenciosamente uma interpretação.
- Após aprovação, atualizar a documentação no mesmo PR que implementar a regra, antes de considerar a tarefa concluída.
- Registrar cada regra com identificador estável, título, descrição normativa, condições, exceções (se houver), regras relacionadas e histórico de alterações.
- Não apagar nem alterar silenciosamente regras existentes; documentar substituições e decisões.
- Quando uma alteração atingir frontend e backend, manter ambos coerentes, mas preservar a documentação canônica no backend.

## Responsabilidades por repositório
- Este repositório contém o backend Node.js, Fastify e TypeScript.
- Priorizar APIs nativas do Node.js e recursos do Fastify.
- Organizar domínio, aplicação (casos de uso/portas) e infraestrutura (adaptadores) de forma independente e testável.
- Manter a documentação de regras de negócio versionada em `docs/business-rules/`.
