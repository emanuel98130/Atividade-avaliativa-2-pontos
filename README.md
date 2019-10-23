Questão 2 
Letra a: 
void main() {
int a = 10;
int b = 12;
String nome = 'inteiros';
print('Hola olhe os numeros $a, $b. Eles são $nome.');
}

Letra b: 
main(){
numeros();
}
void numeros(){
  for(int a = 1; a < 11; a++){
    print('$a');
  }
}

Letra c: 
main() {
  int a = 50;
  numeros(a);
}

void numeros(int b) {
  for (int a = 1; a <= b; a++) {
    print('$a');
  }
}

Letra d: 
void main() {
  int a = 5;
  soma(a);
}
void soma(int a){
  int total = 0;
  for(int b = 1; b <= a; b++){
    total = total + b;
  }
  print('Total = $total');
}

Letra e:
class Carro{
  String modelo;
  String fabrica;
  String marca;
Carro(String modelo, String fabrica, String marca){
  this.modelo = modelo;
  this.fabrica = fabrica;
  this.marca = marca;
}
    
  void tipo_modelo (){
    print('O seu carro é do modelo $modelo.');
  }

  void fabricado(){
    print('O seu carro foi fabricado na fabrica $fabrica.');
  }
  
  void tipo_marca(){
    print('O seu carro é da marca $marca.');
  }

}


void main(){
  Carro c1  = Carro ('Sport','Alagoas','FIAT');
  c1.tipo_modelo();
  c1.fabricado();
  c1.tipo_marca();
}





/// Atividade da prova:

class Banco{
  double depositoO;
  double saqueE;
  double saldoO = 0;
  
  
  double deposito(double valor){
    saldoO = saldoO + valor;
    print('Deposito efetuado!');
    print('Saldo atual na conta: $saldoO');
  }
  
  double saque(double valor){
    if(valor > saldoO){
    print('Saque não diponivel');
    print('Saldo atual na conta: $saldoO');
    }
    else{
    saldoO = saldoO - valor;
    print('saque efetuado!');
    print('Saldo atual na conta: $saldoO');
    }
  }
  void tranferencia (int contaA, double valor){
    if(valor > saldoO){
    print('Transferência não diponivel');
    print('Saldo atual na conta: $saldoO');
    }
    else{
    saldoO = saldoO - valor;
    print('Valor transferido da conta 1234 para a conta $contaA no valor de $valor.');
    print('Saldo atual na conta: $saldoO');
     }
  }
}


void main() {
 Banco c1 = Banco();
}
