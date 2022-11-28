void main() {
  Person person = new Person(nombre:'miguel ',sexo:'masculino');
  person.apellido='rodriguez';
  person.edad= 28;
  print( '${person.nombre }');
  print('${person.edad}');
  print('${person.apellido}');
  print('${person.nombreompleto()}');
  person.edadMas(person.edad);
}



class Person {
  
  String? nombre, sexo, apellido;
  int? edad;
  
  Person({this.nombre,this.sexo});
  
  String nombreompleto() {
    return '$nombre $apellido';    
  }
  
  void edadMas(num) {
    int n = num + 3;
    print('la edad futura es $n');
  
  }
}