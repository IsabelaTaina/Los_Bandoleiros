# Diário de Aula – Introdução ao Flutter

## 🧠 Objetivo
Registrar o processo de instalação e entendimento inicial do Flutter, demonstrando que compreendo **a estrutura de um projeto Flutter** e **a função de cada arquivo**, mesmo antes de começar a programar de fato.

---

## 🔹 Tarefa 1 – Instalação do Flutter

### O que é o Flutter?
O Flutter é um **framework de desenvolvimento** criado pelo Google que permite criar **aplicativos multiplataforma** (Android, iOS, Web, Desktop) usando **uma única base de código**, escrita na linguagem **Dart**.

---

### Passos realizados na instalação

1. **Download do Flutter SDK**
   - Baixei o Flutter pelo site oficial
   - Extraí o arquivo para uma pasta no computador

2. **Configuração de variáveis de ambiente**
   - Adicionei o Flutter ao `PATH` do sistema
   - Isso permite usar comandos Flutter no terminal

3. **Verificação da instalação**
   - Executei o comando:
     ```bash
     flutter doctor
     ```
   - Esse comando verifica:
     - Flutter instalado corretamente
     - Dart
     - Android SDK
     - Conexão com editores (VS Code / Android Studio)

📌 O `flutter doctor` é importante porque mostra **o que está funcionando** e **o que ainda precisa ser configurado**.

---

## 🔹 Tarefa 2 – Criação do Projeto Flutter

Após a instalação, criei um novo projeto Flutter.

- Um projeto Flutter já vem com **uma estrutura padrão**
- Essa estrutura é igual para todos os projetos Flutter
- Cada pasta tem uma função específica

---

## 🔹 Estrutura Básica do Projeto Flutter

> “Aqui está a estrutura básica de um projeto Flutter…”

### 📁 `lib/`
- Pasta **mais importante do projeto**
- Contém o **código principal em Dart**
- É onde o aplicativo realmente é construído

📌 Sem a pasta `lib`, o app não funciona.

---

### 📄 `lib/main.dart`
- Arquivo principal do projeto
- Contém a função:

```dart
void main() {
  runApp(const MyApp());
}

## Estrutura do Projeto Flutter

### Arquivo `main.dart`

- Este arquivo é o **ponto de entrada do aplicativo**
- É a **primeira coisa que o Flutter executa** ao iniciar o app
- A função `runApp()` informa ao Flutter **qual widget será exibido na tela**
- Todo aplicativo Flutter começa a partir deste arquivo

📌 Tudo começa pelo `main.dart`.

---

### Arquivo `pubspec.yaml`

- Arquivo de **configuração do projeto**
- Utilizado para definir:
  - Dependências (pacotes externos)
  - Versão do aplicativo
  - Assets (imagens, fontes e ícones)

📌 Sempre que algo novo é adicionado ao projeto, este arquivo costuma ser alterado.

---

## Outras Pastas do Projeto

### Pasta `android/`

- Contém configurações específicas para a plataforma Android
- Geralmente não é alterada no início do desenvolvimento

---

### Pasta `ios/`

- Contém configurações específicas para a plataforma iOS

---

### Pasta `web/`

- Estrutura utilizada quando o aplicativo é executado como um site

---

### Pastas `windows/`, `linux/` e `macos/`

- Contêm configurações específicas para aplicativos desktop

📌 Mesmo existindo várias pastas no projeto, **o código principal permanece na pasta `lib/`**.

---

## Arquivos Auxiliares

### Arquivo `.gitignore`

- Define quais arquivos e pastas **não devem ser enviados para o repositório GitHub**

---

### Arquivo `README.md`

- Arquivo de documentação do projeto
- Utilizado para explicar o objetivo e o funcionamento do aplicativo

---

## Conclusão

Neste momento:

- O Flutter está instalado corretamente
- O projeto foi criado com sucesso
- Ainda não foram desenvolvidas funcionalidades

No entanto, já compreendo:

- Como o projeto Flutter é organizado
- Onde fica o código principal
- Qual é a função de cada arquivo e pasta

Esse conhecimento é essencial antes de iniciar a implementação das funcionalidades do aplicativo.

---

## Próximos Passos

- Entender o que são **widgets**
- Compreender como a **interface do Flutter é construída**
