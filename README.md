# Softuni-projects
Courses for my education @ Softuni
namespace _11.Orders
{
    internal class Program
    {
        static void Main(string[] args)
        {
            int ordersCount = int.Parse(Console.ReadLine());
            double total = 0;
            for(int i = 1; i <= ordersCount; i++)
            {
                double pricePerCpasule = double.Parse(Console.ReadLine());
                int days = int.Parse(Console.ReadLine());
                int capsuleCount = int.Parse(Console.ReadLine());   

                double price= (days*capsuleCount) * pricePerCpasule;
                total += price;
                Console.WriteLine($"The price for the coffee is: ${price:F2}");
            }
            Console.WriteLine($"Total: ${total:F2}");
        }
    }
}
    
