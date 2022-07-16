## Interfaces
- [Vídeo](#)

## Sumário
- [Interface](#interface)
    - [O que é](#o-que-é)
    - [Estrutura](#estrutura)
- Exemplos
    - [Simples](./simples/README.md)
    - [Avançado](./avancado/README.md)
    - [Generics](./generics/README.md)
- [Referências](#referências)

## Interface
### O que é
_Interface_ é um tipo que providencia uma coleção de métodos, isso significa que o _Interface_ é uma forma de especificar o comportamento de um objeto.

Com a chegada dos Generics na _1.18_, os _Interfaces_ também podem providenciar uma estrutura padrão de um _Struct_ no qual **DEVE** ser seguido.

### Estrutura
```golang
type Nome interface {
    // lista dos métodos
    Foo(param T) T
    Bar(param1 T, param2 K) (T, error)
}
```
Vamos destrinchar essa estrutura:
- `type`
    - A palavra chave para especificar que estamos definindo um tipo
- `Nome`
    - É o identificador do tipo que estamos definindo
- `interface`
    - Especifica qual é o tipo de nosso _sub-tipo_ `Nome`
- `Foo(param T) T` e `Bar(param1 T, param2 K) (T, error)`
    - São os métodos que definem esse _Interface_, logo, para um _Struct_ ser _interface Nome_, ele deve conter os métodos `Foo` e `Bar`.

## Referências:
- [Effective Go](https://go.dev/doc/effective_go#interfaces_and_types)
- [Ref Spec](https://go.dev/ref/spec#Interface_types)
- [Go By Example](https://gobyexample.com/interfaces)