```cs
public class User
{
    public string Name { get; set; }
    public int Age { get; set; }
    public string Subject { get; set; }
    public List<string> Skills { get; set; }
    public bool IsCodingRightNow { get; set; }

    public User()
    {
        this.Name = "Ibrohim";
        this.Age = 16;
        this.Subject = "Programming";
        this.Skills = new List<string> { "C#", "SQL", "Angular", "Debugging" };
        this.IsCodingRightNow = true;
    }

    public void Code()
    {
        if (IsCodingRightNow)
        {
            Console.WriteLine($"{Name} is currently deep in the coding zone! 🎧💻");
        }
        else
        {
            Console.WriteLine($"{Name} is taking a well-deserved break... or maybe just pretending to work. 😴");
        }
    }

    public override string ToString()
    {
        return $"Meet {Name}, {Age} years old, mastering {Subject} with skills in {string.Join(", ", Skills)}.";
    }
}

```
