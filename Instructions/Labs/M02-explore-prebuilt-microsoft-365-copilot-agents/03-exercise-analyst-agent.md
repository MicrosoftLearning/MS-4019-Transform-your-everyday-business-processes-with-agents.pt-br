À medida que as organizações se tornam mais orientadas por dados, a capacidade de interpretar e comunicar rapidamente insights a partir de informações brutas é uma habilidade crítica. O agente Analista do Microsoft 365 Copilot capacita os usuários a fazer exatamente isso, analisando e visualizando dados diretamente em ferramentas familiares como Excel e Forms. Este laboratório fornece um passo a passo prático de como usar o agente Analista para entender os conjuntos de dados existentes, seja de pesquisas, planilhas ou resultados de pesquisas, e transformá-los em insights acionáveis com o mínimo de esforço.

Neste exercício baseado em cenário, você aprenderá a usar o agente Analista para explorar tendências, identificar anomalias e gerar visuais que aprimoram a narrativa de dados. Seja ao relatar o desempenho da equipe, o feedback de clientes ou métricas operacionais, este laboratório mostra como passar de números brutos para um resumo claro ou gráficos prontos para os stakeholders. É uma forma poderosa de economizar tempo, reduzir o esforço manual e aumentar a confiança em suas decisões analíticas com o suporte da IA.

### Exercício

Você tem a tarefa de analisar os resultados da pesquisa que pertencem a uma iniciativa interna da empresa chamada "Project Nexus", um programa piloto de seis semanas destinado a melhorar a colaboração entre departamentos por meio de uma nova plataforma de espaço de trabalho digital. O projeto envolveu funcionários de vários departamentos, incluindo TI, RH, Marketing e Operações, que foram solicitados a usar a plataforma para comunicação diária, compartilhamento de documentos e gerenciamento de tarefas. O objetivo do projeto era avaliar a eficácia da plataforma em aumentar a produtividade, agilizar a comunicação e cumprir os prazos do projeto. 

Após a conclusão do piloto, os participantes foram entrevistados para avaliar sua satisfação com o projeto, a clareza e eficácia da comunicação, a adesão ao cronograma proposto e sua experiência geral com o novo sistema. Você planeja usar o agente Analista pré-construído do Microsoft 365 Copilot para explorar os resultados da pesquisa do Project Nexus. Como acontece com qualquer agente pré-construído, você pode inserir seus próprios prompts personalizados ou usar os prompts iniciais do agente. Os prompts iniciais do agente Analista são projetados para produzir análises quantitativas, qualitativas e de visualização, além de insights e recomendações gerais do projeto.

Execute as seguintes etapas para direcionar o agente Analista a interpretar e visualizar os resultados da pesquisa em relação ao Project Nexus:

