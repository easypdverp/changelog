# Histórico de Atualizações

## 22/09/2026

### 🚀 Novidades

**Exportações em segundo plano**
Agora é possível exportar listas grandes sem travar a tela. A exportação roda em segundo plano e você acompanha o progresso pela central de tarefas (ícone de sino). Quando o arquivo estiver pronto, basta baixar por lá. Disponível em praticamente todas as seções: Catálogo, Produtos, Vendas, Finanças, Suprimentos, Relatórios, Preferências e muito mais.

**Cenários fiscais por produto**
Cada produto agora pode ter cenários fiscais próprios, configurados diretamente no cadastro do produto. Ao adicionar um item em uma NF-e ou NFC-e, o cenário fiscal correto é aplicado automaticamente.

**Reforma Tributária (IBS/CBS e Imposto Seletivo)**
As telas de natureza de operação e cenário fiscal ganharam abas dedicadas para IBS/CBS e Imposto Seletivo, preparando o sistema para a Reforma Tributária.

**Relatório de Curva ABC de Vendas**
Novo relatório de vendas por curva ABC, permitindo identificar quais produtos concentram a maior parte do faturamento.

**Relatório de Vendas por Hora**
Novo relatório que mostra a distribuição das vendas ao longo do dia, hora a hora.

**Relatório de CMV (Custo da Mercadoria Vendida)**
Novo relatório de CMV disponível na seção de Relatórios.

**Nota de Devolução como NF-e de Saída**
A devolução de mercadoria agora gera uma NF-e de saída com finalidade "Devolução". O fluxo foi redesenhado em etapas e, ao salvar, você é direcionado direto para a nota gerada.

**Conferência de recebimento na Nota de Entrada**
Ao receber uma nota de entrada, agora é possível fazer a conferência dos itens diretamente na tela da nota.

**Abastecimento + Conferência (SUPPLY_CHECK)**
Nova modalidade de tarefa que combina abastecimento e conferência em um único fluxo.

**Acordo financeiro e repasse ao condomínio**
Novo módulo de acordo financeiro com condomínio, com leituras de medidor, apuração mensal e repasse por ponto de venda.

**Pesquisas de satisfação (CSAT) no CRM**
Nova seção de análise de pesquisas de satisfação no CRM, com lista, modal de resultados e editor dedicado.

**Suporte a CNPJ alfanumérico**
O sistema passou a aceitar CNPJs no novo formato alfanumérico, conforme a Instrução Normativa RFB 2.229/2024.

**Busca por leitura de código de barras nas tabelas**
Em telas compatíveis, é possível usar um leitor de código de barras para buscar registros diretamente na tabela.

**Horário de pico com média diária de vendas**
O widget de horário de pico no dashboard agora exibe a média diária de vendas faturadas por hora.

**Avatar com inicial do nome**
Usuários sem foto de perfil agora veem um avatar com a inicial do seu nome no lugar da imagem em branco.

**Configurações de regime tributário da empresa**
A tela de preferências da empresa ganhou campo para o regime tributário e a apuração do IRPJ, disponíveis tanto no cadastro inicial quanto na edição.

**Suporte a EAN-8 na detecção automática de etiquetas**
Códigos de barras EAN-8 agora são reconhecidos automaticamente.

**Série da nota travada após escolha**
A série escolhida ao criar uma NF-e ou NFC-e agora determina o número da nota e fica bloqueada durante a edição, evitando inconsistências.

**Filtro por tipo de arquivo no Gerenciador de Arquivos**
Agora é possível filtrar arquivos por tipo (imagem, vídeo, documento etc.) no gerenciador de arquivos.

**Planograma ordena por quantidade em estoque**
A lista de produtos no planograma agora abre ordenada pela maior quantidade em estoque.

**Terminal com empresa e servidor SiTef**
A tela de cadastro de terminal passou a exibir os campos de empresa e servidor SiTef, com assistente de criação redesenhado.

**Filtros e busca salvos na URL**
Filtros, página atual e termo de busca nas tabelas agora ficam salvos na URL. Ao voltar ou compartilhar o link, a tela abre exatamente com as mesmas configurações.

**Gráfico de telemetria por ponto de venda individual**
Agora é possível gerar o gráfico de telemetria para um único PDV.

**Sugestão de dígito verificador de GTIN**
Ao cadastrar um produto, o sistema sugere automaticamente o dígito verificador do código GTIN.

**Localização e categoria nas picklists e planograma**
As tabelas de picklist e planograma ganharam colunas de localização e categoria do produto.

---

### ✨ Melhorias

