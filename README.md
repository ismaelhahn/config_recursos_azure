### 1- Acesse o Portal do Azure 

1- Entre no [Portal do Azure](https://portal.azure.com).

2- No painel, procure por “Máquinas Virtuais” e clique em **"Criar"**. 


### 2- Configure a Máquina Virtual 

1- **Nome da VM**: Escolha um nome fácil de lembrar.

2- **Região**: Selecione a região mais próxima dos seus usuários para melhor performance.

3- **Imagem**: Escolha o sistema operacional (Windows ou Linux) que você quer usar.

4- **Tamanho**: Selecione o tamanho da VM com base nas suas necessidades de CPU e memória.

### 3- Configure o Dimensionamento da VM 

1- **Dimensionamento Manual**: Escolha um tamanho de VM baseado na carga de trabalho que você espera. O Azure oferece uma variedade de tamanhos de VM, desde opções básicas para tarefas leves até opções robustas para aplicações exigentes. 

2- **Dimensionamento Automático**: Configure a autoescala para ajustar automaticamente os recursos da VM com base na demanda. Isso é útil se você tem variações significativas no uso ou precisa garantir que a VM possa lidar com picos de carga. 
  
3- **Utilize o Azure Advisor**: O Azure Advisor fornece recomendações de dimensionamento com base no desempenho atual da sua VM. Ele pode sugerir ajustes para economizar custos ou melhorar o desempenho. 

### 4- Configure a Rede 

1- **Rede Virtual**: Crie uma nova rede ou escolha uma existente.
2- **Sub-rede**: Escolha a sub-rede para conectar sua VM.
3- **Grupo de Segurança de Rede (NSG)**: Defina regras para controlar o tráfego de entrada e saída da VM. Só permita o tráfego que você realmente precisa.

### 5- Defina Credenciais 

1- **Nome de Usuário e Senha**: Configure um usuário e senha fortes para acessar sua VM.
2- **Chaves SSH (para Linux)**: Se for Linux, use chaves SSH para se conectar com mais segurança.
    
 
### 6- Configurações Adicionais 

1- **Monitoramento**: Habilite o monitoramento para ficar de olho no desempenho da VM.
2- **Tags**: Adicione tags para organizar melhor seus recursos.
   
 
### 7- Revise e Crie 

1- Confira todas as configurações.
2- Clique em **"Criar"** e aguarde enquanto o Azure prepara sua VM.
   
 
### 8- Conecte-se à Sua VM 

1- **Para Windows**: Use Remote Desktop (RDP) para se conectar.
2- **Para Linux**: Use SSH para acessar a VM.

# Cuidados Importantes para Produção

## 1- **Segurança**

- **Configuração do NSG**: Defina regras de firewall para proteger sua VM. Bloqueie tudo que não é necessário.
- **Atualizações**: Mantenha o sistema e aplicativos atualizados.
- **Gerenciamento de Credenciais**: Use senhas fortes e considere ferramentas como Azure Key Vault para gerenciar segredos.

## 2- **Desempenho**

- **Tamanho Adequado**: Escolha o tamanho certo da VM para evitar problemas de desempenho.
- **Autoescala**: Configure o dimensionamento automático se sua carga de trabalho variar muito.

## 3- **Backup**

- **Backups Regulares**: Garanta que backups sejam feitos frequentemente.
- **Plano de Recuperação**: Tenha um plano de recuperação em caso de falhas.

## 4- **Monitoramento**

- **Acompanhe o Desempenho**: Use ferramentas de monitoramento para verificar como a VM está funcionando.
- **Relatórios**: Gere relatórios para ficar de olho no uso e na segurança.

## 5- **Custo**

- **Controle de Custos**: Acompanhe o uso e ajuste suas configurações para não gastar mais do que o necessário.
