<h1>Início de Programação Orientada a Objetos</h1>

Muitos recomendam iniciar programação orientada a objetos em Java, por ser considerada uma mãe da orientação a objetos. Esse é um novo conceito, iremos aprender sobre classes, criações de atributos e de construtores. Esse vai ser um tutorial meio grande, mas não se espante, a medida do uso você vai compreendendo, assim como tudo na programação.

Para ter uma programação orientada ao objeto é necessário de uma classe para engolobar atributos, construtores e metodos.

<h2>Atributos</h2>

Os atributos são basicamente as variáveis que a classe vai ter, por exemplo, uma classe pessoa tem: nome, idade, cpf, endereço.

Dá pensar nos atributos como informações que só a classe (e os objetos criados a partir dela) possui, então a classe também tem que definir se essas informações serão acessiveis pra todos ou somente para ela. Pra isso, na declaração da variavel de atributo, dá pra definir se a variavel vai ser pública (public) ou privada (private).

<h2>Construtores</h2>

Os construtores são para quando você instanciar um objeto da classe, como por exemplo, o objeto pessoa, ele já pode definir automaticamente alguns valores que você quiser dos atributos.

Só com o construtor padrão da classe, vai ser necessário informar os valores dos atributos depois da instanciação. Com um construtor mais definido, dá pra informar os atributos na hora que se cria um objeto da classe (e economiza tempo)

<h2>Métodos</h2>
Os métodos são as funções que a classe vai ter, como por exemplo a classe pessoa pode ter uma função de aumentar a sua idade a cada ano que passa, ou um metodo que altera seu endereço.

Essas funções, assim como os atributos, podem ser públicos para serem acessados por qualquer comando fora da instância da classe ou privados para classe. As métodos de uma classe não são diferentes dos definidos na [parte 12 do Módulo Basico](https://github.com/paulorievrs/java4noobs/blob/master/3%20-%20B%C3%A1sico/12-Funcoes-Metodos.md)

<h2>Encapsulamento</h2>
Todos os atributos de uma classe devem ser usados somente dentro dela, portanto, cria-se um encapsulamento privado ao declará-los, e são criadas funções chamadas de get e set, para pegar e alterar esses atributos.

# Ideia sobre o que é Classe:
> Vamos entender o que seria classe, atributos e métodos:
No mundo real, temos a estrutura/objeto 'carro' em diferentes países. A classe é a definição do que seria o carro; ou seja, possui quatro rodas, volante, marcha, entre outros atributos, que são chamados de atributos de classe ou gerais. A partir disso, o carro se diferencia de país para país. Em certos lugares, existem carros com o volante à direita, o tipo de marcha, o veículo pode ser elétrico, automático ou manual, entre outras variações de comportamento. Apesar dessas diferenças, ainda é considerado um carro, e essas variações são representadas nos métodos.

# Atributo de Classe & Variável Local
> ## Qual a diferença entre Atributo de Classe e Variável local?
> Anotação : Atributo de Classe & Variável Local: Quando você cria um atributo geral daquela classe ele se torna uma variável única que pode ser utilizada em diferentes métodos. Quando você não utiliza e precisa criar uma mesma variável em cada método ela se torna três variáveis diferentes com o mesmo nome existindo ao mesmo tempo, se tornando uma variável local. <br><br>
> Atributo de Classe: Ele pode ser acessado e modificado por diferentes métodos da classe, o que o torna uma variável compartilhada dentro da instância do objeto. Isso significa que, enquanto o objeto existir, o atributo pode ser acessado em qualquer método da classe. O valor do atributo é persistente enquanto o objeto estiver em uso, e qualquer alteração feita nele em um método será visível para os outros métodos da mesma instância. <br><br>
> Variável local: Uma variável local é definida dentro de um método e só existe enquanto o método está em execução. Ela é criada quando o método é chamado e destruída quando o método termina sua execução. Cada vez que o método é chamado, a variável local é recriada, e seu valor não é compartilhado entre chamadas de métodos ou entre outros métodos da classe. Isso significa que ela tem um escopo limitado e não pode ser acessada fora do método em que foi criada. <br>

[Próximo](./04-PrimeiraClasse.md) - Primeira classe