- **NFC-e:** Tela de contingência, reemissão em lote e política de ações agora disponível na interface.
- **NFC-e:** Relatório de validação na tela mostra inconsistências por item e impede autorização enquanto houver pendências.
- **NF-e:** As telas de nota de saída e entrada seguem o mesmo padrão visual e de funcionamento da NFC-e, com abas, confirmação de mudança de natureza e abertura em nova aba.
- **NF-e:** O número da nota não some nem pisca ao abrir as telas de saída, entrada e NFC-e.
- **NF-e:** Menu de ações das notas segue a política definida no servidor; filtro de operações disponível nas listas.
- **Promoções:** Novo fluxo de cadastro que começa pela escolha de um modelo, com suporte a grupos de itens e modos "a cada" ou "a partir de".
- **Exportação:** Ao exportar apenas a página atual, somente os itens visíveis na tela são enviados.
- **Produto:** Botão para copiar o código de barras direto da listagem de produtos.
- **Finanças:** Ponto de venda filtrado pela comunidade do contato nas contas a pagar/receber.
- **Finanças:** Largura da coluna Descrição limitada nas listas de contas a pagar e receber para melhor leitura.
- **Estoque:** Ao lançar estoque, o seletor de depósito exibe o nome da loja e o número do PDV.
- **Abastecimento:** Tabelas de separação, abastecimento e conferência sem rolagem horizontal no celular.
- **Preferências:** Campo de alíquota exibe vazio quando não há valor cadastrado, em vez de mostrar zero.
- **Espaço Contador:** O painel não trava mais quando uma tarefa de download não existe.
- **Categorias:** Links clicáveis de hierarquia (breadcrumb) na lista de categorias.
- **Listas de cadastro:** Clientes, fornecedores, funcionários, PDVs, terminais, listas de preço e comunidades agora têm linhas clicáveis para acesso rápido ao cadastro.
- **Agente de IA:** Eventos de progresso em tempo real durante interações com o assistente.
- **Dashboard:** Tooltip de horário de pico corrigido para usar singular quando a média é 1, e sem duplicação do "h" no horário.

---

### 🐛 Correções

- **Promoções:** Item do grupo não aparecia duplicado na linha; busca não mudava de posição ao digitar. Erros de validação aparecem somente após a primeira tentativa de salvar. Tipo "Valor fixo" agora é enviado corretamente ao servidor.
- **NF-e / NFC-e:** Diversas correções de alinhamento e consistência visual nas telas de nota de saída, entrada e NFC-e.
- **NFC-e:** Possibilidade de remover notas com status "negada", conforme permitido pelo servidor.
- **Exportação:** Caminho das categorias alinhado entre a tela e o arquivo exportado. Mensagens de erro do servidor exibidas de forma legível no modal, sem nomes técnicos.
- **Cenário fiscal:** Remoção de CFOP duplicado na aba ICMS.
- **Espaço Contador:** Painel de download não derruba mais o dashboard quando a tarefa não existe.
- **Discrepâncias de inventário:** Validação do campo "motivo" agora funciona corretamente.
- **Pesquisa de busca nas tabelas:** Pequeno "piscar" durante a digitação foi eliminado.
- **Picklist:** Contador principal desconta corretamente os itens removidos.
- **Relatório de CMV:** Placeholders exibidos enquanto o relatório carrega.
- **Gerenciador de arquivos:** Arquivos de vídeo e outros formatos agora exibem o tipo correto.

## 22/09/2026

### 🚀 Novidades

- **Exportação em segundo plano:** agora você pode exportar listas grandes sem precisar aguardar na tela. A exportação roda em segundo plano e você é avisado quando o arquivo estiver pronto — basta baixar pela nova aba "Tarefas" no sino de notificações.
- **Exportação completa pelo sistema:** todas as seções da plataforma (Catálogo, Produtos, Vendas, Suprimentos, Finanças, Relatórios, Preferências, Espaço Contador, Espaço Gestor e mais) agora exportam os dados diretamente pelo servidor, sem limitação de linhas.
- **Cenários fiscais por produto:** é possível vincular e gerenciar cenários tributários diretamente no cadastro do produto, na aba Fiscal.
- **Reforma Tributária (IBS/CBS e IS):** os cadastros de Natureza de Operação e Cenário Fiscal agora contemplam os novos impostos da Reforma Tributária — IBS, CBS e Imposto Seletivo.
- **NF-e de Devolução:** a devolução de mercadoria agora gera uma NF-e de saída com finalidade "Devolução", com fluxo guiado em etapas. Ao salvar, você é direcionado diretamente para a nota criada.
- **Conferência de recebimento na nota de entrada:** ao receber uma nota de entrada, é possível realizar a conferência dos itens diretamente pela tela da NF-e.
- **Contingência, reemissão em lote e política de ações na NFC-e:** novas opções para gerenciar notas em contingência, reemitir em lote e configurar a política de ações da NFC-e.
- **Relatório de Curva ABC de vendas:** novo relatório para identificar os produtos mais e menos representativos nas vendas.
- **Relatório de CMV (Custo da Mercadoria Vendida):** novo relatório de custo de mercadoria vendida, com exportação e filtros alinhados ao padrão do sistema.
- **Relatório de vendas por hora:** novo relatório que mostra a distribuição das vendas ao longo do dia.
- **Acordo financeiro e repasse de condomínio:** nova funcionalidade para registrar acordos financeiros com condomínios, leituras de medidor, apuração mensal e repasse por ponto de venda.
- **Pesquisas de satisfação (CSAT):** nova área no CRM com lista, resultados e editor de pesquisas de satisfação.
- **Abastecimento com Conferência:** nova tela de Abastecimento + Conferência (SUPPLY_CHECK) no fluxo de suprimentos.
- **Avatar com inicial do nome:** quando o usuário não tem foto de perfil, o avatar exibe a inicial do seu nome.
- **Suporte a CNPJ alfanumérico:** a plataforma agora aceita o novo formato de CNPJ alfanumérico (IN RFB 2.229/2024).
- **Leitura de código de barras para busca:** tabelas com suporte à leitura de código de barras (incluindo EAN-8) para localizar itens rapidamente.
- **Filtros, paginação e busca salvos na URL:** ao navegar entre páginas, os filtros, a paginação e o termo de busca aplicados são mantidos na URL, permitindo compartilhar ou retomar exatamente onde parou.
- **Gráfico por ponto de venda individual:** agora é possível gerar gráficos de telemetria filtrando por um único ponto de venda.
- **Regime tributário nas preferências da empresa:** campo para informar o regime tributário diretamente nas preferências da empresa.
- **Apuração do IRPJ:** o sistema agora coleta a apuração do IRPJ no cadastro e na edição da empresa.
- **Sugestão de dígito verificador de GTIN:** ao cadastrar o código de barras de um produto, o sistema sugere automaticamente o dígito verificador correto.
- **Copiar código de barras na listagem de produtos:** nova ação para copiar o código de barras diretamente da lista de produtos.
- **Série travada após criação da nota:** a série escolhida ao criar um rascunho de NF-e ou NFC-e determina o número da nota e fica bloqueada durante a edição, evitando inconsistências.
- **Planograma ordenado por estoque:** a lista de produtos do planograma agora abre com os itens de maior estoque primeiro.
- **Horário de pico com média diária:** o painel de horário de pico agora exibe a média diária de vendas faturadas naquele período.
- **Origem do produto obrigatória:** o campo de origem do produto passou a ser obrigatório no cadastro e na importação do catálogo.

