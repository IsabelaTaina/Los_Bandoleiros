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
