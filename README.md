#Guia de Instalação do Projeto
Siga os passos abaixo para configurar o ambiente de desenvolvimento e instalar todas as dependências do projeto.

#Pré-requisitos
Certifique-se de que você tem o Python 3.8 ou uma versão superior instalada em sua máquina.

1. Criar e Ativar o Ambiente Virtual
É uma boa prática criar um ambiente virtual para isolar as dependências do seu projeto.

python -m venv venv

Em seguida, ative o ambiente virtual. O comando varia de acordo com o seu sistema operacional:

No Windows:

venv\Scripts\activate

No macOS e Linux:

source venv/bin/activate

Você saberá que o ambiente está ativado quando vir (venv) no início da linha de comando do seu terminal.

2. Instalar as Dependências
Com o ambiente virtual ativado, instale todas as dependências do projeto listadas no arquivo requirements.txt:

pip install -r requirements.txt

3. Configurar Variáveis de Ambiente
Crie um arquivo chamado .env na raiz do seu projeto (no mesmo diretório do arquivo manage.py) e adicione a sua SECRET_KEY e outras variáveis de ambiente necessárias.

Exemplo do arquivo .env:

SECRET_KEY='sua_secret_key_aqui'
DEBUG=True

Importante: Não compartilhe seu arquivo .env publicamente. Adicione-o ao seu arquivo .gitignore para evitar que ele seja enviado para repositórios como o Git.