---

### ✨ Melhorias

- **Validação de inconsistências na NFC-e:** a tela de NFC-e exibe um relatório de inconsistências por item antes de autorizar, com indicações claras do que precisa ser corrigido.
- **Natureza de operação com confirmação:** ao alterar a natureza de operação em uma nota, o sistema pede confirmação antes de recalcular os dados fiscais dos itens.
- **Número da nota sem piscar:** o número da NF-e e NFC-e não some nem pisca ao abrir as telas de saída, entrada ou NFC-e.
- **Menu de ações das notas seguindo política do backend:** as ações disponíveis para cada nota (ex.: remover nota negada) agora respeitam as regras definidas pelo servidor.
- **Filtro de operações nas listagens de notas fiscais:** as listas de NF-e e NFC-e agora permitem filtrar por tipo de operação.
- **Seleção de tipo de abastecimento com cartões visuais:** na picklist, o tipo de abastecimento é selecionado com cards visuais, mais fáceis de usar.
- **Localização e categoria nas picklists e planograma:** as tabelas de picklist e planograma agora exibem as colunas de localização e categoria dos produtos.
- **Depósito com nome da loja e número do PDV:** no lançamento de estoque, o seletor de depósito agora exibe o nome da loja e o número do PDV para facilitar a identificação.
- **Tabelas de suprimentos sem scroll horizontal no celular:** as tabelas de separação, abastecimento e conferência agora se adaptam melhor a telas menores.
- **Contador de itens na picklist descontando remoções:** o contador principal da picklist agora reflete corretamente os itens removidos.
- **Linhas clicáveis nas listagens:** nas listas de Clientes, Fornecedores, Funcionários, Pontos de Venda, Terminais, Tabelas de Preço, Comunidades e Categorias, basta clicar na linha para abrir o cadastro.
- **Busca nas tabelas com resposta mais suave:** a busca nas tabelas passou a ter um pequeno atraso inteligente, evitando o piscar de carregamento a cada letra digitada.
- **Promoção com grupos e modos "a cada" ou "a partir de":** o cadastro de promoções foi reestruturado com suporte a múltiplos grupos e dois modos de aplicação de desconto.
- **Promoção iniciada por modelo:** o fluxo de criação de promoções agora começa pela escolha de um modelo, simplificando a configuração.
- **Gerenciador de arquivos com rótulos para vídeo e outros anexos:** vídeos e arquivos genéricos agora recebem rótulos identificadores no gerenciador de arquivos.
- **Assistente de chat com progresso em tempo real:** o chatbot agora exibe o progresso das respostas em tempo real enquanto processa.
- **Campo de alíquota vazio quando sem valor:** nas preferências fiscais, o campo de alíquota agora aparece vazio quando não há valor cadastrado, em vez de exibir zero.
- **Empresa e servidor SiTef no cadastro do terminal:** o terminal agora exibe e permite editar as informações de empresa e servidor SiTef.
- **Ponto de venda filtrado pela comunidade do contato:** nas contas a pagar e a receber, o ponto de venda é automaticamente filtrado pela comunidade do contato selecionado.

---

### 🐛 Correções

