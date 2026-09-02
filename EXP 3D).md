import java.awt.*;
import java.awt.event.*;

public class LoginForm extends Frame implements ActionListener {

    TextField usernameField, passwordField;
    Button loginButton;

    LoginForm() {
        setTitle("Login Form");
        setLayout(new FlowLayout());

        Label userLabel = new Label("Username:");
        usernameField = new TextField(15);

        Label passLabel = new Label("Password:");
        passwordField = new TextField(15);
        passwordField.setEchoChar('*');

        loginButton = new Button("Login");
        loginButton.addActionListener(this);

        add(userLabel);
        add(usernameField);
        add(passLabel);
        add(passwordField);
        add(loginButton);

        setSize(300, 200);
        setVisible(true);

        addWindowListener(new WindowAdapter() {
            public void windowClosing(WindowEvent e) {
                dispose();
            }
        });
    }

    public void actionPerformed(ActionEvent e) {
        if (e.getSource() == loginButton) {
            System.out.println("Username entered: "
                               + usernameField.getText());
            System.out.println("Login button clicked.");
        }
    }

    public static void main(String[] args) {
        new LoginForm();
    }
}

output:

<img width="1402" height="1122" alt="JAVA 3d)" src="https://github.com/user-attachments/assets/555ea4f2-65d5-4562-859d-1dec32b12ed9" />
