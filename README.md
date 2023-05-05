# TypescriptLab

// C# Code
public class Dog
{
	public string Name { get; set; }
	public string Breed { get; set; }

	public Dog(string name, string breed)
	{
    	Name = name;
    	Breed = breed;
	}

	public string Bark()
	{
    	return "Woof!";
	}
}

string[] dogBreeds = new string[] { "Labrador", "Golden Retriever", "Bulldog" };

public string GetRandomBreed(string[] breeds)
{
	Random random = new Random();
	int index = random.Next(breeds.Length);
	return breeds[index];
}

// js

class Dog {
  constructor(name, breed) {
    this.Name = name;
    this.Breed = breed;
  }
  
  Bark() {
    return "Woof!";
  }
}

const dogBreeds = ["Labrador", "Golden Retriever", "Bulldog"];

function GetRandomBreed(breeds) {
  const index = Math.floor(Math.random() * breeds.length);
  return breeds[index];
}

//Typescript

class Dog {
  Name: string;
  Breed: string;
  
  constructor(name: string, breed: string) {
    this.Name = name;
    this.Breed = breed;
  }
  
  Bark(): string {
    return "Woof!";
  }
}

const dogBreeds: string[] = ["Labrador", "Golden Retriever", "Bulldog"];

function GetRandomBreed(breeds: string[]): string {
  const index: number = Math.floor(Math.random() * breeds.length);
  return breeds[index];
}
