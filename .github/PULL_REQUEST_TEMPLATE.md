## 🔗 Work item

<!-- Link do ticket, issue ou tarefa relacionada (ex: Closes #N, Linear, Jira). -->

## 🎯 O que muda

<!-- A capacidade que entra, em linguagem de domínio: o que o time ou o usuário passa a poder fazer. -->

## 🧭 Por quê

<!-- Motivação e contexto: que problema resolve, o que já existia, o que dependia disso. Referencie a issue (Closes #N) quando houver. -->

## 🔧 Como

<!-- Artefatos e decisões que o revisor precisa entender para julgar o diff — não narrativa arquivo por arquivo. Inclua o "por quê" de cada escolha não óbvia. -->

## 🧪 Testes

<!-- O que foi escrito e rodado, com resultado: números da suíte, gates de CI, verificação manual quando aplicável. Se algo não foi verificado, diga explicitamente. -->

## 📸 Evidências

<!-- Screenshots, logs, saída de terminal ou gravação mostrando a alteração funcionando dentro do fluxo de sistema (local, development ou staging — não produção). Use apenas dados sintéticos ou mascarados — não cole saída com token, Authorization header, connection string, credencial ou PII. Obrigatório para mudanças visíveis ou comportamentais; escreva "N/A" apenas quando não houver evidência de execução significativa (ex.: mudanças de documentação, metadados ou configuração sem efeito em runtime). -->

## ⚠️ Risco

<!-- Segurança, invariantes, compatibilidade de dados/sessões, o que pode quebrar e como reverter. "Nenhum risco" é raro — prefira registrar o que foi considerado. -->

## 📌 Pendências conhecidas

<!-- Achados que não bloqueiam, dívida assumida de propósito e o que ficou fora de escopo. Escreva "Nenhuma" quando for o caso. -->

## ✅ Checklist

- [ ] Testes cobrindo o comportamento novo, escritos antes da implementação (RED → GREEN)
- [ ] Build, lint e testes locais rodados e limpos
- [ ] Commits atômicos, um por mudança lógica
- [ ] Diff revisado por mim; não há linha que eu não saiba explicar
