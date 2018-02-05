# Java
Java begginner projects
public class Animal {
	
	int age;

	  public void dogHealthStatus() {
		  
	  
		  String mood="Hungry";
		
		  
		   switch (mood){
		   
		   case "Sad": System.out.println("Take your pet to the Vet");
			   break;
			  
	       case "Playful": System.out.println("Enjoy your pet");
	       break;
	       
	       case "Hungry":  System.out.println("Feed your pet");
	break; 
		   }
				   
			   
	  }
		 
		   
	


	public static void main(String[] args) {
		// TODO Auto-generated method stub

	}

}



public class Dog extends Animal {
	// Instance variable  integer age, string breed,//
	int age; 
	String breed; 
	String name; 
	String color; 
	String mood;
	
  // line 4 creates constructor specifies initial dog age by adding a parameter  //  
	public Dog(String dogsName, int dogsAge, String dogsBreed, String dogsColor, String dogsMood) {
		
		age = dogsAge;
		breed=dogsBreed;
		name=dogsName;
		color=dogsColor;
		mood=dogsMood;
	} 
	
	public void dogDescriptiveStatus() {
		
		System.out.println( name + " is " + age + " year(s) old, and he/she is a " + breed + " and color " + color + " . " + 
		"The mood of your dog is " + mood);
	}
	
	
	
	public static void main(String[] args) {
		// TODO Auto-generated method stub

		
		 Dog dog1=new Dog("Chispita", 2 , "German Sheperd", "Black", "Sad");
		 Dog dog2=new Dog("Tequila" , 1, "Chihuahua", "Brown", "Playful"); 
		 Dog dog3=new Dog("Bandido", 4, "Streeter" , "White", "Hungry");
		   dog1.dogDescriptiveStatus();
		   dog1.dogHealthStatus();
		  
		   
		   dog2.dogDescriptiveStatus();
		   dog2.dogHealthStatus();
		   
		   dog3.dogDescriptiveStatus();
		   dog3.dogHealthStatus();
		
	}

}
