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

💰 Redução de Custos
Com a computação em nuvem, elimina-se a necessidade de investimentos pesados em hardware e infraestrutura física. O modelo de pagamento conforme o uso permite que as empresas paguem apenas pelos recursos que realmente utilizam, convertendo despesas de capital (CapEx) em despesas operacionais (OpEx) .

📈 Escalabilidade e Elasticidade
A nuvem permite ajustar rapidamente os recursos de TI de acordo com as necessidades do negócio. Seja para lidar com picos de demanda ou para reduzir custos em períodos de baixa atividade, a escalabilidade é uma das principais vantagens .

🌐 Acessibilidade e Mobilidade
Os serviços em nuvem podem ser acessados de qualquer lugar com conexão à internet, facilitando o trabalho remoto e a colaboração entre equipes distribuídas geograficamente .

🔐 Segurança Aprimorada
Provedores de nuvem investem significativamente em segurança, oferecendo recursos como criptografia de dados, autenticação multifator e monitoramento contínuo. Além disso, a centralização dos dados facilita a implementação de políticas de segurança .

⚙️ Atualizações e Manutenção Automatizadas
Os provedores de serviços em nuvem cuidam das atualizações de software e manutenção da infraestrutura, garantindo que os sistemas estejam sempre atualizados e funcionando com desempenho otimizado .

🔄 Continuidade dos Negócios e Recuperação de Desastres
A computação em nuvem oferece soluções robustas para backup e recuperação de dados, garantindo a continuidade das operações mesmo em casos de falhas ou desastres naturais .
Oracle

🌱 Sustentabilidade
Ao migrar para a nuvem, as empresas podem reduzir significativamente seu consumo de energia e a emissão de carbono, contribuindo para práticas mais sustentáveis .

-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

☁️ IaaS – Infraestrutura como Serviço
O que é: Fornece recursos de infraestrutura virtualizados, como servidores, armazenamento e redes, permitindo que empresas construam e gerenciem suas próprias plataformas e aplicações.

Responsabilidades do cliente: Gerenciar sistemas operacionais, middleware, dados e aplicações.
Exemplos: Microsoft Azure, Amazon Web Services (AWS), Google Cloud Platform.

Quando usar: Ideal para empresas que necessitam de controle total sobre sua infraestrutura e desejam flexibilidade para configurar ambientes personalizados.

🛠️ PaaS – Plataforma como Serviço
O que é: Oferece uma plataforma completa para desenvolvimento, teste e implantação de aplicações, sem a necessidade de gerenciar a infraestrutura subjacente.
DIO

Responsabilidades do cliente: Desenvolver e gerenciar suas aplicações e dados.
Exemplos: Google App Engine, Heroku, Microsoft Azure App Services.

Quando usar: Indicado para desenvolvedores que desejam focar na criação de aplicações sem se preocupar com a gestão de servidores e infraestrutura.

📦 SaaS – Software como Serviço
O que é: Disponibiliza aplicações prontas para uso, acessíveis via internet, eliminando a necessidade de instalação e manutenção por parte do usuário.
Cloud Treinamentos

------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

Como criar um grupo de recursos no azure

✅ Usando o Portal Azure (interface gráfica)
Acesse o Portal Azure.

No menu lateral esquerdo, clique em "Grupos de recursos".
Clique no botão "+ Criar" ou "Adicionar".

Preencha os campos:
Assinatura: Escolha a assinatura do Azure.
Grupo de recursos: Dê um nome ao grupo (ex: meu-grupo-dev).
Região: Escolha a região onde os recursos estarão localizados (ex: Brazil South).

Clique em "Revisar + criar" e depois em "Criar".

Responsabilidades do cliente: Gerenciar o uso da aplicação, como configurações e dados inseridos.
Exemplos: Microsoft 365, Google Workspace, Salesforce.

Quando usar: Perfeito para empresas que buscam soluções prontas, com rápida implementação e sem a necessidade de gerenciar infraestrutura ou desenvolvimento.

------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

🖥️ Como criar uma máquina virtual no Azure
Acesse o portal do Azure: Vá para https://portal.azure.com e faça login com sua conta.

Navegue até "Máquinas virtuais": No menu lateral esquerdo, clique em "Máquinas virtuais" ou use a barra de pesquisa para encontrar essa opção.

Inicie a criação da VM: Na página de Máquinas Virtuais, clique em "Criar" e selecione "Máquina virtual do Azure".


Configure os detalhes da instância

Nome da VM: Escolha um nome, por exemplo, MinhaVM.
Região: Selecione a região mais próxima de você, como "Brasil Sul".
Imagem: Escolha o sistema operacional desejado, como "Windows Server 2022 Datacenter: Azure Edition - x64 Gen 2".
Tamanho: Selecione o tamanho da VM conforme suas necessidades.


Configure a conta de administrador:

Nome de usuário: Por exemplo, azureuser.
Senha: Crie uma senha segura com pelo menos 12 caracteres.

Defina as regras de porta de entrada:
Em "Regras de porta de entrada", escolha "Permitir portas selecionadas".

Selecione RDP (3389) para acesso remoto e HTTP (80) se planeja hospedar um site.


Revise e crie a VM:

Clique em "Examinar + criar".
Após a validação, clique em "Criar" para iniciar a implantação da VM.
Acesse a VM:
Após a implantação, vá para a página da VM.

Clique em "Conectar" e selecione "RDP".
Baixe o arquivo RDP e abra-o para iniciar a conexão remota.
Insira o nome de usuário e a senha que você definiu anteriormente.

