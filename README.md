# DESAFIO DIO - Modelando o iPhone com UML: Funções de Músicas, Chamadas e Internet

Projeto do curso da [**DIO**](https://web.dio.me/track/coding-future-gft-desenvolvimento-java-com-ia) (Desenvolvimento Java com IA) que modela em UML as principais funcionalidades do iPhone baseando-se no vídeo [Lançamento iPhone 2007](https://www.youtube.com/watch?v=9ou608QQRq8).

## Funcionalidades

### Reprodutor Musical
- `tocar()`
- `pausar()`
- `selecionarMusica(String musica)`

### Aparelho Telefônico
- `ligar(String numero)`
- `atender()`
- `iniciarCorreioVoz()`

### Navegador na Internet
- `exibirPagina(String url)`
- `adicionarNovaAba()`
- `atualizarPagina()`

## Diagrama UML

```mermaid
classDiagram
    class ReprodutorMusical {
        +tocar()
        +pausar()
        +selecionarMusica(String musica)
    }

    class AparelhoTelefonico {
        +ligar(String numero)
        +atender()
        +iniciarCorreioVoz()
    }

    class NavegadorInternet {
        +exibirPagina(String url)
        +adicionarNovaAba()
        +atualizarPagina()
    }

    class iPhone

    iPhone ..|> ReprodutorMusical
    iPhone ..|> AparelhoTelefonico
    iPhone ..|> NavegadorInternet
