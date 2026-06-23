//    \_\_\_\_\_\_ \_\_\_\_\_  \_\_\_\_\_                                                 

//    | \_\_\_ \\  \_  ||  \_  |                                                

//    | |\_/ / | | || | | |   \_\_\_\_\_\_   \_ \_\_ \_\_\_  \_\_\_ \_   \_ \_ \_\_ \_\_\_   \_\_\_  

//    |  \_\_/| | | || | | |  |\_\_\_\_\_\_| | '\_\_/ \_ \\/ \_\_| | | | '\_ ` \_ \\ / \_ \\ 

//    | |\_  \\ \\\_/ /\\ \\\_/ /           | | |  \_\_/\\\_\_ \\ |\_| | | | | | | (\_) |

//    \\\_(\_)  \\\_\_\_(\_)\\\_\_\_(\_)          |\_|  \\\_\_\_||\_\_\_/\\\_\_,\_|\_| |\_| |\_|\\\_\_\_/ 

//                                                                        

//    Esse resumo fritas acompanha?

//

\----------------------------------------------------------------------------  

*Dependendo do local onde o resumo for aberto, o titulo em arte ascii será transformado em um amontoado de símbolos esquisitos, abra no bloco de notas com 110 de zoom*

*para melhor experiência!*

\----------------------------------------------------------------------------



O que é Programação orientada a objetos?

A programação orientada a objetos é um "estilo" (paradigma) de programação onde o código é organizado em classes e 

dividido em pequenas partes. Essas pequenas partes são os objetos. POO é muito útil para manutenção e melhor compreensão de 

códigos grandes, imagina ter que mudar um código de milhares e milhares de linhas, dessa maneira chega POO e salva a vida de milhões de 

programadores da tristeza e da miséria 😎.



* Classes: são moldes que representam o modelo de maneira abstrata. Elas definirão os atributos e os métodos ("comportamento")

dos objetos.



ex.: public class Usuário{}, public class Jogo{}, public class ContaSteam{}...



Cada uma das classes citadas compõem um único código, só que fragmentado em classes e objetos.



* Objetos e atributos: O objeto é a "concretização" da classe, ele armazenará os dados no tempo em que for ser executado o código. O objeto 

geralmente é criado na Main, com as informações desejadas. Os atributos irão armazenar dentro da classe essas informações.



ex. de criação de objeto: Usuario u1 = new Usuario("Cleidson", 12, "Cleidson.JohnnyJabelsJarbas@leinad.com");

ex. de atributo: private String nome, private int idade, private String email;



* Métodos: são as ações realizadas com o objeto declaradas nas classes. Elas podem alterar atributos, utilizar dados de entrada e resultar em uma saída de dados.



ex.: public Jogo(String tituloJogo, int classificacao, double preco) {

&#x20;       this.tituloJogo = tituloJogo;

&#x20;       if (classificacao < 0) {

&#x20;           this.classificacao = 0;

&#x20;       } else {

&#x20;           this.classificacao = classificacao;

&#x20;       }

&#x20;       if (preco < 0) {

&#x20;           this.preco = 0;

&#x20;       } else {

&#x20;           this.preco = preco;

&#x20;       }

&#x20;   }



* Encapsulamento: o encapsulamento é muito importante em POO, protegendo dados importantes! Vamos supor que os dados sensíveis do usuário sejam armazenados em um objeto.

Ninguém pode ter acesso a esses dados, imagina alguém pega o CPF e o RG de alguém e faz uma conta bancária falsa para lavar dinheiro 😢????? Para isso, utilizamos o private, 

tornando o dado acessível apenas dentro de sua própria Classe! Quando o dado é irrestrito, utilizamos o public.



Ex.: **private** String nome, **private** int idade



* Getters e Setters: métodos publicos que permitem que atributos private sejam vistos e alterados com maior segurança.



ex.: public String getTituloJogo() {

&#x20;       return tituloJogo;

&#x20;   }



&#x20;   public void setTituloJogo(String tituloJogo) {

&#x20;       this.tituloJogo = tituloJogo;

&#x20;   }



* Construtores: os construtores são métodos especiais que vão inicializar projeto, recebendo dados para inicializar os atributos. Como resultado o baby objeto nasce.



Ex.: public CompraSteam(Usuario usuario, Jogo jogo, Jogo ValorFinal) {

&#x20;       this.usuario = usuario;

&#x20;       this.jogo = jogo;

&#x20;       this.valorFinal = valorFinal;

&#x20;       this.statusCompra = "pendente";

&#x20;   }



* Override toString(): quando queremos imprimir um objeto diretamente no java, o programa não vai saber qual informações queremos, e entregará um output bizarro. Esse output

bizarro é o local da memória onde o objeto se encontra. Para resolver isso like a pro 😎😎😎😎😎, usamos o override toString()

O override toString() vai trocar o output do método de um endereço de memoria para um texto ali definido (você pode por qualquer coisa, mas EU acho que a principal utilidade é

ver tudo do objeto...eu acho)

Ex.:



* Sobrecarga: quando criamos dois métodos (como os construtores) que recebem dados diferentes mas possuem o mesmo nome, o programa vai analisar qual metodo melhor se encaixa nos

dados enviados e realiza a sobrecarga. 



Ex.: public Jogo(String tituloJogo, int classificacao, double promocao, double preco){...}

public Jogo(String tituloJogo, int classificacao){...}



* Composição: a composição ocorre quando uma classe possuí atributos que foram "criados" em outras classes.



Ex.: public class CompraSteam {

&#x20;   Usuario usuario;

&#x20;   Jogo jogo;

&#x20;   double valorFinal;

&#x20;   String statusCompra;

&#x20;   static double taxaLoja = 2.50;

...}

Nesse caso, a classe comprasteam utiliza objetos do tipo usuario e jogo.





