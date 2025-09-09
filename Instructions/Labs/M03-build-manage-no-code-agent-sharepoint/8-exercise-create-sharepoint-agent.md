À medida que as organizações dependem mais do SharePoint para gerenciar conhecimento, projetos e recursos de equipe, a capacidade de criar agentes inteligentes que interagem com esse conteúdo se torna um poderoso impulsionador de produtividade. O Microsoft 365 Copilot possibilita criar um agente do Copilot baseado no SharePoint que possa exibir rapidamente informações, responder perguntas e ajudar os usuários a navegar em conteúdos complexos do site. Este laboratório orienta você pelo processo de criação de seu próprio agente do Copilot conectado ao SharePoint, que compreende a estrutura e os dados de um site real que você usa todos os dias.

Por meio deste exercício prático, você irá aprender a criar um site do SharePoint, configurá-lo como uma fonte de dados e personalizar o comportamento e as respostas do agente. Desde o suporte à integração até o acompanhamento de projetos ou auxílio com recursos da equipe, você projeta e testa um agente adaptado às suas necessidades. Depois de concluir este laboratório, você deverá ter um agente do SharePoint em funcionamento e uma compreensão mais profunda de como a IA pode tornar o conteúdo do site mais acessível e acionável para os usuários em toda a sua equipe ou organização.

### Exercício

Neste exercício, você vai criar um agente do SharePoint para ajudá-lo a obter respostas rápidas ou executar ações úteis relacionadas a um site específico do SharePoint que você já usa. Por exemplo, um site de equipe, site de projeto ou hub de recursos.

1. Você deve começar identificando um site do SharePoint ao qual você já tem acesso. Para ajudá-lo a localizar um site, navegue até a home page do **Microsoft 365**, selecione **Aplicativos** no painel de navegação e, em seguida, selecione **SharePoint**. Examine os sites que aparecem no painel de navegação. O site que você selecionar deve, de preferência, conter documentos, listas ou páginas com informações de projetos, recursos da equipe ou outras fontes de conhecimento. Por exemplo:
   - Um site pessoal do OneDrive com documentos compartilhados.
   - Um site do SharePoint conectado ao Teams
   - Um projeto compartilhado ou site de departamento<br><br>

    > [!NOTE]
    > Se você não tiver acesso a um site que possa usar, crie um site básico do SharePoint para este laboratório ou junte-se a outro aluno que tenha acesso a um site.

1. Selecione o site do SharePoint que você deseja usar. 
1. Há quatro locais dos quais você pode iniciar o processo para criar um novo agente para um site:
     - A home page do site do SharePoint
     - A barra de comandos de uma biblioteca de documentos
     - O menu de contexto dos arquivos selecionados em uma biblioteca de documentos
     - O painel de chat do agente

    Para este laboratório, vamos usar a home page do site do SharePoint. Na home page do site, selecione **+Novo** e, no menu suspenso exibido, selecione **Agente**.

