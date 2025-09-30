import java.util.Scanner;

class Employee {
    private String firstName;
    private String lastName;
    private double monthlySalary;

    public Employee() {
        firstName = "";
        lastName = "";
        monthlySalary = 0.0;
    }

    public void set() {
        Scanner sc = new Scanner(System.in);

        System.out.print("Enter first name: ");
        firstName = sc.next();

        System.out.print("Enter last name: ");
        lastName = sc.next();

        System.out.print("Enter monthly salary: ");
        double salary = sc.nextDouble();

        if (salary > 0.0)
            monthlySalary = salary;
        else
            monthlySalary = 0.0;
    }

    public void get() {
        System.out.println("Employee: " + firstName + " " + lastName);
        System.out.println("Monthly Salary: " + monthlySalary);
        System.out.println("Yearly Salary: " + getYearlySalary());
    }

    public double getYearlySalary() {
        return monthlySalary * 12;
    }

    public void giveRaise() {
        monthlySalary = monthlySalary + (monthlySalary * 0.10);
    }
}

public class EmployeeTest {
    public static void main(String[] args) {
        // create two employee objects
        Employee emp1 = new Employee();
        Employee emp2 = new Employee();

        System.out.println("Enter details for Employee 1:");
        emp1.set();

        System.out.println("\nEnter details for Employee 2:");
        emp2.set();

        System.out.println("\nBefore Raise");
        emp1.get();
        emp2.get();

        emp1.giveRaise();
        emp2.giveRaise();

        System.out.println("\nAfter 10% Raise");
        emp1.get();
        emp2.get();
    }
}