- **Dashboard sem erro ao baixar tarefas inexistentes:** o painel do Espaço Contador não trava mais quando a tarefa de download não existe.
- **Tooltip de horário de pico com texto correto:** corrigido o texto do tooltip que mostrava "h" duplicado e usava plural quando a média era 1.
- **Exportação com caminho de categorias correto:** o caminho das categorias nos arquivos exportados agora é consistente entre o que o sistema exibe e o que é gerado no arquivo.
- **Mensagens de erro na exportação sem código técnico:** quando o servidor recusa uma exportação, a mensagem exibida no modal agora está em linguagem clara, sem nomes técnicos internos.
- **Promoção "Valor fixo" funcionando corretamente:** a opção de desconto por valor fixo nas promoções agora é enviada com o valor correto para o servidor.
- **Erro de validação na promoção aparece só após o primeiro salvamento:** a mensagem de erro no cadastro de promoção não aparece mais antes de você tentar salvar pela primeira vez.
- **Grupo de promoção sem repetição de item:** a linha do grupo de promoção não duplica mais itens, e a busca não muda de posição durante a navegação.
- **Cenário fiscal sem CFOP duplicado:** removida a duplicidade do campo CFOP na aba ICMS do cenário fiscal.
- **Preferências de NF-e sem opção desnecessária:** removida uma opção sem uso das preferências de nota fiscal.
- **Seleção em tabelas sem perda ao navegar entre páginas:** a seleção de itens nas tabelas agora é mantida corretamente ao mudar de página.
- **Validação do motivo de discrepâncias de quantidade corrigida:** o comportamento da validação do motivo de discrepâncias no inventário foi corrigido.

## 11/09/2026

### 🚀 Novidades

- **Emissão de NF-e e NFC-e completa:** agora é possível gerenciar todo o ciclo de vida das suas notas fiscais diretamente pela plataforma, incluindo emissão, cancelamento e inutilização.
- **Contingência offline:** caso haja instabilidade na comunicação com a Sefaz, o sistema passa automaticamente para o modo de contingência, garantindo que suas vendas não sejam interrompidas.
- **Nota de devolução:** emita notas de devolução de forma simples e integrada ao fluxo de vendas.
- **Cenários tributários:** suporte a diferentes configurações tributárias, facilitando a adequação do sistema à realidade fiscal do seu negócio.
- **Relatórios de vendas aprimorados:** novos dados fiscais integrados aos relatórios, oferecendo uma visão mais completa das suas vendas.

---

## 24/07/2026

### 🚀 Novidades

- **Assistente inteligente com respostas em tempo real:** o chatbot da plataforma agora exibe as respostas conforme elas são geradas, tornando a conversa mais fluida e natural.
- **Assistente consulta promoções:** o assistente virtual agora consegue buscar e informar sobre as promoções cadastradas na sua loja, ajudando você a tirar dúvidas rapidamente sem sair do chat.

## 24/07/2026

### 🚀 Novidades

- **Assistente com respostas em tempo real:** o chatbot agora exibe as respostas enquanto ainda está processando, tornando a conversa mais fluida e rápida. Além disso, ele passou a entender perguntas sobre **promoções**, podendo consultá-las e sugeri-las diretamente no chat.

---

## 22/07/2026

### 🐛 Correções

- **Segurança ao redefinir senha:** ao redefinir sua senha, todas as sessões abertas em outros dispositivos são encerradas automaticamente, garantindo mais segurança para a sua conta.

## 22/07/2026

### 🐛 Correções

- Ao redefinir sua senha, todas as sessões abertas em outros dispositivos agora são encerradas automaticamente, aumentando a segurança da sua conta.

---

## 20/07/2026

### 🚀 Novidades

- Melhorias no gerenciamento de cenários fiscais e promoções, tornando as configurações tributárias e ofertas mais precisas e confiáveis.

### ✨ Melhorias

- Ao redefinir sua senha, suas sessões em outros dispositivos são desconectadas automaticamente para proteger o acesso à sua conta.

## 20/07/2026

### 🚀 Novidades

- **Cenários fiscais aprimorados:** agora é possível configurar e gerenciar cenários de tributação com mais flexibilidade, garantindo maior precisão nas operações fiscais.
- **Melhorias nas promoções:** novas opções de gerenciamento de promoções disponíveis para facilitar a criação e o controle das suas ofertas.

### ✨ Melhorias

- **Mais segurança na redefinição de senha:** ao redefinir sua senha, todas as sessões abertas em outros dispositivos são encerradas automaticamente, protegendo o acesso à sua conta.

## 20/07/2026

### 🚀 Novidades

- **Cenários fiscais e promoções aprimorados:** melhorias no tratamento de cenários de impostos e promoções nos pedidos.

### 🔒 Segurança

- Ao redefinir a senha, todas as sessões ativas do usuário são encerradas automaticamente, aumentando a segurança da conta.

---

## 29/06/2026

### 🚀 Novidades

- **Painel de PDVs em tempo real:** novo painel de monitoramento dos pontos de venda com atualização automática a cada 10 segundos, contador de vendas animado e indicador de status ao vivo.
- **Modo tela cheia no painel de PDVs:** agora é possível expandir o painel de telemetria para tela cheia, ideal para exibição em monitores dedicados.
- **Detalhes do PDV em modal:** clique em um terminal para ver informações detalhadas sobre conectividade, status e métricas de venda sem sair da tela.

### ✨ Melhorias

- A ordenação das colunas nas tabelas foi corrigida e agora funciona corretamente em todas as listagens.
- Os números animados no painel de vendas em tempo real não travam mais ao serem interrompidos — a animação retoma de onde parou.

### 🐛 Correções

- Corrigido problema que podia travar a tela ao carregar uma nova versão da plataforma — agora um botão de recarregamento é exibido automaticamente nesses casos.
- Ao redefinir a senha, todas as sessões ativas do usuário passam a ser encerradas corretamente, garantindo mais segurança.

