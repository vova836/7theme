using System;
using System.Collections.Generic;

public struct Warehouse
{
    public string Name;
    public int Capacity;
    public string Location;

    public void DisplayInfo()
    {
        Console.WriteLine($"Warehouse {Name} located in {Location} with capacity of {Capacity} units.");
    }

    public int CalculateFreeSpace(int currentOccupied)
    {
        return Capacity - currentOccupied;
    }
}

class Program
{
    static void Main()
    {
        Warehouse warehouse1;
        warehouse1.Name = "Warehouse 1";
        warehouse1.Capacity = 1000;
        warehouse1.Location = "City A";

        Warehouse warehouse2 = new Warehouse
        {
            Name = "Warehouse 2",
            Capacity = 500,
            Location = "City B"
        };

        var warehouse3 = new Warehouse
        {
            Name = "Warehouse 3",
            Capacity = 800,
            Location = "City C"
        };

        List<Warehouse> warehouses = new List<Warehouse>();
        warehouses.Add(warehouse1);
        warehouses.Add(warehouse2);
        warehouses.Add(warehouse3);

        Console.WriteLine("Warehouses list:");
        foreach (var warehouse in warehouses)
        {
            warehouse.DisplayInfo();
            int freeSpace = warehouse.CalculateFreeSpace(200);
            Console.WriteLine($"Free space available: {freeSpace} units");
            Console.WriteLine();
        }
    }
}using System;
using System.Collections.Generic;

public struct Warehouse
{
    public string Name;
    public int Capacity;
    public string Location;

    public void DisplayInfo()
    {
        Console.WriteLine($"Warehouse {Name} located in {Location} with capacity of {Capacity} units.");
    }

    public int CalculateFreeSpace(int currentOccupied)
    {
        return Capacity - currentOccupied;
    }
}

class Program
{
    static void Main()
    {
        Warehouse warehouse1;
        warehouse1.Name = "Warehouse 1";
        warehouse1.Capacity = 1000;
        warehouse1.Location = "City A";

        Warehouse warehouse2 = new Warehouse
        {
            Name = "Warehouse 2",
            Capacity = 500,
            Location = "City B"
        };

        var warehouse3 = new Warehouse
        {
            Name = "Warehouse 3",
            Capacity = 800,
            Location = "City C"
        };

        List<Warehouse> warehouses = new List<Warehouse>();
        warehouses.Add(warehouse1);
        warehouses.Add(warehouse2);
        warehouses.Add(warehouse3);

        Console.WriteLine("Warehouses list:");
        foreach (var warehouse in warehouses)
        {
            warehouse.DisplayInfo();
            int freeSpace = warehouse.CalculateFreeSpace(200);
            Console.WriteLine($"Free space available: {freeSpace} units");
            Console.WriteLine();
        }
    }
}
