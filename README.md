# 🙋‍ Relatório Técnico sobre Acesso SSH no EC2 - Luis Miranda

## :mag: Introdução:

Instalação e configuração de uma instância EC2, conectada via SSH utilizando o PuTTy.

## :dart: O objetivo:

O objetivo deste guia é apresentar, de maneira simplificada, como criar uma instância EC2 na AWS e acessá-la de qualquer lugar onde você esteja usando SSH via PuTTY.


## :jigsaw: Materiais necessários para o Relatório:

* Conta na AWS;
* Conta no GitHub para criar o arquivo Markdown;
* Ferramenta PuTTY.

# Método

## 1. Configurando a Instância EC2 na AWS

Se você já tiver uma conta logada na AWS, sua página WEB irá abrir diretamente na máquina que você tem disponível. Clique em "Executar" para iniciar a configuração da sua EC2. 

<img width="960" alt="tela-inicio" src="https://github.com/ragazziluis/ssh_no_EC2-S3M5/assets/110607385/a09de97c-7fca-4cd6-a698-3880bc616ad5">

Em seguida, iremos dar um nome para a instância. Neste exemplo, daremos o nome de "ponderada-S3", sinalizando que é a ponderada realizada na semana 3 do módulo

<img width="960" alt="criar_instancia" src="https://github.com/ragazziluis/ssh_no_EC2-S3M5/assets/110607385/8e2bb9d8-ef75-446a-8039-4fa60c64abc7">

Agora, iremos configurar o tipo de imagem que será usado. Neste exemplo, iremos utilizar o "Amazon Linux"

<img width="960" alt="selecionar_img" src="https://github.com/ragazziluis/ssh_no_EC2-S3M5/assets/110607385/e320020d-7823-4a77-af16-f61103a1daf5">

Rolando para baixo, iremos agora configurar a senha de acesso e o tipo de AMI. Você pode usar o da sua preferência

<img width="960" alt="criar_senha" src="https://github.com/ragazziluis/ssh_no_EC2-S3M5/assets/110607385/51080861-0b98-49ef-80b6-efebfc9eff95">

Para criar um par de chaves, basta clicar em "Create new key pair" e configurar parao o tipo ".ppk" para conseguirmos acesso ao SSH via PuTTY

<img width="959" alt="criar_senha2" src="https://github.com/ragazziluis/ssh_no_EC2-S3M5/assets/110607385/ad9755aa-ce6b-4921-a413-b3a0161a5e9b">

Agora, finalizando esta parte da configuração na AWS, configure os grupos de segurança e depois clique em "Launch instance". Em seguida, iniciamos a configuração dentro do PuTTY. Para esta etapa, é necessário tem a ferramenta instalada em seu PC/MAC para conseguir prosseguir nos próximos passos. 

## 2. Configurando a Instância EC2 utilizando o PuTTY (SSH)

Inicie o PuTTY em seu PC/MAC e inisira o endereço IP disponivél no EC2 em "Host Name"

<img width="630" alt="conexão_putty" src="https://github.com/ragazziluis/ssh_no_EC2-S3M5/assets/110607385/e22d5e98-76c0-40b1-a6f5-f1de9b264801">

Lembre-se de inserir a chave criada ".ppk" clicando em "Auth" na lista disponibilizada a esquerda da tela do PuTTY e clique em "Open" na sequência

<img width="827" alt="conexão_putty2" src="https://github.com/ragazziluis/ssh_no_EC2-S3M5/assets/110607385/d753aef7-bb3a-4778-a667-84eecdfda681">

## Resultados

Após finalizar todos os procedimentos na seção PuTTY, insira as credênciais "ec2-user" no terminal e aperte enter. Pronto! Sua máquina está rodando

<img width="842" alt="resultado_final2" src="https://github.com/ragazziluis/ssh_no_EC2-S3M5/assets/110607385/c43640ad-bc73-405e-bb36-23cf291c8709">

Você também pode confirmar se a máquina está rodando tranquilamente, acessando diretamente pela AWS, como na imagem a seguir, a mensagem "sucess" estará visível:

<img width="960" alt="resultado_final" src="https://github.com/ragazziluis/ssh_no_EC2-S3M5/assets/110607385/6913e7c2-64c4-4bda-88a0-21334484cea7">

# Conclusão do Relatório

Neste guia em formato Markdown, apresentamos o passo a passo para a criação de uma instância EC2 na plataforma AWS e também apresentamos a configuração necessária para o uso do SSH, utilizando a ferramenta PuTTY como meio de acesso remoto. Esse procedimento oferece uma visão das etapas na criação de uma instância em ambiente cloud.
