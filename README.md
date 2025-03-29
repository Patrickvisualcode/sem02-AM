class Alumno {
  String? nombres;
  String? apellidos;

  int? nota_1;
  int? nota_2;
  int? nota_3;


  Alumno(this.nombres, this.apellidos, this.nota_1, this.nota_2, this.nota_3);

  Alumno.notas(this.nota_1, this.nota_2, this.nota_3);


  void mostrarInformacion() {
    // Mostrar Nombres y Apellidos
    print('Nombres y Apellidos del Alumno: $nombres $apellidos');
    print('Notas:');
    

    if (nota_1 != null) {
      print('Nota 1: $nota_1');
    }
    
    if (nota_2 != null) {
      print('Nota 2: $nota_2');
    }
    
    if (nota_3 != null) {
      print('Nota 3: $nota_3');
    }
  }
}

void main() {

  Alumno patrick = Alumno('Patrick', 'Chavez', 8, 9, 7);


  patrick.mostrarInformacion();
}
