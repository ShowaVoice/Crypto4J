## [Back to Development Manual](../start.md)
***
import crypto4j.Crypto4J;

import java.nio.charset.StandardCharsets;

public class Main {
public static void main(String[] args) {

        // string
        String pwd = Crypto4J.Unicode.encrypt("admin123");
        System.out.println(pwd);
        System.out.println(Crypto4J.Unicode.decrypt(pwd));

        // bytes
        pwd = Crypto4J.Unicode.encrypt("admin123".getBytes(StandardCharsets.UTF_8));
        System.out.println(pwd);
        System.out.println(Crypto4J.Unicode.decrypt(pwd));
    }
}
```