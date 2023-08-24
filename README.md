# POO

# Ejercicio multiplos


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
