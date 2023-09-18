# POO

package ClasesYObjetos;

public class Figura {
    String nombre;
    String lados;
    String angulos;
    String clasificacion;
    String area;
    String perimetro;
    String elementos;
    String propiedades;

#Animales
package ClasesYObjetos;

public class Animal {
    String animal;
    String color;
    int peso;
    int tamono;
    String sueño;
    String dieta;
    String velocidad;
    String peligro;
    String defensa;
    String pelo;
    
    public static void main(String[] args) {
    
    Animal animal1 = new Animal();
        
    animal1.animal = "Leon";
    animal1.color = "Amarillo";
    animal1.peso = 150;
    animal1.tamono = 2;
    animal1.pelo = "Corto";
    animal1.dieta = "Estrictamente carnivora de los animales de la sabana";
    animal1.sueño = "Al rededor de 20h al día";
    animal1.velocidad = "74 km/h";
    animal1.peligro = "La caza constante de leones, su desnutrición por poca comida";
    animal1.defensa = "La marca de territorio con orina, su imponente rugido y su velocidad para cazar a los intrusos";
    
    
        System.out.println("Animal 1");
        System.out.println("");
        System.out.println("Atributos");
        System.out.println("El animal es: " + animal1.animal);
        System.out.println("El color del animal es: " + animal1.color);
        System.out.println("El peso del animal es: " + animal1.peso + " kg");
        System.out.println("El tamaño del animal es: " + animal1.tamono + " m");
        System.out.println("El tipo de pelo del animal es: " + animal1.pelo);
        System.out.println("");
        System.out.println("Metodos");
        System.out.println("La dieta del animal es: " + animal1.dieta);
        System.out.println("La rutina de sueño del animal es: " + animal1.sueño);
        System.out.println("La velocidad del animal es: " + animal1.velocidad);
        System.out.println("");
        System.out.println("Eventos");
        System.out.println("El peligro del animal es: " + animal1.peligro);
        System.out.println("La defensa del animal es: " + animal1.defensa);
    }    
} 

#Coches
package ClasesYObjetos;

public class Coche {
    //Atributos
    String color;
    String marca;
    int km;
    
    public static void main(String[] args) {
        Coche coche1 = new Coche();
        
        coche1.color = "Blanco";
        coche1.marca = "Audi";
        coche1.km = 0;
        
        System.out.println("Coche 1");
        System.out.println("El color del coche 1 es: " + coche1.color);
        System.out.println("La marca del coche 1 es: " + coche1.marca);
        System.out.println("El kilometraje del coche 1 es: " + coche1.km);
        
        Coche coche2 = new Coche();
        
        coche2.color = "Rojo";
        coche2.marca = "Ferrari";
        coche2.km = 100;
        
        System.out.println("");
        System.out.println("Coche 2");
        System.out.println("El color del coche 2 es: " + coche2.color);
        System.out.println("La marca del coche 2 es: " + coche2.marca);
        System.out.println("El kilometraje del coche 2 es: " + coche2.km);
        
        Coche coche3 = new Coche();
        
        coche3.color = "Negro";
        coche3.marca = "Camaro";
        coche3.km = 200;
        
        System.out.println("");
        System.out.println("Coche 3");
        System.out.println("El color del coche 3 es: " + coche3.color);
        System.out.println("La marca del coche 3 es: " + coche3.marca);
        System.out.println("El kilometraje del coche 3 es: " + coche3.km);
    }
}

# Ejercicio arreglos nombres y carreras
     public static void main (String [] args){
     Scanner lector = new Scanner (System.in);

     String nombres [] = new String [20];
     String carrera [] = new String [20];
     int i, lim;
     System.out.println ("Ingrese limite del arreglo");
     lim = lector.nextInt();

     for (i = 0; i < lim; i++){
     System.out.println ("Nombre " + (i + 1) + ", " + "Carrera " + (i + 1) );
     nombres[i]

# Ejercicio Primeros Numeros
    public static void main(String[] args) {
        Scanner scanner = new Scanner (System.in);
        System.out.println("Ingrese la cantidad de numeros que desea inegresar: ");
        int n = scanner.nextInt();
            int[] numeros = new int [n];
            for(int i = 0; i < n; i++){
                System.out.println("Ingrese el numero " + (i + 1) + ": ");
                numeros [i] = scanner.nextInt();
            }
            System.out.println("Los primeros 5 numeros insertados son: ");
            for (int i = 0; i < 5; i++){
                System.out.println(numeros [i]);
            }
    }
    }

# Ejercicio Mayor y Menor y Suma
    public static void main(String[] args) {
        Scanner scanner = new Scanner (System.in);
        int mayor = 0, menor = 0, suma = 0, numero;
        while (true){
            System.out.println("Ingrese un numero: ");
            numero = scanner.nextInt();
            if(numero == 0){
                break;
            }
            if(numero > mayor) {
                mayor = numero;
            }
            if(numero < menor){
                menor = numero;
            }
            suma += numero;
        }
        System.out.println("El numero mayor es: " + mayor);
        System.out.println("El numero menor es: " + menor);
        System.out.println("La suma de los numeros es: " + suma);
    }
    }

# Ejercicio multiplos

        public static void main(String[] args) {
        Scanner scanner = new Scanner(System.in);
        int[] numbers = new int[5];
        int multiplos3 = 0, multiplos5 = 0, multiplos3y5 = 0, multiplosninguno = 0;

        System.out.println("Ingrese 5 números:");

        // Ingresar los números
        for (int i = 0; i < 5; i++) {
            System.out.print("Número " + (i + 1) + ": ");
            numbers[i] = scanner.nextInt();
        }

        // Identificar los múltiplos
        System.out.println("Resultados:");
        for (int number : numbers) {
            if (number % 15 == 0) {
                multiplos3 = multiplos3 + 1;
                multiplos5 = multiplos5 + 1;
                //System.out.println(number + " es múltiplo de 3 y 5.");
            } else if (number % 3 == 0) {
                multiplos3 = multiplos3 + 1; 
                //System.out.println(number + " es múltiplo de 3.");
            } else if (number % 5 == 0) {
                multiplos5 = multiplos5 + 1;
                //System.out.println(number + " es múltiplo de 5.");
            } else {
                multiplosninguno = multiplosninguno + 1;
                //System.out.println(number + " no es múltiplo de 3 ni de 5.");
            }
        }
        System.out.println("Multiplos de 3:");
        System.out.println(multiplos3);
        System.out.println("Multiplos de 5:");
        System.out.println(multiplos5);
    }
}

# Ejercicio tabla del 5
    public static void main(String[] args) {
        int resultados, m;
        
        for(resultados = 1; resultados<=20; resultados++){
            m = 5 * resultados;
            System.out.println(5 + " * " + resultados + " = " + m);
        }
    }
}

# Ejercico tablas 
    public static void main(String[] args) {
        Scanner tabla = new Scanner (System.in);
        
        int r, m, n;
        
        System.out.println("Ingrese numero:");
        r = tabla.nextInt();
        if(r<=10){
        for(n = 1; n<=12; n++){
            m = r * n;
            System.out.println(r + " * " + n + " = " + m);
            }
        }else{
            System.out.println("Valores invalidos");
        }
    }
}
