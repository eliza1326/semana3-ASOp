# semana3-ASOp
/Nombre: Jeanneth Farinango
// Fecha: 2024-12-15
// Hoja 1

using System;

namespace FigurasGeometricas
{
    // Clase para la figura Círculo
    public class Circulo
    {
        // Variable privada para el radio
        private double radio;

        // Constructor que inicializa el radio
        public Circulo(double radio)
        {
            this.radio = radio;
        }

        // Método para calcular el área del círculo
        // Área = PI * radio^2
        public double CalcularArea()
        {
            return Math.PI * radio * radio;
        }

        // Método para calcular el perímetro (circunferencia) del círculo
        // Perímetro = 2 * PI * radio
        public double CalcularPerimetro()
        {
            return 2 * Math.PI * radio;
        }
    }

    // Clase para la figura Rectángulo
    public class Rectangulo
    {
        // Variables privadas para la base y la altura
        private double baseRectangulo;
        private double altura;

        // Constructor que inicializa base y altura
        public Rectangulo(double baseRectangulo, double altura)
        {
            this.baseRectangulo = baseRectangulo;
            this.altura = altura;
        }

        // Método para calcular el área del rectángulo
        // Área = base * altura
        public double CalcularArea()
        {
            return baseRectangulo * altura;
        }

        // Método para calcular el perímetro del rectángulo
        // Perímetro = 2 * (base + altura)
        public double CalcularPerimetro()
        {
            return 2 * (baseRectangulo + altura);
        }
    }

    // Clase principal para probar las figuras
    class Program
    {
        static void Main(string[] args)
        {
            // Crear un objeto de la clase Circulo con radio 5
            Circulo circulo = new Circulo(5);
            Console.WriteLine("Círculo:");
            Console.WriteLine("Área: " + circulo.CalcularArea());
            Console.WriteLine("Perímetro: " + circulo.CalcularPerimetro());

            // Crear un objeto de la clase Rectángulo con base 4 y altura 6
            Rectangulo rectangulo = new Rectangulo(4, 6);
            Console.WriteLine("\nRectángulo:");
            Console.WriteLine("Área: " + rectangulo.CalcularArea());
            Console.WriteLine("Perímetro: " + rectangulo.CalcularPerimetro());
        }
    }
}

