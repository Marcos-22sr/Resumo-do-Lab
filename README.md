# Resumo-do-Lab
Este repositório contém o resumo do assunto de computação em nuvem utilizando o Microsoft azure.

A computação em nuvem é um fornecimento de serviços de computação pela internet, tendo mais flexibilidade e rápidez.
Isso ocorre porque quanto mais as empresas vão evoluindo, mais dados precisam ser armazenados, logo para criar Datacenters, precisa de local físico, tornando o processo mais trabalhoso do que em um ambiente virtual

Existem 3 tipos de computação em nuvem, são elas: privada, pública, híbrida.

A privada ela só pode ser operadas pelos seus usuários, logo não conseguem ser compartilhadas e as organizações criam um ambiente em nuvem em seu datacenter. 
A pública pertence aos serviços nuvem e fornece os seus recursos e serviços a vários usuários. O acesso geralmente é pela internet.
A híbrida acaba tornando-se a "melhor parte" dos dois tipos passados. É a combinação dos dois tipos para que sejam executas em um melhor local.

Comparação de modelos de nuvem :

Pública: 
- Não há despesas de capital (CAPEX).
- As organizações só pagam pelo que utilizam.

Privada:
- As organizações tem controle total de seus recursos e segurança, juntamente com a manutenção e atualizações de hardware e software.

Híbrida:
- As organizações controlam onde vão executar seus aplicativos
- Fornece maior flexibilidade

Diferença entre CapEx e OpEx

OpEx: (Despesas operacionais)
- Gasta com serviços e produtos conforme necessário e pagamento conforme o uso
- Seja cobrado imediatamente

CapEx: (Despesas capital)
- O gasto inicial de dinheiro em estrutura física
- As despesas vão reduzindo ao passar do tempo.

Modelos baseados em consumo.

Os provedores de serviços nuvem eles operam em um modelo baseado no consumo, o que significa que os usuários só pagam pelo que consome.

------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

Praticar o processo de criação e configuração de uma máquina virtual na plataforma Microsoft Azure.

🖥️ Como Criar uma Máquina Virtual no Microsoft Azure (Windows)

Acesse o Portal do Azure
Vá para portal.azure.com e faça login com sua conta Microsoft. Se ainda não tiver uma conta, você pode criar uma gratuitamente com créditos iniciais.

Crie um Grupo de Recursos (opcional, mas recomendado)
No menu lateral, clique em "Grupos de recursos" e depois em "+ Criar". Dê um nome ao grupo, como MeuGrupoVM, e escolha uma região próxima, como Brasil Sul.

Inicie a Criação da Máquina
No menu lateral, clique em "Máquinas virtuais" e depois em "+ Criar" > "Máquina virtual".

Configure os Detalhes Básicos
Assinatura: Selecione sua assinatura do Azure. Grupo de Recursos: Escolha o grupo criado anteriormente. Nome da VM: Por exemplo, MinhaVM. Região: Escolha a mesma do grupo de recursos. Imagem: Selecione Windows Server 2022 Datacenter: Azure Edition - x64 Gen 2. Tamanho: Escolha um tamanho adequado às suas necessidades.

Configure a Conta de Administrador
Nome de usuário: Por exemplo, azureuser. Senha: Crie uma senha segura com pelo menos 12 caracteres, incluindo letras maiúsculas, minúsculas, números e símbolos.

Configure as Regras de Porta de Entrada
Em "Regras de porta de entrada", selecione "Permitir portas selecionadas". Escolha RDP (3389) para acesso remoto e, opcionalmente, HTTP (80) se desejar hospedar um site.

Revise e Crie a VM
Clique em "Revisar + criar". Após a validação, clique em "Criar" para iniciar a implantação.

Acesse sua Máquina Virtual
Após a implantação, vá para a página da VM e clique em "Conectar" > "RDP". Baixe o arquivo .rdp e abra-o para iniciar a conexão. Insira o nome de usuário e a senha definidos anteriormente.

🌐 Instale um Servidor Web (Opcional)

Para testar a VM, você pode instalar o IIS (Internet Information Services):

Conecte-se à VM via RDP. Abra o PowerShell como administrador. Execute o comando:

no powershell digite:

Install-WindowsFeature -name Web-Server -IncludeManagementTools

Após a instalação, abra um navegador e digite o endereço IP público da VM para ver a página padrão do IIS.

🧹 Gerencie seus Recursos

Desligamento Automático: Configure para evitar cobranças inesperadas. No portal da VM, vá em "Operações" > "Desligamento automático" e defina um horário. Exclusão de Recursos: Quando não precisar mais da VM, exclua o grupo de recursos para remover todos os recursos associados.
