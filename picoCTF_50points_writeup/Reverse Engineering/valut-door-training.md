# valut-door-training

## Description

Your mission is to enter Dr. Evil's laboratory and retrieve the blueprints for his Doomsday Project. The laboratory is protected by a series of locked vault doors. Each door is controlled by a computer and requires a password to open. Unfortunately, our undercover agents have not been able to obtain the secret passwords for the vault doors, but one of our junior agents obtained the source code for each vault's computer! You will need to read the source code for each level to figure out what the password is for that vault door. As a warmup, we have created a replica vault in our training facility. The source code for the training vault is here:
``` bash
import java.util.*;

class VaultDoorTraining {
public static void main(String args[]) {
VaultDoorTraining vaultDoor = new VaultDoorTraining();
Scanner scanner = new Scanner(System.in); 
System.out.print("Enter vault password: ");
String userInput = scanner.next();
String input = userInput.substring("picoCTF{".length(),userInput.length()-1);
if (vaultDoor.checkPassword(input)) {
System.out.println("Access granted.");
} else {
System.out.println("Access denied!");
}
}

// The password is below. Is it safe to put the password in the source code?
// What if somebody stole our source code? Then they would know what our
// password is. Hmm... I will think of some ways to improve the security
// on the other doors.
//
// -Minion #9567
public boolean checkPassword(String password) {
return password.equals("w4rm1ng_Up_w1tH_jAv4_3808d338b46");
}
}

```
## Solution

There is code password.equals ("w4rm1ng _ Up _ w1tH _ jAv4 _ 3808 d 338 b 46") that uses an equals method to compare strings, so the answe picoCTF{w4rm1ng_Up_w1tH_jAv4_3808d338b46}

## Flag

picoCTF{w4rm1ng_Up_w1tH_jAv4_3808d338b46}