1. Na janela **Criar novo agente**, a ferramenta de agente do Copilot no SharePoint cria uma versão de rascunho do agente para o site selecionado. Observe como, no meio da janela, ele indica a origem desse agente (que é o site selecionado). Agora você deseja configurar o agente, portanto, selecione o botão **Editar**. Isso irá abrir o formulário **Editar agente**. 
1. O formulário **Editar agente** tem três guias : **Visão geral**, **Fontes** e **Comportamento**. A guia **Visão geral** é aberta primeiro por padrão. Nessa guia, você deve inserir o nome e a finalidade do agente. Os valores padrão são fornecidos para cada campo, mas você pode alterá-los agora, se desejar. 
1. A guia **Visão geral** também exibe o ícone padrão associado ao agente. Você pode selecionar a opção **Alterar** que aparece abaixo do ícone se quiser personalizá-la. O ícone do agente deve ser um arquivo .png que não exceda 1 MB de tamanho. Se você não tiver um ícone para usar, prossiga para a próxima etapa.
1. Neste estágio, observe como o botão **Salvar e fechar** está habilitado. Você pode selecioná-lo neste ponto, mas não faça isso ainda. Se você fizer isso, a ferramenta aceitará as fontes de conhecimento e os atributos de comportamento padrão para o seu agente. Isso também tornaria o agente ativo em vez de mantê-lo no modo de rascunho. Embora você ainda possa fazer alterações posteriormente, para os fins deste laboratório, vamos continuar trabalhando no modo de rascunho para configurar os atributos restantes do agente. Para fazer isso, selecione a guia **Fontes**.
1. A guia **Fontes** permite que você defina mais fontes para a versão de rascunho do seu agente. A fonte padrão para um agente do SharePoint é todo o site do SharePoint. Você pode ver essa opção no campo de fonte, onde o valor padrão é **Originado de todo o site**. Essa opção usa todas as fontes de dados neste site. No entanto, se você quiser selecionar fontes mais granulares, selecione esse campo e, no menu suspenso exibido, selecione **Originado de bibliotecas de documentos, pastas ou arquivos**. Você pode decidir qual opção de fonte você prefere. Se você selecionar a opção **Originado de bibliotecas de documentos, pastas ou arquivos**, então conclua as seguintes etapas:
   1. Quando você seleciona a opção **Originado de bibliotecas de documentos, pastas ou arquivos**, a seguinte opção aparece abaixo dela: **+Adicionar bibliotecas de documentos, pastas ou arquivos**. Selecione esta opção de menu, que exibe a janela **Selecionar itens**.
   1. A janela **Selecionar itens** exibe a pasta **Documentos** do site do SharePoint associado ao agente. Você tem duas opções para selecionar arquivos e pastas:
      - **Selecionar todos os arquivos e pastas na biblioteca Documentos**. Escolha o botão **Selecionar** para selecionar toda a biblioteca Documentos. Isso retorna a guia **Fontes** e exibe **Documentos** abaixo do campo **Originado de bibliotecas de documentos, pastas ou arquivos**.
      - **Selecionar arquivos e pastas específicos dentro da biblioteca documentos**. Quando você seleciona um ou mais arquivos ou pastas, uma marca de seleção é exibida ao lado dos arquivos e pastas selecionados. Isso retorna a guia **Fontes ** e exibe os arquivos e pastas selecionados abaixo do campo **Originado de bibliotecas de documentos, pastas ou arquivos**.
1. Depois de voltar à guia **Fontes**, você poderá selecionar a opção **+Adicionar bibliotecas de documentos, pastas ou arquivos** se quiser adicionar mais bibliotecas, arquivos ou pastas.
1. Depois de concluir a definição de suas origens, você deverá selecionar a guia **Comportamento**. A guia **Comportamento** permite definir uma mensagem de **Boas-vindas**, que é exibida quando um usuário seleciona esse agente no SharePoint. Este campo de mensagem está disponível em agentes do SharePoint, mas não em agentes do Copilot Chat. 
1. A partir daqui, você pode configurar até três prompts de início.
1. Por fim, você pode definir as instruções para o agente usando texto em linguagem natural, assim como faz ao criar um agente no Copilot Chat.
1. Quando terminar de fazer as alterações finais no agente do SharePoint, selecione o botão **Salvar e fechar** para salvar as alterações. Como você ainda estava no modo de rascunho, salvar a versão de rascunho do agente a converte em um agente do SharePoint ativo.
1. Selecione o **X** no canto superior da janela **Criar seu novo agente** para fechar. Fazer isso retorna você para a home page do site do SharePoint e o agente aparece no lado direito da janela. 
1. Reserve algum tempo para testar o agente. Você pode usar qualquer um dos prompts de início ou inserir prompts personalizados.
1. Se você quiser fazer alterações no agente, selecione o ícone de reticências no canto superior do painel do agente. No menu suspenso exibido, selecione **Editar agente**. Isso irá abrir a janela **Editar agente**, que é basicamente uma réplica da janela **Criar seu novo agente**. Navegue pelas guias para atualizar as propriedades que você deseja alterar e, em seguida, salve as alterações. 
