# Dicas-Azure-Dio
Este repositório oferece um guia passo a passo para criar e configurar máquinas virtuais no Azure, ideal para iniciantes que querem aprender sobre computação em nuvem e infraestrutura no Azure.

# Como Criar uma Máquina Virtual no Azure: Guia Fácil

Neste guia, vamos aprender a criar uma **máquina virtual** (VM) no **Azure** e entender um pouco sobre redes, computação e os tipos de nuvem. 

---

## Índice

1. [O que é uma Máquina Virtual no Azure?](#o-que-é-uma-máquina-virtual-no-azure)
2. [Como Criar uma Máquina Virtual Passo a Passo](#como-criar-uma-máquina-virtual-passo-a-passo)
3. [Componentes Importantes no Azure](#componentes-importantes-no-azure)
4. [Dicas sobre Redes e Computação no Azure](#dicas-sobre-redes-e-computação-no-azure)
5. [Tipos de Nuvens: O que são e como Funcionam](#tipos-de-nuvens-o-que-são-e-como-funcionam)

---

## O que é uma Máquina Virtual no Azure?

Uma **máquina virtual (VM)** no Azure é como um computador que fica na nuvem, ou seja, em um servidor remoto. Você pode usar uma VM para rodar programas e armazenar arquivos, assim como um computador normal, mas ela fica hospedada no **Azure** e pode ser acessada pela internet.

---

## Como Criar uma Máquina Virtual Passo a Passo

### 1. Acesse o Portal do Azure
   - Primeiro, entre no [portal.azure.com](https://portal.azure.com).

### 2. Criando sua Máquina Virtual
   - No menu do lado esquerdo, clique em **"Máquinas Virtuais"** e depois em **"Criar"**.
   - Complete as informações:
     - **Assinatura**: Escolha sua assinatura do Azure (se você não tiver, o professor provavelmente já fez isso para você).
     - **Grupo de Recursos**: Crie ou escolha um grupo para organizar seus recursos.
     - **Nome da VM**: Dê um nome para sua máquina virtual.
     - **Região**: Escolha onde seu servidor estará (a região mais próxima de você).
     - **Imagem**: Escolha o sistema operacional que vai usar (Windows, Linux, etc.).
     - **Tamanho da VM**: Escolha um modelo de máquina de acordo com as necessidades do seu projeto (não precisa ser muito grande no começo).
     - **Usuário e Senha**: Coloque um nome de usuário e uma senha para acessar a VM.

### 3. Configuração de Rede
   - Escolha ou crie uma **rede virtual (VNet)** para conectar sua VM com outros recursos. 
   - Ative um **IP público** para poder acessar a máquina pela internet.

### 4. Armazenamento
   - Selecione se quer usar **discos SSD (rápidos)** ou **HDD (mais lentos e baratos)** para guardar seus arquivos.

### 5. Finalize a Criação
   - Após revisar, clique em **"Criar"**. A máquina será criada em alguns minutos e estará pronta para uso!

---

## Componentes Importantes no Azure

O Azure é composto por várias ferramentas e recursos que você pode usar para montar sua solução:

- **Máquinas Virtuais (VMs)**: São os "computadores" virtuais que você cria para rodar programas.
- **Redes Virtuais (VNets)**: São como redes privadas que conectam suas máquinas, bancos de dados e outros serviços dentro do Azure.
- **Armazenamento (Storage Accounts)**: É onde você guarda arquivos e dados na nuvem, como fotos, vídeos e documentos.
- **Load Balancer**: Ajuda a distribuir o tráfego para várias VMs, garantindo que tudo funcione sem sobrecarregar uma só máquina.
- **Azure Active Directory (Azure AD)**: Gerencia quem pode acessar o quê dentro da sua conta no Azure.
- **Azure Firewall**: Protege sua rede contra acessos não autorizados.

---

## Dicas sobre Redes e Computação no Azure

### Redes no Azure
- **VNet (Rede Virtual)**: Crie uma rede privada para que suas VMs e outros serviços possam conversar entre si sem estar na internet aberta.
- **Sub-redes**: Organize suas VMs em diferentes sub-redes para separar o tráfego (por exemplo, uma sub-rede para a parte pública e outra para a parte privada).
- **Peering de VNets**: Se você tem mais de uma VNet, pode conectá-las para permitir que elas se comuniquem entre si.

### Computação no Azure
- **Escalabilidade**: No Azure, você pode aumentar ou diminuir os recursos (como o número de VMs) conforme a necessidade do seu projeto, sem precisar se preocupar em comprar hardware novo.
- **Azure Scale Sets**: Se você precisar de várias máquinas para rodar seu projeto, pode configurar um **"set de escalabilidade"** para aumentar ou diminuir automaticamente o número de VMs.

---

## Tipos de Nuvens: O que são e como Funcionam

Existem três tipos principais de nuvem:

- **Nuvem Pública**: É quando você usa os serviços da nuvem de empresas como o Azure, AWS, Google Cloud. Eles cuidam de tudo para você.
  - **Vantagens**: Custo mais baixo, fácil de usar, pode crescer conforme sua necessidade.
  - **Desvantagens**: Menos controle sobre os recursos, mais dependência do fornecedor.
  
- **Nuvem Privada**: A nuvem é exclusiva para uma única organização. Ela pode ser montada dentro da própria empresa ou por um terceiro.
  - **Vantagens**: Mais controle e segurança.
  - **Desvantagens**: Mais caro, precisa de mais manutenção.

- **Nuvem Híbrida**: Combina nuvem pública e privada, oferecendo flexibilidade para escolher onde armazenar os dados.
  - **Vantagens**: Flexibilidade e mais opções de segurança.
  - **Desvantagens**: Mais difícil de gerenciar e configurar.

---

Esse guia te ajudou a entender como criar uma máquina virtual no Azure e como funciona a infraestrutura e as redes no ambiente de nuvem. Agora você pode usar o Azure para explorar mais e criar projetos interessantes na nuvem!