1. Selecione o link a seguir para baixar uma cópia dos resultados da pesquisa do [Project Nexus](https://github.com/MicrosoftLearning/MS-4004-Empower-workforce-copilot-use-cases/raw/refs/heads/master/ResourceFiles/Project_Nexus_survey_results.xlsx). Selecione o botão **Baixar** na parte superior da tela para baixar o arquivo para seu dispositivo.
1. No **Microsoft Edge**, abra uma nova guia e insira a seguinte URL: [**https://M365copilot.com**](https://M365copilot.com)
1. No **Microsoft 365**, selecione o agente **Analista** se ele aparecer no painel de navegação, na seção **Agentes**. Caso contrário, selecione **Todos os agentes** no painel de navegação e, na janela **Loja de agentes**, selecione **Analista** na seção **Criado pela Microsoft**. 
1. No **Microsoft 365**, a janela do agente **Analista** é exibida. No campo de prompt, selecione o ícone **Adicionar conteúdo e agentes**, que é o ícone de operador de adição (**+**). 
1. No menu exibido, selecione **Carregar deste dispositivo**. No **Explorador de Arquivos**, navegue até a pasta **Downloads** e selecione o arquivo **Resultados da Pesquisa do Project Nexus** que você baixou anteriormente e selecione **Abrir**. 
1. No campo de prompt, insira o seguinte prompt ao lado do arquivo Resultados da Pesquisa do Project Nexus vinculado: **Analise esta planilha e diga-me as três principais tendências**.

   > [!NOTE]
   > Observe como o Analista executa vários comandos Python para criar sua lista final de tendências. Pode ser necessário aguardar um minuto ou mais para que ele execute todos os comandos, agregue os resultados e determine as três principais tendências. Abaixo de cada comando há uma descrição dos resultados desse comando. Continue rolando para baixo nos resultados para ver as três principais tendências.
1. Você deseja detalhar cada categoria, portanto, comece inserindo o seguinte prompt: **Qual é a classificação média para cada categoria de pesquisa**?
1. Em nossos testes, o agente retorna o que parece ser uma página em branco. Na realidade, não se trata de uma página em branco; é apenas um grande espaço vazio entre a resposta do agente e o campo de prompt. Se a mesma coisa acontecer com você, role para cima usando a barra de rolagem vertical e você deverá encontrar a resposta. E se você rolar até a parte inferior da página, o campo de prompt deverá aparecer. Esse agente é novo, então parece que todo esse espaço vazio é um problema que precisa ser resolvido. Por outro lado, quando você fizer este exercício, esse problema do espaço em branco extra pode já ter sido corrigido. Em ambos os casos, examine os resultados. Se o agente Analista sugerir uma próxima etapa, como "Gostaria de uma comparação visual dessas médias?" então digite **Sim** no campo de prompt (se o problema de espaço em branco ainda persistir, você precisará rolar até a parte inferior da página para ver o campo de prompt).
1. Novamente, role para cima até os resultados do prompt anterior (se necessário) e examine-os.
1. Neste ponto, fique à vontade para gastar o tempo que quiser para analisar os resultados da pesquisa usando o agente Analista. Você pode inserir seus próprios prompts personalizados ou, se desejar, tente qualquer um desses prompts, dependendo do tipo de análise que você deseja executar:
   - Prompts de análise quantitativo:
      - **Qual categoria recebeu a classificação média mais alta e qual recebeu a menor**?
      - **Quantos participantes classificaram a satisfação do projeto como 4 ou superior**?
      - **Qual porcentagem de participantes avaliou a adesão ao cronograma abaixo de 3**?
      - **Você pode identificar quaisquer correlações entre a eficácia da comunicação e a experiência geral**?
   - Prompts de análise qualitativo:
      - **Resuma os temas mais comuns na seção de comentários**.
      - **Há alguma preocupação ou sugestão recorrente mencionada nos comentários**?
      - **Identifique os comentários que mencionam problemas com comunicação ou linha do tempo**.
   - Insights e prompts de recomendação:
      - **Com base nos dados da pesquisa, quais são os três principais pontos fortes do Project Nexus**?
      - **Quais são as principais áreas para melhoria sugeridas pelos participantes**?
      - **Forneça um relatório resumido das descobertas da pesquisa com recomendações acionáveis**.
   - Prompts de visualização quantitativos:
      - **Gere um gráfico de pizza da distribuição geral das classificações**.
      - **Crie um gráfico de barras comparando as médias das avaliações de Satisfação com o Projeto, Eficácia da Comunicação, Adesão ao Cronograma e Experiência Geral**.
      - **Plote um histograma das avaliações de satisfação para visualizar a distribuição das notas**.
      - **Gere um gráfico de dispersão para analisar a relação entre a Eficácia da Comunicação e a Experiência Geral**.
      - **Crie um mapa de calor de correlação para todas as categorias de avaliação numéricas**.
      - **Crie um diagrama de caixa para cada categoria de avaliação para mostrar o intervalo e os quartis**.
      - **Plote um gráfico de linha mostrando as avaliações de adesão ao cronograma dos participantes, ordenados por ID do Participante**.
