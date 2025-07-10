# Desafio POO - iPhone

Este projeto simula um componente do iPhone com funcionalidades de:

- Reprodutor Musical
- Aparelho Telefônico
- Navegador na Internet

## Diagrama UML

```mermaid
classDiagram
    class IReprodutorMusical {
        +tocar()
        +pausar()
        +selecionarMusica(String musica)
    }

    class IAparelhoTelefonico {
        +ligar(String numero)
        +atender()
        +iniciarCorreioVoz()
    }

    class INavegadorInternet {
        +exibirPagina(String url)
        +adicionarNovaAba()
        +atualizarPagina()
    }

    class IPhone {
        +tocar()
        +pausar()
        +selecionarMusica(String musica)
        +ligar(String numero)
        +atender()
        +iniciarCorreioVoz()
        +exibirPagina(String url)
        +adicionarNovaAba()
        +atualizarPagina()
    }

    IReprodutorMusical <|.. IPhone
    IAparelhoTelefonico <|.. IPhone
    INavegadorInternet <|.. IPhone
