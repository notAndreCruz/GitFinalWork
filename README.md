# GitFinalWork
Este projeto tem como objetivo praticar e compreender os principais conceitos e práticas de colaboração no GitHub. 
Através da criação de um novo repositório e da realização de diversas tarefas, pretendemos familiarizar-nos com os fluxos de trabalho comuns, como criação de branches, commits, pull requests e resolução de conflitos. 
O projeto é simples e flexível, permitindo contribuições em diversas áreas, desde adicionar funcionalidades e corrigir bugs até melhorar a documentação.

1. Criação ou Seleção de um Repositório:
Optamos por criar um novo repositório para este projeto para ter controle total sobre a estrutura e configurações.

2. Clone Local:
Cada membro clonou o repositório para sua máquina local usando git clone.
Atualizamos regularmente nossos clones locais com git pull para manter a versão mais recente do código.


3. Distribuição de Tarefas:
As tarefas foram divididas entre os membros, garantindo que todos tivessem contribuições claras e significativas.


4. Utilização de Branches e Commits:
Criamos branches individuais para cada tarefa usando "git branch" e "git checkout -b".
Fizemos commits frequentes com mensagens descritivas usando "git commit".


5. Merges, Rebase e Cherry-Picks:
Para integrar as contribuições ao branch principal de forma eficiente, empregamos diversas estratégias:

Merges Diretos: Quando as contribuições eram independentes e não afetavam o mesmo conjunto de arquivos, realizamos merges diretos.
Para isso, garantimos que a branch de destino estivesse atualizada com as alterações mais recentes do branch principal, e então fizemos o merge utilizando "git merge <branch>".

Rebase: Em casos em que múltiplas branches estavam em desenvolvimento simultâneo e queríamos manter um histórico linear e organizado, optamos pelo rebase. 
Primeiro, nos certificamos de que a branch a ser rebased estava atualizada com o branch principal. Então, usamos "git rebase <branch_principal>" na branch a ser rebased para reorganizar os commits em relação ao branch principal.

Cherry-Picks: Para trazer alterações específicas de uma branch para outra, sem incorporar todas as mudanças presentes na branch de origem, recorremos aos cherry-picks. 
Identificamos o commit desejado na branch de origem e aplicamos esse commit na branch de destino usando "git cherry-pick <commit>".
