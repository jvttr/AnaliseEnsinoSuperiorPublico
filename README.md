## Perfil socioeconômico dos alunos matriculados em universidades públicas

Marcando o término da segunda guerra mundial, a Organização das Nações Unidas
(ONU) foi fundado em 1945 com o compromisso de prevenir conflitos entre paı́ses e
garantir que as pessoas possam desfrutar de paz e de prosperidade. Para tal feito, em
10 de dezembro de 1948, a Assembleia Geral das Nações Unidas proclamou a [Declaração
Universal dos Direitos Humanos (DUDH)](https://www.unicef.org/brazil/declaracao-universal-dos-direitos-humanos) composta por 30 normas comuns para os povos
de todas as nações. O primeiro inciso artigo XXVI deste documento defende o direito a instrução gratuita
e obrigatória para os graus fundamentais:

>Todo ser humano tem direito à instrução. A instrução será gratuita, pelo menos nos graus elementares e fundamentais. A instrução elementar será obrigatória. A instrução técnico-profissional será acessível a todos, bem como a instrução superior, esta baseada no mérito.

Contudo, permite que o acesso ao ensino superior seja dado perante mérito. Este trabalho pretende identificar o perfil socioeconômico dos
alunos que ingressam e concluem um curso de graduação oferecido por uma instituição de educação superior (IES) da rede pública. Este trabalho têm finalidade básica estratégica, com objetivo descritivo, utiliza uma abordagem qualiquantitativa, através do método hipotético dedutivo e faz uso de procedimentos bibliográficos e documentais.
Para facilitar o trabalho em grupo de maneira remota, o desenvolvimento do trabalho faz uso das ferramentas Git, um versionador de documentos, e Docker, que permite criar ambientes virtuais usualmente chamados de containers. Segue os passos para configurar o ambiente de trabalho necessário para executar e visualizar os resultados desta análise, através do terminal de um sistema operacional linux:

1. Instale o git (Caso não tenha instalado ainda):
~~~
sudo apt-get install git-all
~~~
2. Baixe o projeto:
~~~
git clone https://github.com/jvttr/AnaliseEnsinoSuperiorPublico.git
~~~
3. Instale também o Docker (Caso não tenha instaldo ainda):
~~~
sudo dpkg --configure -a
sudo apt install docker.io
~~~
4. Na pasta AnaliseEnsinoSuperiorPublico clonada através do github, rode o comando:
~~~
docker build -t analise_ensino_superior_publico .
~~~
5. Após criado o ambiente virtual com o comando acima, execute-o com o comando:
~~~
docker run -d --rm --name jupyterserver -p 8888:8888 -v "$PWD/notebooks:/home/notebooks" analise_ensino_superior_publico
~~~
6. Copie o token do jupyter que aparece após comando:
~~~
docker container logs jupyterserver
~~~
7. Acesso o jupyter e cole o token no endereço abaixo através de um navegador web:
~~~
localhost:8888
~~~
8. Acesse a análise em notebooks/analise.ipynb