## 29/06/2026

### 🚀 Novidades

- **Painel de PDVs ao vivo:** o painel de terminais de venda ganhou uma visualização completamente reformulada, com contador de vendas animado, indicador de status em tempo real e modo tela cheia para acompanhamento no salão ou retaguarda.
- **Atualização automática do painel:** os dados do painel de PDVs agora se atualizam automaticamente a cada 10 segundos, sem precisar recarregar a página.
- **Detalhes do PDV em modal:** agora é possível clicar em um terminal para ver informações detalhadas diretamente em uma janela, sem sair da tela.

### ✨ Melhorias

- **Gestão de inventário:** melhorias na busca e nos filtros do gerenciamento de estoque, tornando mais fácil localizar e organizar os itens do inventário.
- **Ordenação de tabelas:** a ordenação das colunas nas listagens foi corrigida para funcionar de forma mais precisa e consistente.

### 🐛 Correções

- Corrigido um problema em que o contador animado de vendas podia "travar" se a atualização fosse interrompida no meio.
- Corrigido um erro que podia ocorrer ao abrir ações em linhas da lista de NF-e de entrada.
- Ao ocorrer uma falha de carregamento na plataforma, agora é exibida uma mensagem clara com a opção de recarregar a página manualmente.

## 25/06/2026

### 🐛 Correções

- Corrigido um erro que impedia algumas ações na lista de NF-e de entrada

---

## 24/06/2026

### 🚀 Novidades

- **NF-e de entrada:** nova tela de lançamento de estoque completamente reformulada, com comparação lado a lado entre os itens da nota e os produtos do seu catálogo — facilitando a identificação e vinculação de cada item
- **NF-e de entrada:** agora é possível baixar o XML e o DANFE diretamente da lista de notas de distribuição
- **NF-e de entrada:** informações detalhadas sobre valor, remetente, chave de acesso e datas da nota agora ficam disponíveis em painéis de tooltip diretamente na lista
- **Pedidos de compra, venda e NFC-e:** lançamento de estoque integrado ao novo fluxo unificado de lançamento em lote
- **Catálogo:** linhas da tabela agora são clicáveis para abrir o produto; formulário de categoria abre em modal diretamente pela URL
- **Lista de produtos:** exibe há quanto tempo o produto foi atualizado, com data e hora exatas ao passar o mouse

### ✨ Melhorias

- **Filtros nas tabelas:** os filtros aplicados agora aparecem como etiquetas removíveis na barra de ferramentas, facilitando a visualização e remoção de cada filtro individualmente
- **Paginação:** o rodapé das tabelas agora exibe o intervalo de registros sendo visualizado (ex.: "1–20 de 150")
- **Lista de produtos:** visual mais compacto e organizado
- **NF-e de entrada:** indicação visual de carregamento ao importar uma nota de distribuição
- **Fornecedores e comunidades:** endereço agora é opcional no cadastro e edição
- **Lançamento de estoque:** itens da nota exibem etiqueta indicando se o produto foi identificado por EAN ou por SKU do fornecedor
- **NF-e de saída e NFC-e:** a opção de lançar estoque só aparece para notas autorizadas

### 🐛 Correções

- **Segurança:** ao redefinir a senha, todas as sessões ativas da conta são encerradas automaticamente
- **Pedidos de compra:** a lista é atualizada corretamente após um lançamento de estoque bem-sucedido
- **Pedidos de compra:** o SKU do fornecedor agora é usado corretamente na identificação dos itens durante o lançamento
- **Contatos:** validação do campo de estado do endereço corrigida
- **Lançamento em lote:** estado do modal é reiniciado corretamente ao reabri-lo
- Ajustes nas dimensões de imagens em diversas telas

## 24/06/2026

### 🐛 Correções

- Ao redefinir sua senha, todas as sessões ativas da sua conta são encerradas automaticamente, garantindo mais segurança no acesso.

## 19/06/2026

### 🐛 Correções

- Ao redefinir sua senha, todas as sessões ativas da sua conta são encerradas automaticamente, aumentando a segurança do acesso.

---

## 18/06/2026

### 🚀 Novidades

- **Guia de primeiros passos:** um novo widget flutuante aparece na tela inicial para te guiar pelas etapas de configuração da plataforma, com progresso por nível e a possibilidade de reabrir o guia quando quiser.
- **Notificações push:** agora é possível enviar notificações push diretamente pelo painel, com um novo botão de envio acessível pelo sino de notificações no topo da tela.
- **NF-e de entrada:** novos modais para editar, adicionar e cadastrar produtos diretamente a partir dos itens de uma nota fiscal de entrada, facilitando a conciliação do seu estoque.
- **Reconciliação de produtos (NF-e):** ao importar uma nota fiscal, o sistema agora identifica automaticamente os produtos e permite vincular a um produto existente, criar um novo ou ignorar itens que não são para revenda.
- **NF-e automática:** notas fiscais destinadas ao seu CNPJ agora são capturadas e registradas automaticamente, sem necessidade de ação manual.
- **Novas preferências:** páginas de configuração de separação e preferências do usuário foram adicionadas, com mais opções de personalização do sistema.
- **Configuração de permissões:** nova seção de configuração de permissões disponível nas configurações do sistema.

