<<<<<<< HEAD
# ANÁLISE DE DESEMPENHO POR CURSO DE GRADUAÇÃO DAS UNIVERSIDADES PÚBLICAS SEGUNDO PERFIL SOCIOECONÔMICO DOS GRADUANDOS
=======
### ANÁLISE DO DESEMPENHO NO ENADE DE ESTUDANTES DO ENSINO SUPERIOR MATRICULADOS EM UNIVERSIDADES PÚBLICAS SEGUNDO PERFIL SOCIOECONÔMICO

>>>>>>> desenvolvimento
O artigo XXVI da DUDH declara sobre acesso ao ensino superior mediante meritocracia, contudo não abrange a sustentabilidade do aluno após o processo seletivo. Este trabalho tem como objetivo avaliar se existe uma alta discrepância no desempenho entre grupos socioeconômicos distintos entre os graduandos do ensino superior público.
Este trabalho têm finalidade básica estratégica, com objetivo descritivo, utiliza uma abordagem qualiquantitativa, através do método hipotético dedutivo e faz uso de procedimentos bibliográficos e documentais.
Para facilitar o trabalho em grupo de maneira remoto, o desenvolvimento do trabalho faz uso das ferramentas Git, um versionador de documentos, e Docker, que permite criar ambientes virtuais comumente chamados de containers. Pressupondo que você já tenha instalado git no seu computador, eis os passos para configurar o ambiente de trabalho usando o Docker via Linux:

1. Instale, caso ainda não tenha instalado, através deste manual segundo seu sistema operacional

2. Na pasta AnaliseEnsinoSuperiorPublico clonada através do github, rode o comando:
$ docker build -t analise_ensino_superior_publico .

3. Após criado o ambiente virtual com o comando acima, execute-o com o comando:
$ docker run -d --rm --name jupyterserver -p 8888:8888 -v "$PWD/notebooks:/home/notebooks" analise_ensino_superior_publico

4. Isto já vai permitir acessar o jupyter no navegador através do endereço “localhost:8888”

5. Para acessar/editar as pastas de trabalho através do jupyter copie o token após comando:
$ docker container logs jupyterserver

6. Com o token em mãos, é só voltar ao navegador e fazer uso do arquivo notebooks/analise.ipynb
