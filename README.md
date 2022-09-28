# java-weeklysalary-JOptionPane
input ug weekly salary tas deduction then e solve daun sa prog


import javax.swing.JOptionPane;

public class weeklySalary {

	public static void main(String[] args) {
		
		String wageString, dependentsString;
		double wage, weeklyPay;
		int dependents;
		final double hrs_in_week = 332.5;
		
		wageString = JOptionPane.showInputDialog (null, "Enter employee's hourly wage", "Salary Dialog 1",JOptionPane.INFORMATION_MESSAGE);
		
		weeklyPay = Double.parseDouble(wageString) * hrs_in_week;
		dependentsString = JOptionPane.showInputDialog (null, "How many dependents?", "Salary Dialog 2",JOptionPane.QUESTION_MESSAGE);
		
		dependents = Integer.parseInt(dependentsString);
		JOptionPane.showInputDialog (null, "weekly salary is Php" + weeklyPay + "\nDeductions will be made for " + dependents + " dependents ");
				
		System.exit(0);		
	}
}
