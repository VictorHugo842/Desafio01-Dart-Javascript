# Desafio01 - Dart/Javascript

## Instruções para executar o código em Dart
   
```dart
import 'dart:io';

void main() {
  int soma = 0;

  print("Digite o valor inteiro:");
  String? input = stdin.readLineSync();
  
  if (input != null) {
    try {
      int numero = int.parse(input);

      for(int i = 1; i < numero; i++){
        if((i % 5 == 0) || (i % 3 == 0)){
          soma += i;
        }
      }
      print("Soma dos valores divisíveis por 3 ou 5: " + soma.toString());
    } catch(e) {
      print("Por favor, insira um valor correto.");
    }
  } else {
    print("Nenhum valor digitado");
  }
}
```

1. Acesse o compilador Dart em [Online Dart Compiler](https://www.adaface.com/online-compiler/online-dart-compiler).
2. Copie e cole código no compilador.
3. Clique em "Run".
