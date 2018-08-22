---     
layout: workshop
carpentry: swc
venue: Universidade Federal do Ceará
address: LabVis
country: Brazil
language: pt
latlng: -3.74576,-38.57431
humandate: 10-11 de Setembro de 2018
humantime: 9:00 am - 5:00 pm
startdate: 2018-09-10
enddate: 2018-09-11
instructor: ["Raniere Silva"]
helper: ["Romuere Silva"]
contact: fsombraufc@gmail.com
etherpad:
eventbrite: 
---
<!--
  HEADER

  Edit the values in the block above to be appropriate for your
  workshop.  Run 'tools/check' *before* committing to make sure that
  changes are good.
-->

<!--
  EVENTBRITE

  This block includes the Eventbrite registration widget if
  'eventbrite' has been set in the header.  You can delete it if you
  are not using Eventbrite, or leave it in, since it will not be
  displayed if the 'eventbrite' field in the header is not set.
-->
{% if page.eventbrite %}
<iframe
  src="https://www.eventbrite.com/tickets-external?eid={{page.eventbrite}}&ref=etckt"
  frameborder="0"
  width="100%"
  height="274px"
  scrolling="auto">
</iframe>
{% endif %}

<h2>Informações gerais</h2>

<!--
  INTRODUCTION

  Edit the general explanatory paragraph below if you want to change
  the pitch.
-->
<p>
  A missão da <a href="//software-carpentry.org">Software Carpentry</a>
  é ajudar cientistas e engenheiros a serem mais produtivos com menos sofrimento
  ao ensinar práticas laboratoriais para computação científica.
  Esse workshop prático irá cobrir
  conceitos e ferramentas, incluindo design de programas, controle de versão,
  gerenciamento de dados e automação de tarefas.
  Participantes são encorajados a se ajudarem
  e aplicarem o que eles aprenderem em suas próprias pesquisas.
</p>
<p align="center">
  <em>
    Para mais informações sobre o que ensinamos e porque,
    leia nosso artigo
    "<a href="http://journals.plos.org/plosbiology/article?id=10.1371/journal.pbio.1001745">Best Practices for Scientific Computing</a>".
  </em>
</p>

