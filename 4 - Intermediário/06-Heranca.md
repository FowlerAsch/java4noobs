# Herança

Quando você cria uma classe, você pode fazer com que ela herde os atributos e métodos de outra classe. Esse processo é chamado de herança. A classe que herda é chamada de subclasse e a classe de onde ela herda é chamada de superclasse. Para herdar de uma classe, use a palavra-chave `extends` depois do nome da subclasse e o nome da superclasse.

No exemplo abaixo temos uma classe `Animal` que possue um método `comer()` e uma classe `Cachorro` que herda de `Animal` e possue um método `latir()`. Quando criamos um objeto do tipo `Cachorro` podemos acessar os métodos tanto de `Animal` e `Cachorro`, afinal o `Cachorro` herda de `Animal`.

```java
class Animal {
    public void comer() {
        System.out.println("Comendo...");
    }
}

class Cachorro extends Animal {
    public void latir() {
        System.out.println("Au au!");
    }
}

public class Main {
    public static void main(String[] args) {
        Cachorro cachorro = new Cachorro();
        cachorro.comer();
        cachorro.latir();
    }
}
```

A utilização da herança é importante para reutilizar código e evitar repetição. Por exemplo, se todos os animais comem, não faria sentido implementar o método `comer()` em cada classe de animal. Além disso, isso facilita a manutenção e expansão do código. Se no futuro precisarmos adicionar um novo método à classe `Animal`, por exemplo, o método `dormir()`, podemos adicioná-lo à classe Animal e todos os animais herdarão esse método.

O princípio da herança permite que uma classe (conhecida como superclasse ou classe pai) compartilhe atributos e métodos com outra classe (conhecida como subclasse ou classe filha). Essa relação hierárquica entre classes promove a reutilização de código e facilita a organização e manutenção do sistema. Um dos principais benefícios da herança é a reutilização de código. Em vez de reescrever o mesmo código em várias classes, você pode definir atributos e métodos comuns em uma superclasse e permitir que as subclasses herdem essas características. Outro aspecto importante da herança é a sobrescrita de métodos (ou overriding), onde uma subclasse pode fornecer uma implementação específica de um método que já existe na superclasse. Isso permite que diferentes subclasses se comportem de maneira distinta, mesmo que compartilhem uma interface comum. Por exemplo, uma superclasse Animal pode ter um método fazerSom(), enquanto as subclasses Cachorro e Gato podem sobrescrever esse método para produzir sons específicos, como "Au Au!" e "Miau!", respectivamente.

## Sobrescrever métodos

Em alguns casos, você pode querer que a subclasse tenha um método com o mesmo nome da superclasse, porém com uma funcionalidade diferente. Para isso, você pode sobrescrever o método da superclasse. Para sobrescrever um método basta criar um método com o mesmo nome e parâmetros na subclasse. É também recomendado, mas não obrigatório, utilizar a anotação `@Override` para indicar que o método está sendo sobrescrito.

```java
class Animal {
    public void fazerBarulho() {
        System.out.println("O animal faz barulho...");
    }
}

class Cachorro extends Animal {
    @Override
    public void fazerBarulho() {
        System.out.println("Au au!");
    }
}
```

[Próximo](./07-Interfaces.md) - Interfaces