### ✨ Melhorias

- As tabelas e listas em toda a plataforma foram redesenhadas com um visual mais moderno, limpo e com indicadores de status coloridos em diversas seções (vendas, finanças, cadastros, notificações, relatórios e outras).
- Os campos de busca de NCM, CEST e CFOP agora contam com modais de criação integrados, agilizando o cadastro fiscal de produtos.
- O menu do usuário no cabeçalho foi aprimorado e agora fecha automaticamente ao clicar fora dele.
- O sistema passou a iniciar mais rapidamente graças a otimizações internas no carregamento de dados.

### 🐛 Correções

- Corrigido um problema em que a seção de notícias na tela inicial podia travar caso a resposta do servidor viesse em formato inesperado.
- Na tela de envio de notificação push, o seletor de ponto de venda agora aparece apenas quando necessário, evitando confusão.
- Resolvido um erro em que o campo de título vazio na notificação push gerava um identificador incorreto ao regenerar.

## 18/06/2026

### 🚀 Novidades

- **Guia de primeiros passos:** um novo widget flutuante aparece na tela inicial para guiar você pelas etapas de configuração da plataforma. Acompanhe seu progresso em cada fase e retome de onde parou a qualquer momento.
- **Envio de notificações push:** agora é possível enviar notificações push diretamente pelo sino de notificações no cabeçalho da plataforma, sem precisar navegar até outra página.
- **Reconciliação de NF-e de entrada:** ao importar uma nota fiscal de entrada, o sistema agora identifica automaticamente os produtos e permite vincular itens da nota a produtos já cadastrados, criar novos produtos ou ignorar itens que não são para revenda.
- **Criação de NCM, CEST e CFOP diretamente nos formulários:** ao preencher dados fiscais de produtos, você agora pode criar ou buscar códigos NCM, CEST e CFOP sem sair da tela atual.
- **Novas páginas de preferências:** foram adicionadas páginas de configuração de separação e preferências de usuário, com novas opções de personalização.
- **Configuração de permissões:** nova tela de configuração de permissões disponível nas configurações da plataforma.
- **NF-e com ciência automática:** notas fiscais eletrônicas recebidas agora geram a manifestação de ciência da operação automaticamente ao serem descobertas.

### ✨ Melhorias

- **Visual das tabelas atualizado:** todas as listagens da plataforma (vendas, financeiro, catálogo, estoque, relatórios, notificações, preferências e outras) receberam um novo visual mais moderno e organizado, com indicadores de status coloridos.
- **Indicadores de status nas listas:** as listas agora exibem etiquetas coloridas de status, facilitando a identificação rápida de cada registro.
- **Telemetria e análises aprimoradas:** novos componentes de telemetria foram adicionados ao painel, trazendo mais informações sobre o uso da plataforma.
- **Login com Google e Apple mais confiável:** a autenticação social foi aprimorada para maior estabilidade e segurança.
- **Mais sessões simultâneas permitidas:** o limite de sessões ativas por usuário foi aumentado, reduzindo desconexões inesperadas.

### 🐛 Correções

- **Notificações push:** a seleção de terminal agora aparece apenas quando o destino correto é escolhido, evitando confusão no formulário de envio.
- **Notificações push:** ao recriar uma notificação sem título, o sistema não gerava o identificador corretamente — isso foi corrigido.
- **Tela inicial:** a seção de novidades não exibia nada quando a resposta do servidor vinha em formato inesperado — corrigido para evitar tela em branco.
- **NF-e de entrada:** a associação de produtos da nota ao estoque agora verifica corretamente se todos os itens foram reconciliados antes de permitir a entrada.
- **Relatórios fiscais:** os relatórios de operações agora agrupam e descrevem os CFOPs corretamente.

## 18/06/2026

### 🚀 Novidades

- **Guia de primeiros passos:** um novo widget flutuante aparece na tela inicial para guiar você pelas etapas essenciais de configuração da plataforma. Acompanhe seu progresso por níveis, marque tarefas concluídas e retome de onde parou a qualquer momento.
- **Envio de notificações push:** agora é possível criar e enviar notificações push diretamente pelo painel, escolhendo o aplicativo de destino e o terminal desejado. O botão de envio fica disponível tanto no menu de notificações quanto na página de listagem.
- **Reconciliação de NF-e de entrada:** ao importar uma nota fiscal de entrada, o sistema agora reconhece automaticamente os produtos e oferece ações para vincular a um produto existente, cadastrar um novo produto ou marcar o item como não destinado à revenda.
- **Cadastro de NCM, CEST e CFOP direto na nota:** ao editar itens de uma NF-e de entrada, você pode pesquisar e criar códigos NCM, CEST e CFOP sem sair da tela.
- **NF-e automática (auto-ciência):** novas notas fiscais destinadas ao seu CNPJ agora são reconhecidas e registradas automaticamente no sistema.

### ✨ Melhorias

- As tabelas de listagem em toda a plataforma foram redesenhadas com um visual mais moderno, organizado e com indicadores de status mais claros.
- O menu do usuário no cabeçalho agora fecha automaticamente ao clicar fora dele.
- Novos campos de configuração adicionados nas preferências de separação e preferências do usuário.
- Novas opções de permissões disponíveis nas configurações do sistema.

