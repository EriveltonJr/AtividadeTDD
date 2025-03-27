# TDD - Money Example (Kent Beck)

Este projeto é uma implementação prática do exemplo apresentado nos capítulos 1 a 11 do livro **Test-Driven Development: By Example**, de Kent Beck.

O exercício foi realizado como parte da disciplina de Engenharia de Software.

## 📚 Objetivo

Reproduzir uma sessão de desenvolvimento usando **TDD (Test-Driven Development)**, passando por:

- Escrita de testes com JUnit
- Desenvolvimento incremental (vermelho → verde → refatorar)
- Refatorações para eliminar duplicações
- Implementação de uma hierarquia de classes (`Money`, `Dollar`, `Franc`)
- Unificação final em uma única classe `Money`

## 🛠️ Como rodar os testes

### Requisitos

- Java JDK 11 ou superior
- Terminal configurado com `javac` e `java`
- JUnit 4.13.2 e Hamcrest 1.3

### Estrutura do projeto

```
📦 projeto
├── lib/
│   ├── junit-4.13.2.jar
│   └── hamcrest-core-1.3.jar
├── src/
│   ├── Money.java
│   └── MoneyTest.java
```

### Passos para rodar os testes via terminal:

1. Compile os arquivos:

```bash
javac -cp "lib/*" -d bin src/*.java
```

2. Execute os testes:

```bash
java -cp "lib/*:bin" org.junit.runner.JUnitCore MoneyTest
```

💡 *(No Windows, use `;` em vez de `:` no classpath)*:
```cmd
java -cp "lib/*;bin" org.junit.runner.JUnitCore MoneyTest
```

## ✅ Status dos testes

Todos os testes foram executados com sucesso:

```
JUnit version 4.13.2
...
OK (3 tests)
```

## 👤 Autor

Nome: [Francisco Erivelton]  
Instituição: [IFPI / Análise e Desenvolvimento de Sistemas]