<!--
  AUDIENCE

  Explain who your audience is.  (In particular, tell readers if the
  workshop is only open to people from a particular institution.
-->
<p>
  <strong>Quem:</strong>
  Este curso é destinado alunos de graduação, pós-graduação e outros pesquisadores.
</p>

<!--
  LOCATION

  This block displays the address and links to maps showing directions
  if the latitude and longitude of the workshop have been set.  You
  can use http://itouchmap.com/latlong.html to find the lat/long of an
  address.
-->
{% if page.latlng %}
<p>
  <strong>Onde:</strong>
  {{page.address}}.
  Obtenha direções em
  <a href="//www.openstreetmap.org/?mlat={{page.latlng | replace:',','&mlon='}}&zoom=16">OpenStreetMap</a>
  ou
  <a href="//maps.google.com/maps?q={{page.latlng}}">Google Maps</a>.
</p>
{% endif %}

<!--
  SPECIAL REQUIREMENTS

  Modify the block below if there are any special requirements.
-->
<p>
  <strong>Requerimentos:</strong>
</p>

<ol>
  <li>Aceitar o <a href="{{site.swc_site}}/conduct.html">Código de Conduta</a> da Software Carpentry.</li>
  <li>Realizar a pré-inscrição.</li>
  <li>Enviar currículo e carta de apresentação para <a href='mailto:flavio86@ufpi.edu.br?Subject=Software Carpentry na UFC - CV'>flavio86@ufpi.edu.br</a>.</li>
  <li>Realizar inscrição (seguindo informações enviadas por email).</li>
  <li>Trazer seu próprio notebook
    com os programas listados <a href="#setup">abaixo</a> já instalados.</li>
</ol>

<!--
  CONTACT EMAIL ADDRESS

  Display the contact email address set in the header.  If an address
  isn't set in the header, the Software Carpentry admin address is
  used.
-->
<p>
  <strong>Contato</strong>:
  Por favor, envie um email para <a href='mailto:flavio86@ufpi.edu.br?Subject=Software Carpentry na UFC'>Flavio</a> 
  ou <a href="mailto:romuere@ufpi.edu.br?Subject=Software Carpentry na UFC">Romuere</a>
  ou {% if page.contact %}
    <a href='mailto:{{page.contact}}'>{{page.contact}}</a>
  {% else %}
    <a href='mailto:{{site.contact}}'>{{site.contact}}</a>
  {% endif %}
  com suas dúvidas.
</p>

<hr/>

<!--
  SCHEDULE

  Show the workshop's schedule.  Edit the items and times in the table
  to match your plans.  You may also want to change 'Day 1' and 'Day
  2' to be actual dates or days of the week.
-->
<h2>Programação</h2>

<div class="row-fluid">
  <div class="col-md-6">
    <h3>Dia 1</h3>
    <table class="table table-striped">
      <tr> <td>09:00</td> <td>Automatização de tarefas com o terminal Unix</td> </tr>
      <tr> <td>12:00</td> <td>Intervalo para almoço</td> </tr>
      <tr> <td>13:00</td> <td>Construindo programas com R</td> </tr>
      <tr> <td>16:00</td> <td>Revisão</td> </tr>
    </table>
  </div>
  <div class="col-md-6">
    <h3>Dia 2</h3>
    <table class="table table-striped">
      <tr> <td>09:00</td> <td>Controle de Versão com Git</td> </tr>
      <tr> <td>12:00</td> <td>Intervalo para almoço</td> </tr>
      <tr> <td>13:00</td> <td>Mais exemplos de programas em R</td> </tr>
      <tr> <td>16:00</td> <td>Revisão</td> </tr>
    </table>
  </div>
</div>

<!--
  ETHERPAD

  Display the Etherpad for the workshop.  You can set this up in
  advance or on the first day; either way, make sure you push changes
  to GitHub after you have its URL.  To create an Etherpad, go to

      http://etherpad.mozilla.org/YYYY-MM-DD-site

  where 'YYYY-MM-DD-site' is the identifier for your workshop (e.g.,
  '2015-06-10-esu'.
-->
{% if page.etherpad %}
<p>
  <strong>Etherpad:</strong> <a href="{{page.etherpad}}">{{page.etherpad}}</a>.
  <br/>
  Iremos utilizar o Etherpad listado acima para chat,
  anotações e compartilhamento de links e pequenos pedaços de código.
</p>
{% endif %}

<hr/>

<!--
  SYLLABUS

  Show what topics will be covered.

  1. If your workshop is R rather than Python, remove the comment
     around that section and put a comment around the Python section.
  2. Some workshops will delete SQL.
  3. Please make sure the list of topics is synchronized with what you
     intend to teach.
  4. You may need to move the div's with class="col-md-6" around inside
     the div's with class="row" to balance the multi-column layout.

  This is one of the places where people frequently make mistakes, so
  please preview your site before committing, and make sure to run
  'tools/check' as well.
-->
<h2>Resumo</h2>

<div class="row">
  <div class="col-md-4">
    <h3>Unix Shell</h3>
    <ul>
      <li>Arquivos e diretórios</li>
      <li>Histórico e tab completion</li>
      <li>Pipes e redirecionamento</li>
      <li>Laços sobre arquivo</li>
      <li>Criando e executando shell scripts</li>
      <li>Encontrando "coisas"</li>
      <li><a href="{{site.swc_lessons}}/ref/01-shell.html">Referências...</a></li>
    </ul>
  </div>
  <!--
  <div class="col-md-6">
    <h3>Programação em Python</h3>
    <ul>
      <li>Usando bibliotecas/pacotes</li>
      <li>Trabalhando com vetores</li>
      <li>Lendo e visualizando dados</li>
      <li>Criando e usando funções</li>
      <li>Laços e condicionais</li>
      <li>Programação defensiva</li>
      <li>Usando Python pela linha de comando</li>
      <li><a href="{{site.swc_lessons}}/ref/03-python.html">Referências...</a></li>
    </ul>
  </div>
  -->
  <div class="col-md-4">
    <h3>Programming in R</h3>
    <ul>
      <li>Trabalhando com vetores e data frames</li>
      <li>Lendo e visualizando dados</li>
      <li>Criando e usando funções</li>
      <li>Laços e condicionais</li>
      <li>Usando R pela linha de comando</li>
      <li><a href="{{site.swc_lessons}}/ref/06-R.html">Referências...</a></li>
    </ul>
  </div>
  <div class="col-md-4">
    <h3>Controle de versão com Git</h3>
    <ul>
      <li>Criação de repositórios</li>
      <li>Salvando mudanças de arquivos: <code>add</code>, <code>commit</code>, ...</li>
      <li>Visualizando mudanças: <code>status</code>, <code>diff</code>, ...</li>
      <li>Ignorando arquivos</li>
      <li>Trabalhando na internet: <code>clone</code>, <code>pull</code>, <code>push</code>, ...</li>
      <li>Resolvendo conflitos</li>
      <li>Licenças Abertas</li>
      <li>Onde hospedar seu trabalho e porque</li>
      <li><a href="{{site.swc_lessons}}/ref/02-git.html">Referências...</a></li>
    </ul>
  </div>
  <!--
  <div class="col-md-6">
    <h3>Gerenciando dados com SQL</h3>
    <ul>
      <li>Lendo e ordenando dados</li>
      <li>Filtrando com <code>where</code></li>
      <li>Calculando novos valores "on the fly"</li>
      <li>Lidando com valores perdidos</li>
      <li>Combinando valores</li>
      <li>Combinando tabelas</li>
      <li>Criando, modificando e deletando dados</li>
      <li>Programação com banco de dados</li>
      <li><a href="{{site.swc_lessons}}/ref/04-sql.html">Referências...</a></li>
    </ul>
  </div>
  -->
</div>

<hr/>

<!--
  SETUP

  Delete irrelevant sections from the setup instructions.  Each
  section is inside a 'div' without any classes to make the beginning
  and end easier to find.

  This is the other place where people frequently make mistakes, so
  please preview your site before committing, and make sure to run
  'tools/check' as well.
-->

<h2 id="setup">Setup</h2>

<p>
  Para participar de um workshop da Software Carpentry,
  você vai precisar dos seguintes programas instalados.
  Além dos softwares listados,
  você precisa de um navegador web atual.
</p>

<div id="editor"> <!-- Start of 'editor' section. -->
  <h3>Editor</h3>
  <p>
    Quando você está escrevendo um código, é interessante ter um editor de
    texto otimizado para a escrita de código, com funcionalidades como
    utilização de cores para palavras chaves. O editor padrão no Mac OS X e
    Linux é o Vim, que não é famoso por ser intuitivo.
    Se você acidentalmente encontrar-se preso nele,
    tente pressionar <code>ESC</code>, digitar <code>:q!</code> e pressionar <code>ENTER</code>
    para retornar à linha de comando.
  </p>

  <div class="row">
    <div class="col-md-4">
      <h4 id="editor-windows">Windows</h4>
      <p>
        <code>nano</code> é o editor instalado pelo instalador da Software
        Carpentry. Ele é um editor básico utilizado nas lições.
      </p>
      <p>
        <a href="http://notepad-plus-plus.org/">Notepad++</a> é outro popular
        editor livre para Windows. Depois de instalá-lo você precisa adicionar o
        diretório onde ele foi instalado no <em>path</em> do seu sistema para que
        possa invocá-lo pela linha de comando (ou para que outros programas como
        Git invoque-o por você). Por favor requisite ajuda dos instrutores para
        fazer isso.
      </p>
    </div>
    <div class="col-md-4">
      <h4 id="editor-macosx">Mac OS X</h4>
      <p>
        Nos recomendamos
        <a href="http://www.barebones.com/products/textwrangler/">Text Wrangler</a> ou
        <a href="http://www.sublimetext.com/">Sublime Text</a>.
        Você também pode utilizar o <code>nano</code> que deveria estar instalado
        por padrão.
      </p>
    </div>
    <div class="col-md-4">
      <h4 id="editor-linux">Linux</h4>
      <p>
        <a href="http://kate-editor.org/">Kate</a> é uma das várias opções para os
        usuários de Linux.
        Você também pode utilizar <code>nano</code> que deveria estar
        pré-instalado.
      </p>
    </div>
  </div>
</div> <!-- End of 'editor' section. -->

<div id="shell"> <!-- Start of 'shell' section. -->
  <h3>Bash Shell</h3>

  <p>
    Bash é o terminal comumente utilizado. Utilizar um terminal lhe permite
    fazer tarefas mais complexas de forma mais rápida no seu computador.
  </p>

  <div class="row">
    <div class="col-md-4">
      <h4 id="shell-windows">Windows</h4>
      <p>
        Baixe e instale
        <a href="http://msysgit.github.io/">Git for Windows</a>.
        Ele irá disponibilizar Git e Bash no seu computador.
      </p>
      <h4>Instalador da Software Carpentry</h4>
      <p>Ele instala e configura o <code>nano</code> (<a href="{{site.swc_github}}/windows-installer">e outras coisas</a>)</p>
      <p><em>Esse instalador precisa que uma conexão de internet.</em></p>
      <p>Depois de instalar Git Bash:</p>
      <ul>
        <li>
          Baixe <a href="{{site.swc_installer}}">Software Carpentry Windows Installer</a>.
        </li>
        <li>
          Click duas vezes no arquivo para executá-lo.
        </li>
      </ul>
    </div>
    <div class="col-md-4">
      <h4 id="shell-macosx">Mac OS X</h4>
      <p>
        O terminal padrão em todas as versões do Mac OS X é o bash e portanto você
        não precisa instalar nada. Você pode acessar o bash pelo Terminal
        encontrado em <code>/Applications/Utilities</code>. Você provavelmente vai
        querer manter o Terminal no dock da sua área de trabalho.
      </p>
    </div>
    <div class="col-md-4">
      <h4 id="shell-linux">Linux</h4>
      <p>
        O terminal padrão normalmente é <code>bash</code> e você não precisa
        instalar nada.  Se sua máquina estiver configurada de maneira diferente
        você pode abrir um terminal e digitar <code>bash</code>.
      </p>
    </div>
  </div>
<div> <!-- End of 'shell' section. -->

<div id='git'> <!-- Start of 'Git' section. GitHub browser compatability
           is given at https://help.github.com/articles/supported-browsers/-->
  <h3>Git</h3>

  <p>
    Git é um sistema de controle de versão
    que permite você manter registro de quem faz uma alteração
    em qual arquivo e quando
    além de possuir opções para facilmente atualizar seu código
    em <a href="https://github.com/">github.com</a>.
    Você vai precisar de um navegador web
    <a href="https://help.github.com/articles/supported-browsers/">suportado</a>
    (versões atuais do Chrome, Firefox ou Safari,
    ou Internet Explorer 9 ou superior).
  </p>

  <div class="row">
    <div class="col-md-4">
      <h4 id="git-windows">Windows</h4>
      <p>
        Git deve estar instalado no seu computador como parte da instalação do
        Bash (descrito acima).
      </p>
    </div>
    <div class="col-md-4">
      <h4 id="git-macosx">Mac OS X</h4>
      <p>
	<strong>Para OS X 10.8 e superior</strong>,
        instale Git para Mac
        baixando e executando
	<a href="http://sourceforge.net/projects/git-osx-installer/files/latest/download">esse instalador</a>.
        Depois de instalar Git, não existirá nenhum atalho no seu diretório <code>/Applications</code>
        pois Git é um programa de linha de comando.
      </p>
      <p>
	<strong>Para versões antigas do OS X (10.5-10.7)</strong>
        utilize o instalador mais recente para a sua máquina
	<a href="http://sourceforge.net/projects/git-osx-installer/files/">disponível em</a>.
        Utilize o instalador para Leopard para 10.5
        e o Snow Leopard para 10.6-10.7.
      </p>
    </div>
    <div class="col-md-4">
      <h4 id="git-linux">Linux</h4>
      <p>
        Se Git ainda não encontra-se disponível na sua máquina você pode
        instalá-lo via o gerenciador de pacotes da sua distribuição
        Para Debian/Ubuntu execute
        <code>sudo apt-get install git</code>
        e para Fedora execute <code>sudo yum install git</code>.
      </p>
    </div>
  </div>
</div> <!-- End of 'Git' section. -->

<div id="r"> <!-- Start of 'R' section. -->
  <h3>R</h3>

  <p>
    <a href="http://www.r-project.org">R</a> é uma linguagem de programação
    que é particularmente poderosa para exploração de dados, visualização, e
    análises estatísticas. Para interagir com R, nós utilizaremos o
    <a href="http://www.rstudio.com/">RStudio</a>.
  </p>

  <div class="row">
    <div class="col-md-4">
      <h4 id="r-windows">Windows</h4>
      <p>
	Instale R baixando e rodando
	<a href="http://cran.r-project.org/bin/windows/base/release.htm">este arquivo .exe</a>
	disponível no <a href="http://cran.r-project.org/index.html">CRAN</a>.
	Além disso, por favor instale o
	<a href="http://www.rstudio.com/ide/download/desktop">RStudio IDE</a>.
      </p>
    </div>
    <div class="col-md-4">
      <h4 id="r-macosx">Mac OS X</h4>
      <p>
	Instale o R baixando e rodando
	<a href="http://cran.r-project.org/bin/macosx/R-latest.pkg">este arquivo .pkg</a>
	disponível no <a href="http://cran.r-project.org/index.html">CRAN</a>.
	Além disso, por favor instale o
	<a href="http://www.rstudio.com/ide/download/desktop">RStudio IDE</a>.
      </p>
    </div>
    <div class="col-md-4">
      <h4 id="r-linux">Linux</h4>
      <p>
	Você pode baixar os arquivos binários para sua distribuição particular
	em <a href="http://cran.r-project.org/index.html">CRAN</a>. Ou
	você pode utilizar seu "package manager" (e.g. para Debian/Ubuntu
	rode <code>sudo apt-get install r-base</code> e para Fedora rode
        <code>sudo yum install R</code>). Além disso, por favor instale o
	<a href="http://www.rstudio.com/ide/download/desktop">RStudio IDE</a>.
      </p>
    </div>
  </div>
</div> <!-- End of 'R' section. -->

<!--
  Thanks section
-->
<h2 id="thanks">Agradecimentos</h2>

<div id="thaks-table">
  <div class="row">
    <div class="col-md-3">
      <h4>Indivíduos</h4>
      <ul>
        <li>Raniere Silva</li>
        <li>Fátima Medeiros</li>
        <li>Romuere Silva</li>
      </ul>
    </div>
    <div class="col-md-3">
      <h4>Apoio Financeiro</h4>
      <img src="img/logo_gpi_big.gif" alt="LABVIS - Laboratório de Visão, Imagens e Sinais"/>
    </div>
    <!--
    <div class="col-md-3">
      <h4>Developed With</h4>
    </div>
    <div class="col-md-3">
      <h4>Organized By</h4>
    </div>
    <div class="col-md-3">
      <h4>Financial Support </h4>
      <img src="http://www.monsanto.com/Style%20Library/Images/logo.png" alt="Monsanto" class="img-responsive">
    </div>
    -->
</div>
