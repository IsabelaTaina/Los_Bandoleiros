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
```

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


# Registro de Erros e Correções – Instalação do Flutter

# 📋 Registro de Erros e Correções – Instalação do Flutter

Este registro documenta **apenas os erros que ocorreram até a etapa atual da instalação do Flutter**, bem como os comandos executados e as ações realizadas para correção.

---

## 🛑 Erro 1 – Comando `flutter` não reconhecido no terminal

### Descrição do erro
Ao tentar executar o comando:

```dart
flutter --doctor
```


o terminal retornava uma mensagem informando que o comando `flutter` não era reconhecido.

### Causa
O Flutter SDK já estava instalado no computador, porém o caminho da pasta `flutter/bin` **não estava configurado nas variáveis de ambiente (PATH)** do sistema.

### Passos realizados para corrigir
1. Localizei a pasta onde o Flutter SDK foi extraído  
2. Copiei o caminho da pasta `flutter/bin`  
3. Adicionei esse caminho às **Variáveis de Ambiente (PATH)** do Windows  
4. Reiniciei o terminal  
5. Executei novamente o comando:

```dart
flutter --doctor
```


### Resultado
O comando passou a ser reconhecido e o Flutter funcionou corretamente no terminal.

---

## 🛑 Erro 2 – Falha ao aceitar licenças do Android SDK

### Descrição do erro
Após executar:

```dart
flutter --doctor
```

o Flutter indicou erro relacionado ao Android SDK.  
Ao tentar aceitar as licenças, ocorreu o seguinte erro:

flutter doctor --android-licenses
Could not find an option named "--android-licenses".


Em uma nova tentativa, apareceu o erro:

Android sdkmanager not found.
Update to the latest Android SDK and ensure that the cmdline-tools are installed.


### Causa
O **Android SDK não estava totalmente configurado**, pois os **Command-line Tools (sdkmanager)** ainda não estavam instalados ou reconhecidos pelo sistema.

### Passos realizados para corrigir
1. Abri o **Android Studio**
2. Acessei o **SDK Manager**
3. Instalei os **Android SDK Command-line Tools**
4. Verifiquei a configuração do Android SDK
5. Executei novamente o comando no terminal:

```dart
flutter doctor --android-licenses
}
```

6. Aceitei todas as licenças solicitadas

### Resultado
Após a instalação dos componentes corretos, o comando funcionou e as licenças do Android foram aceitas com sucesso.

---

## 🧩 Situação atual

Até este momento:

- ✅ O Flutter SDK está instalado  
- ✅ O comando `flutter` funciona no terminal  
- ✅ O Android SDK está configurado  
- ✅ As licenças do Android foram aceitas  
- ⚠️ Outros erros **ainda não ocorreram**, pois as próximas etapas ainda não foram realizadas  

Este registro será atualizado conforme novas etapas forem executadas.


