# Função desenvolvido em Dart/Javascript

Implemente uma função que receba um número inteiro positivo e retorne o somatório de todos os valores
inteiros divisíveis por 3 ou 5 que sejam inferiores ao número passado.

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
      print("Soma dos valores divisiveis por 3 ou 5: " + soma.toString());
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

## Instruções para executar o código em Javascript

```javascript
var soma = 0;
var valido = false;
    
    while(!valido) {
        num = prompt("Digite um número: ");
        
        if(isNaN(num) || num.trim() === ""){
            console.log("Digite um número válido");
        }else {
            valido = true;
        }
    }
    
    num = parseInt(num);
    
    for(i = 1;i < num;i++){
    
        if((i % 5 == 0) || (i % 3 == 0)){
            soma += i;
        }
    }
    
    console.log("A soma dos números divisiveís por 5 ou 3 é de: " + soma);
```

1. Acesse o compilador Javascript em [Programiz](https://www.programiz.com/javascript/online-compiler/#google_vignette).
2. Copie e cole código no compilador.
3. Clique em "Run".