### 🐛 Correções

- Corrigido problema em que a seleção de terminal aparecia indevidamente ao enviar notificações push para destinos que não eram o aplicativo do ponto de venda.
- Corrigido erro que gerava um timestamp incorreto ao tentar recriar uma notificação push com o título em branco.
- Corrigida exibição de gráficos na tela inicial que falhava quando a API retornava dados em formato inesperado.

---

## 22/05/2026

### 🚀 Novidades

- A seção de novidades da tela inicial agora é carregada dinamicamente a partir de uma fonte de conteúdo atualizada.
- Suporte completo ao envio de notificações push via Firebase Cloud Messaging, com agendamento, filtro por aplicativo de destino e por terminal.

---

## 30/04/2026

### 🚀 Novidades

- **Ocorrências de vendas:** novo módulo para registrar e gerenciar ocorrências relacionadas a vendas, com lista, detalhes, histórico de comentários, evidências com upload de imagens/vídeos e ações de conversão.
- **Galeria de imagens com editor:** agora é possível visualizar, anotar e baixar imagens de evidências diretamente no painel, com ferramentas de desenho, recorte, rotação e desfazer.
- **Reprodução de vídeos:** a galeria de mídia passou a suportar a visualização de vídeos.
- **Listas de preços — ações em lote:** novas opções para aplicar markup em massa (geral ou por categoria), remover itens em lote e duplicar uma lista de preços inteira.
- **Promoções:** novo módulo de gestão de promoções com criação, edição e exclusão.
- **Relatório de perda de produtos:** novo relatório disponível para acompanhamento de perdas no estoque.
- **Eventos de webhook:** nova página para visualizar os eventos recebidos via webhook.
- **Notificações em lote:** agora é possível marcar várias notificações como lidas ou removê-las de uma só vez.
- **Envio de NFC-e por SMS:** o link para download da NFC-e agora pode ser enviado por SMS ao cliente.

### ✨ Melhorias

- **Inventário:** nova opção para zerar as quantidades de produtos não contados ao iniciar uma conferência, e nova seleção de período dos últimos inventários a considerar.
- **Planograma:** filtros aprimorados e melhorias visuais na impressão de etiquetas.
- **Gráficos:** tooltips e legendas mais detalhados para facilitar a leitura dos dados.
- **Impressão de etiquetas:** melhorias na validação e nas opções de impressão.
- **Ponto de venda:** um PDV agora pode ter múltiplos terminais associados.

### 🐛 Correções

- Corrigido erro que podia salvar uma ocorrência em duplicidade ao editar a descrição de uma evidência.
- Corrigido problema de fuso horário na exibição de datas em ocorrências vinculadas a cobranças.
- Corrigido erro na aplicação de cupons de desconto em pedidos de venda com valores nulos.
- Corrigido problema ao atualizar promoções com condições específicas.
- Corrigida exibição de valores nulos nos gráficos do painel.

## 30/04/2026

### 🚀 Novidades
- **Editor de Imagens**: Nova funcionalidade para editar evidências de ocorrências diretamente no sistema, com ferramentas para desenhar, recortar, girar e fazer download das imagens editadas
- **Player de Vídeo**: Adicionado suporte para visualização de vídeos na galeria de evidências
- **Ocorrências de Vendas**: Novo módulo completo para gestão de ocorrências com criação, listagem, detalhamento e conversão para pedidos
- **Promoções**: Sistema completo de gestão de promoções com operações CRUD
- **Webhook Events**: Nova funcionalidade para monitoramento e gestão de eventos webhook
- **Lista de Preços**: Implementadas operações em lote como aplicar markup por categoria, remover itens e duplicar listas
- **Relatório de Perdas**: Novo relatório disponível para análise de produtos com perdas
- **SMS para NFC-e**: Envio automático de link para download da NFC-e via SMS

### ✨ Melhorias
- **Dashboard**: Gráficos aprimorados com tooltips e legendas mais informativos, além de controle de acesso baseado em permissões
- **Inventário**: Adicionada opção para zerar quantidades de produtos não conferidos e seleção de dias do último inventário
- **Notificações**: Implementadas ações em lote para marcar como lidas e remover notificações
- **Etiquetas**: Melhorias na funcionalidade de impressão com validação aprimorada
- **Exportação de Dados**: Sistema configurável para exportação de dados implementado
- **Upload de Arquivos**: Configuração aprimorada com suporte a diferentes tipos de arquivos

### 🐛 Correções
- **Dashboard**: Corrigido tratamento de valores nulos em gráficos
- **Ocorrências**: Corrigidos problemas de fuso horário em datas e prevenção de duplo salvamento
- **Planograma**: Corrigidos problemas de mapeamento de campos
- **Sistema**: Melhorias gerais de estabilidade e performance

## 22/04/2026

### ✨ Melhorias
- **Produtos**: Otimizada lógica de mapeamento GTIN para melhor performance
- **Terminal e Planograma**: Aprimoradas opções de filtro na interface

## 20/04/2026

### 🚀 Novidades
- **Ocorrências de Vendas**: Implementado sistema completo de gestão com funcionalidades de soft-delete e histórico
- **Múltiplos GTINs**: Produtos agora suportam múltiplos códigos GTIN para maior flexibilidade
- **Validação GTIN**: Nova validação para códigos GTIN em NF-e

