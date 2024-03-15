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

6. Tags:
Utilizamos tags para marcar releases significativas do projeto, facilitando o acompanhamento do progresso e a identificação de versões estáveis.
Para criar uma tag seguimos os passos abaixo:

Identificar o Commit Correspondente à Versão a Ser Marcada:
Revisamos o histórico de commits para identificar o commit que representa a versão que desejamos marcar com a tag.

Criar a Tag:
Utilizamos o comando git tag seguido pelo nome da tag e do identificador do commit. Por exemplo:
"git tag -a v1.0 -m "Versão 1.0""
O parâmetro "-a" cria uma tag anotada, que inclui informações adicionais como autor, data e mensagem.

Enviar a Tag para o Repositório Remoto:
Após criar a tag localmente, precisamos enviá-la para o repositório remoto usando o comando:
"git push origin <V1.0.0>"

Isso garante que a tag esteja disponível para outros colaboradores e para fins de referência futura.

7. Pull Requests:
Todas as contribuições foram enviadas ao repositório original via pull requests, com descrições claras do que cada uma adiciona ou modifica.
Abaixo estão os passos para criar uma pull request:

Criar uma Branch para a Feature ou Correção:
Antes de iniciar o trabalho, criamos uma nova branch a partir do branch principal utilizando "git checkout -b <nome_da_branch>".

Desenvolver as Alterações:
Implementamos as mudanças necessárias na nova branch, realizando commits conforme avançamos no desenvolvimento.

Sincronizar a Branch com as Atualizações do Branch Principal:
Regularmente, sincronizamos a nossa branch com as atualizações do branch principal utilizando "git pull origin <branch_principal>".

Criar a Pull Request:
No GitHub, navegamos até a página do repositório e selecionamos a nossa branch.
Clicamos no botão "New pull request".
Selecionamos o branch principal como destino da pull request e a nossa branch como origem.
Preenchemos uma descrição clara e informativa, explicando as alterações realizadas.

Rever e Discutir as Alterações:
Revemos a pull request, fornecendo feedback e sugestões através de comentários na interface do GitHub.

Realizar Modificações se Necessário:
Se forem solicitadas alterações adicionais, fazemos as modificações na nossa branch local e realizamos commits adicionais.

Integrar a Pull Request:
Uma vez aprovada e revista, realizamos a integração da pull request, mesclando as alterações no branch principal.

Fechar a Pull Request:
Após a integração das alterações, a pull request é fechada, indicando que o trabalho foi concluído com sucesso.
Seguindo estes passos, garantimos um processo de colaboração suave e organizado, permitindo que cada contribuição seja revista e integrada de forma eficiente à base de código principal.
