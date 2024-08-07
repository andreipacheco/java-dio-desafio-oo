# 📱 iPhone Project

Este projeto simula as funcionalidades básicas de um iPhone utilizando Programação Orientada a Objetos (POO) em Java. As funcionalidades implementadas incluem um Reprodutor Musical, um Aparelho Telefônico e um Navegador na Internet. 

## 📂 Estrutura do Projeto

iPhoneProject/
├── src/
│ ├── main/
│ │ ├── java/
│ │ │ ├── com/
│ │ │ │ ├── iphone/
│ │ │ │ │ ├── iPhone.java
│ │ │ │ │ ├── interfaces/
│ │ │ │ │ │ ├── ReprodutorMusical.java
│ │ │ │ │ │ ├── AparelhoTelefonico.java
│ │ │ │ │ │ ├── NavegadorInternet.java
└── README.md


## 🛠️ Funcionalidades

### Reprodutor Musical
- `tocar()`: Reproduz uma música.
- `pausar()`: Pausa a música em reprodução.
- `selecionarMusica(String musica)`: Seleciona uma música para reprodução.

### Aparelho Telefônico
- `ligar(String numero)`: Faz uma ligação para um número específico.
- `atender()`: Atende uma chamada.
- `iniciarCorreioVoz()`: Inicia o correio de voz.

### Navegador na Internet
- `exibirPagina(String url)`: Exibe uma página da web.
- `adicionarNovaAba()`: Adiciona uma nova aba no navegador.
- `atualizarPagina()`: Atualiza a página atual.

## 🚀 Como Executar

1. **Clone o repositório:**
    ```bash
    git clone https://github.com/seu-usuario/iPhoneProject.git
    cd iPhoneProject
    ```

2. **Compile os arquivos Java:**
    ```bash
    javac src/main/java/com/iphone/interfaces/*.java src/main/java/com/iphone/iPhone.java
    ```

3. **Execute o programa:**
    ```bash
    java -cp src/main/java com.iphone.iPhone
    ```

4. **Teste as funcionalidades:**
    - Abra a classe `iPhone.java` e adicione chamadas aos métodos implementados no método `main` para testar as funcionalidades.

## 📝 Exemplo de Uso

```java
public class Main {
    public static void main(String[] args) {
        iPhone meuIphone = new iPhone();

        // Testando Reprodutor Musical
        meuIphone.selecionarMusica("Minha Musica Favorita");
        meuIphone.tocar();
        meuIphone.pausar();

        // Testando Aparelho Telefônico
        meuIphone.ligar("123456789");
        meuIphone.atender();
        meuIphone.iniciarCorreioVoz();

        // Testando Navegador na Internet
        meuIphone.exibirPagina("https://www.exemplo.com");
        meuIphone.adicionarNovaAba();
        meuIphone.atualizarPagina();
    }
}
