# Programacion-II
repositorio para clases de prog II
------------------------------------------------------------------------------------------------------
CLASE 16/08   [JAVA]
------------------------------------------------------------------------------------------------------
public class Main {

    public static void main(String[] args) {
	auto a1 = new auto();
	    a1.color = "Blanco";

	auto a2 = new auto();
	    a2.color = "Negro";

	auto a3 = new auto();
	    a3.color = "Azul";


	a1.setMarca("Volskwagen");
	a1.cantidadPuertas = 4;
	a1.modelo("2016");

	    a1.cambiarColor("Negro");

	System.out.println(a1);

    }
}

------------------------------------------------------------------------------------------------------
public class auto {
    //Atributos

    String color;
    String nombre;
    String marca;
    String modelo;
    int cantidadPuertas;

    //este setea el valor
    public void setMarca (String m) {
        marca = m;
    }

    //este obtiene la marca
    public String getMarca () {
        return marca;
    }



    //este modifica la variable
    void cambiarColor(String c) {
        color = c;
    }
 
    //asi si ponen que el auto tiene -1 puertas, o 100 puertas, hara que el auto tenga 0 puertas o 4 puertas por defecto
    public void setCantidadPuertas(int cp){
        if (cp < 0)
            cantidadPuertas = 0;
        else if (cp > 5)
            cantidadPuertas =5;
        else
            cantidadPuertas = cp;
    }
}


