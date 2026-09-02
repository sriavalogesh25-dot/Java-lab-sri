import java.awt.*;

public class StudentRegistrationForm extends Frame {

    StudentRegistrationForm() {

        setTitle("Student Registration Form");
        setLayout(new GridLayout(5, 2, 10, 10));

        add(new Label("Name:"));
        add(new TextField());

        add(new Label("Roll Number:"));
        add(new TextField());

        add(new Label("Class:"));
        add(new TextField());

        add(new Label("Email:"));
        add(new TextField());

        add(new Label(""));
        add(new Button("Register"));

        setSize(350, 250);
        setVisible(true);
    }

    public static void main(String[] args) {
        new StudentRegistrationForm();
    }
}

OUTPUT:

<img width="1536" height="1024" alt="JAVA 3e)" src="https://github.com/user-attachments/assets/0f948c43-b4fd-4377-9f5c-a22fa3a3b03e" />


