# Criar-uma-m-quina-virtual-do-Windows-no-portal-Azure
Este repositório tem como objetivo de consolidar conhecimentos em máquinas virtuais da Azure.
Criar uma Máquina Virtual do Windows no Portal do Azure

Passo 1: Entrar no Azure

- Entre no portal do Azure.

Passo 2: Criar Máquina Virtual

- Digite "máquinas virtuais" na pesquisa.
- Em Serviços, selecione Máquinas virtuais.
- Na página Máquinas virtuais, clique em Criar e selecione Máquina virtual do Azure.
- A página Criar uma máquina virtual é aberta.

Passo 3: Detalhes da Instância

- Em Detalhes da instância, insira "myVM" no Nome da máquina virtual e escolha "Windows Server 2022 Datacenter: Azure Edition - x64 Gen 2" na Imagem.
- Deixe os outros padrões.

Passo 4: Conta de Administrador

- Em Conta de administrador, forneça um nome de usuário, como "azureuser" e uma senha.
- A senha deve ter no mínimo 12 caracteres e atender a requisitos de complexidade definidos.

Passo 5: Regras de Porta de Entrada

- Em Regras de porta de entrada, escolha Permitir portas selecionadas e, em seguida, selecione RDP (3389) e HTTP (80) na lista suspensa.

Passo 6: Criar a Máquina Virtual

- Deixe os padrões restantes e, em seguida, selecione o botão Examinar + criar na parte inferior da página.
- Após a execução da validação, selecione o botão Criar na parte inferior da página.
- Clique no botão Criar para criar a VM.

Passo 7: Conectar-se à Máquina Virtual

- Inicie uma conexão da área de trabalho remota para a máquina virtual.
- Selecione Conectar>RDP na página de visão geral de sua máquina virtual.
- Na guia Conectar-se ao RDP, mantenha as opções padrão para se conectar por endereço IP pela porta 3389 e clique em Baixar arquivo RDP.
- Abra o arquivo RDP baixado e clique em Conectar quando solicitado.

Passo 8: Instalar Servidor Web

- Abra um prompt do PowerShell na VM e execute o seguinte comando: `Install-WindowsFeature -name Web-Server -IncludeManagementTools`

Passo 9: Exibir a Página de Boas-vindas do IIS

- No portal, selecione a VM e, na visão geral da VM, passe o mouse sobre o endereço IP para mostrar Copiar para área de transferência.
- Copie o endereço IP e cole-o em uma guia do navegador.
- A página de boas-vinda do IIS padrão será aberta.

Passo 10: Limpar os Recursos

- Excluir recursos: quando o grupo de recursos, a máquina virtual e todos os recursos relacionados não forem mais necessários, exclua-os.
- Desligamento automático: configure o desligamento automático para evitar custos desnecessários.

Próximas Etapas

- Aprenda mais sobre máquinas virtuais do Azure e explore os recursos adicionais, como documentação e treinamento.

  https://learn.microsoft.com/pt-br/azure/virtual-machines/windows/quick-create-portal