### ✨ Melhorias
- **Planograma**: Melhorias na funcionalidade de etiquetas com novos filtros
- **PDV**: Aprimoramentos nos filtros e seleções

### 🐛 Correções
- **Busca**: Corrigidos caracteres especiais em pesquisas
- **Comentários**: Validação aprimorada para conteúdo não vazio
- **Sistema**: Melhor tratamento de erros e logs mais informativos

## 11/04/2026

### ✨ Melhorias
- **Planograma**: Melhorias na interface e funcionalidades de etiquetagem
- **Sistema**: Aprimoramentos gerais de performance e estabilidade

## 08/04/2026

### ✨ Melhorias
- **PDV**: Melhorias no mapeamento e nomenclatura de métodos
- **Sistema**: Atualização de dependências e otimizações gerais

## 08/04/2026

🐛 **Correções**
- Melhorada a sincronização de dados do painel administrativo e inventário

## 26/03/2026

🚀 **Novidades**
- Sistema completo de gestão de promoções no painel administrativo

🐛 **Correções**
- Aprimorada a lógica de criação de usuários
- Corrigido o login com Apple

## 25/03/2026

🚀 **Novidades**
- Funcionalidade de transferência entre estoques
- Nova opção para excluir contas de clientes

🐛 **Correções**
- Melhoradas as interfaces de gestão de inventário
- Corrigido o sistema de emissão de notas fiscais para vendas de clientes

## 23/03/2026

🚀 **Novidades**
- Sistema completo de emissão de NFC-e (Nota Fiscal do Consumidor Eletrônica)
- Novos modais e funcionalidades de relatórios de inventário

🐛 **Correções**
- Melhorado o sistema de geração de relatórios

## 20/03/2026

🚀 **Novidades**
- Busca de estabelecimentos por localização (coordenadas GPS)
- Mapeamento de unidades de conversão para produtos
- Funcionalidades de aprovação e cancelamento em lote para compras
- Filtros por categoria nas entradas de estoque

🛠️ **Melhorias**
- Funcionalidade de exclusão em lote para itens do sistema
- Melhorado o sistema de atualização de datas

## 20/03/2026

🚀 **Novidades**
- Nova funcionalidade de histórico de preços dos produtos para acompanhar variações ao longo do tempo
- Suporte para conversão entre diferentes unidades de medida dos produtos
- Filtros por coordenadas geográficas para pontos de venda

✨ **Melhorias**
- Aprimoramento no gerenciamento de inventário com novos componentes visuais
- Melhorias na aprovação e cancelamento de compras em lote
- Otimização dos filtros de entrada de produtos no estoque

## 19/03/2026

🚀 **Novidades**
- Sistema completo de histórico de preços implementado para melhor controle de custos

## 13/03/2026

🐛 **Correções**
- Corrigidos problemas de layout e funcionamento na página de verificação de inventário
- Removida obrigatoriedade da data de fabricação para lotes no inventário

✨ **Melhorias**
- Atualizações na API do cliente e melhorias na organização dos dados
- Filtros de tarefas de inventário agora permitem busca por nome do inventário

## 09/03/2026

✨ **Melhorias**
- Nova funcionalidade de exportação reformulada para melhor performance

🐛 **Correções**
- Correções na normalização de códigos NCM, CEST e CFOP
- Atualização nas credenciais de autenticação OAuth do Google e Apple
- Corrigido problema de entrada duplicada no planograma

## 07/03/2026

🐛 **Correções**
- Correção na exibição de imagens públicas no painel principal

🚀 **Novidades**
- Melhorias nas sugestões de compra com filtros por termo de busca
- Suporte para múltiplos IDs de produtos nas sugestões

## 04/03/2026

✨ **Melhorias**
- Otimização nas consultas de especificações de inventário
- Atualizações nos tipos de dados para campos de observações e tags
- Melhorias nos filtros de data para pedidos de venda

## 02/03/2026

🚀 **Novidades**
- Nova página inicial redesenhada com seções de boas-vindas, guia de configuração e notícias
- Implementado sistema de histórico de mudanças (changelog) na página "Sobre"
- Adicionada área do gestor com funcionalidades específicas de administração
- Nova funcionalidade de gerenciamento de assinaturas e planos
- Sistema de filtros avançados para diversos módulos (NFe, inventário, financeiro)

✨ **Melhorias**
- Aprimoramento na geração de sugestões de compra com análise detalhada do inventário
- Interface melhorada para gerenciamento de itens NFCe
- Novos relatórios detalhados de fornecimento
- Melhorias na autenticação e interface do usuário

🐛 **Correções**
- Correções na exibição de status em modais de detalhes
- Ajustes nos filtros de pagamentos sem data de registro
- Correções nos caminhos de importação e renderização condicional de componentes

## 25/02/2026

🚀 **Novidades**
- Lançamento da área do gestor com ferramentas exclusivas de gestão
- Melhorias na recuperação de produtos com filtros por quantidade disponível e ponto de venda

## 23/02/2026

🐛 **Correções**
- Correções na navegação por abas de status
- Ajustes nos caminhos de importação de componentes
- Correções pontuais de funcionamento em diversas telas
