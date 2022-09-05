# `BigInteger` и `BigDecimal`

- у них теоретически нет максимального размера
```java
public class Main {
    public static void main(String[] args) {
        BigInteger integer = new BigInteger("9999999999999999999999999"); // можно и больше
        System.out.println(integer);

        BigDecimal decimal = new BigDecimal("123.9999999999999999999999999"); // можно и больше
        System.out.println(decimal);
    }
}
```

- Передача строки в качестве параметра — только один из возможных конструкторов.
- Эти объекты являются неизменяемыми (`Immutable`).

```java
import java.math.BigInteger;
public class Main {
   public static void main(String[] args) {
       BigInteger integer = new BigInteger("1111111111111111111111111111111111");
       System.out.println(integer);
       // integer.add(BigInteger.valueOf(33333333)); - так ничего не будет, Immutable!
       BigInteger result = integer.add(BigInteger.valueOf(33333333));
       System.out.println(result);
   }
}
```

[продолжение](https://javarush.ru/groups/posts/2274-kak-ispoljhzovatjh-bigdecimal-v-java)

продолжение
Наше число не изменилось, как и следовало ожидать. Чтобы операция сложения прошла успешно, необходимо создать новый объект и присвоить ему результат сложения.