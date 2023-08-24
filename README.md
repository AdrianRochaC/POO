# POO

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
