// Alligator class that inherits from Animal and implements Countable
public class Alligator extends Animal implements Countable {

    private Sheep sheep;  // Reference to a Sheep instance

    // Default constructor
    public Alligator() {
        this.count = 0;  // Initialize count to zero
        this.sheep = new Sheep();  // Create a new Sheep instance by default
    }

    // Parameterized constructor that accepts a Sheep instance
    public Alligator(Sheep sheep) {
        this.count = 0;  // Initialize count to zero
        this.sheep = sheep;  // Initialize the reference to Sheep instance
    }

    // Override incrementCount to add 1 alligator and deduct 1 sheep if possible
    @Override
    public void incrementCount() {
        count++;  // Add one alligator
        
        // Check if there are any sheep to deduct
        if (sheep != null) {
            sheep.subtractSheep();
        }

        // Display the current status
        if (count > 0) {
            System.out.println("Alligator count: " + count + " - Watch out! Alligators are hungry!");
        }
    }
}
