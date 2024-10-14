# Construindo-Arquiteturas-no-Azure
Resposta ao desafio DIO - Construindo Arquiteturas no Azure
Para criar uma máquina virtual (VM) no Azure, siga este guia com as configurações principais para iniciar o processo:

### 1. **Acesse o Portal do Azure**
   - Entre no [Portal do Azure](https://portal.azure.com/) com sua conta.
   - No menu esquerdo, clique em **Máquinas Virtuais** e, em seguida, em **+ Criar** > **Máquina virtual do Azure**.

### 2. **Configurações Básicas**
   Na seção **Básico**, você configurará os detalhes principais:

   - **Assinatura**: Selecione a assinatura do Azure que deseja usar para a VM.
   - **Grupo de Recursos**: Escolha um grupo existente ou crie um novo para organizar a VM e seus recursos.
   - **Nome da VM**: Dê um nome à máquina virtual (exemplo: `VM-de-Estudo`).
   - **Região**: Escolha a região onde deseja hospedar a VM, como `East US` ou `Brazil South`.
   - **Disponibilidade**: Configure a **Opção de Redundância de Zona** se precisar de alta disponibilidade.
   - **Imagem**: Escolha o sistema operacional da VM (exemplo: Windows Server, Ubuntu, CentOS).
   - **Tamanho da VM**: Selecione o tamanho da máquina virtual com base na necessidade de CPU e memória. Para projetos pequenos, o tamanho `Standard_B1s` é uma escolha econômica.

### 3. **Configurações de Autenticação**
   - **Tipo de Autenticação**: Escolha entre **Senha** ou **Chave SSH** (recomendado para Linux).
   - **Nome de Usuário e Senha**: Defina as credenciais de administrador (anote essas informações para fazer login mais tarde).
   
### 4. **Discos**
   Na seção **Discos**, configure o armazenamento:
   - **Disco do Sistema Operacional**: Escolha o tipo (Standard SSD, Premium SSD, HDD) com base em performance e custo.
   - **Discos de Dados**: Adicione discos extras, se necessário, para armazenar dados.

### 5. **Rede**
   - **Rede Virtual (VNet)**: Escolha uma rede virtual existente ou crie uma nova para permitir a comunicação.
   - **Sub-rede**: Configure uma sub-rede ou selecione uma existente dentro da VNet.
   - **IP Público**: Se precisar de um IP público, habilite-o para acesso remoto.
   - **Grupo de Segurança de Rede (NSG)**: Configure as regras de segurança (como acesso RDP para Windows ou SSH para Linux) para garantir que apenas portas necessárias estejam abertas.

### 6. **Gerenciamento e Outras Configurações**
   - **Monitoramento**: Habilite o **Insight de Monitoramento** para acompanhar o desempenho da VM.
   - **Backup e Recuperação**: Configure backups automáticos, se necessário.
   - **Tags**: Adicione tags para facilitar a organização e o gerenciamento.

### 7. **Revisão e Criação**
   - Revise todas as configurações e clique em **Criar**. O Azure implantará a VM com base nas configurações escolhidas.

### 8. **Acessando a Máquina Virtual**
   - Após a criação, vá até **Máquinas Virtuais** e selecione a VM recém-criada.
   - Para Windows, acesse via **RDP**; para Linux, acesse via **SSH**.

### Dicas:
   - Escolha a região de acordo com a proximidade geográfica para reduzir latência.
   - Teste o desempenho com uma configuração menor e faça ajustes conforme necessário para otimizar custo e performance.
