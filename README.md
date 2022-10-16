### ANÁLISE DO PERFIL SOCIOECONÔMICO DE ALUNOS DO ENSINO SUPERIOR MATRICULADOS EM UNIVERSIDADES PÚBLICAS

O artigo XXVI da Declaração Universal dos Direitos Humanos defende o acesso gratuito ao ensino, contudo permite que o acesso ao ensino superior seja perante mérito. O objetivo deste trabalho é identificar se existe maior ocorrência de um perfil socioeconômico dentre os alunos que entram e dentre os que finalizam um curso de graduação do ensino superior público.
Este trabalho têm finalidade básica estratégica, com objetivo descritivo, utiliza uma abordagem qualiquantitativa, através do método hipotético dedutivo e faz uso de procedimentos bibliográficos e documentais.
Para facilitar o trabalho em grupo de maneira remota, o desenvolvimento do trabalho faz uso das ferramentas Git, um versionador de documentos, e Docker, que permite criar ambientes virtuais usualmente chamados de containers. Segue os passos para configurar o ambiente de trabalho necessário para executar e visualizar os resultados desta análise:

1. Instale o git, caso ainda não tenha instalado, através do comando:
$ sudo apt-get install git-all

2. Instale também o Docker, caso ainda não tenha instalado, através dos comandos:
$ sudo dpkg --configure -a
$ sudo apt install docker.io

3. Na pasta AnaliseEnsinoSuperiorPublico clonada através do github, rode o comando:
$ docker build -t analise_ensino_superior_publico .

4. Após criado o ambiente virtual com o comando acima, execute-o com o comando:
$ docker run -d --rm --name jupyterserver -p 8888:8888 -v "$PWD/notebooks:/home/notebooks" analise_ensino_superior_publico

5. Isto já vai permitir acessar o jupyter no navegador através do endereço “localhost:8888”

6. Para acessar/editar as pastas de trabalho através do jupyter copie o token após comando:
$ docker container logs jupyterserver

7. Com o token em mãos, é só voltar ao navegador e fazer uso do arquivo notebooks/analise.ipynb
