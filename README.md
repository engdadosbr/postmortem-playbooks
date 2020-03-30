## Postmortem Ticket

Conforme descrito no capítulo 15 do livro [Site Reliability Engineering](https://landing.google.com/sre/sre-book/toc/index.html) (Engenharia de Confiabilidade), [Postmortem Culture: Learning from Failure](https://landing.google.com/sre/sre-book/chapters/postmortem-culture/), o uso de tickets postmortem permitem registrar falhas e anomalias ocorridas em produção, ou mesmo ambientes de teste, visando encurtar caminhos quando situações similares se mostrarem presentes, adotando a postura "blameless culture" (cultura da não culpabilização). John Allspaw escreveu em seu artigo [Blameless PostMortems and a Just Culture](https://codeascraft.com/2012/05/22/blameless-postmortems/), destacando os pontos :

> Possuindo um processo Post-Mortem "sem culpa" significa que engenheiros cujas ações tenha contribuído com um acidente pode fornecer uma explanação detalhada de :

> * Quais ações devem tomar em determinado tempo,
> * Quais efeitos eles observaram,
> * Expectativas que tiveram,
> * Suposições que fizeram,
> * e entendimento da linha temporal dos eventos como eles ocorreram.

> e poderem dar detalhamentos sem receios de punição ou culpa.


Um modelo de postmortem report que pode ser seguido ou mesmo inspirado, [Example Postmortem](https://landing.google.com/sre/sre-book/chapters/postmortem/)


Para se criar diretório, algumas regras de formatação para identificação :

00x[numero de identificação]_nomedaferramenta(Hadoop,Spark, Hive etc)_nomeambiente(local,nuvem[AWS,GCP])_

Exemplo :

001_Spark_Docker_AWS

O arquivo README.md poderá conter resumo do postmortem, ou a estrutura total.
