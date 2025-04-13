# 🔢 Java ke Commonly Used Data Types (Primitive Types)

Java mein kuch commonly used basic data types hote hain, jinhe primitive types bhi kaha jata hai. Ye data types directly ek value ko store karte hain.

| **Type**                                | **Matlab Kya Store Karta Hai**                               |
|---------------------------------------------|---------------------------------------------------------------|
| `boolean` | Sab jagah se access kiya ja sakta hai |
| `char` | 16-bit Unicode character (ek letter jaise 'A', 'B', etc.) |
| `byte` | 8-bit signed integer (chhoti value: -128 se 127) |
| `short` | 16-bit signed integer (bigger than byte) |
| `int` | 32-bit signed integer (default integer type) |
| `long` | 64-bit signed integer (bohot badi value) |
| `float` | 32-bit decimal number (point wale numbers ke liye) |
| `double` | 64-bit decimal number (float se zyada accurate) |

---

## 🧠 Important Notes:

- Agar tum likhte ho `int x = 14;` toh by default ye `int` mana jaata hai.

- Agar tum likhte ho `long y = 195L;` toh `L` ya `l` lagana zaroori hai taaki Java ko pata chale ye `long` hai.

- Decimal numbers jaise `3.1416` by default `double` hote hain.

    - Agar tumhe `float` chahiye toh likhna padega `3.1416F` ya `3.1416f`.

## 💡 Code Example (Declaration + Initialization)

```
public class DataTypes {

    public static void main(String[] args) {
        
        boolean flag = true;                 // ek boolean variable
        char grade = 'A';                    // ek character variable
        byte b = 12;                         // byte type variable
        short s = 24;                        // short type variable
        int k = 257;                   // teen int, sirf k initialized hai
        long l = 890L;                       // long ke liye L lagaya
        float pi = 3.1416F;                  // float ke liye F lagaya
        double e = 2.71828, a = 6.022e23;    // do double type variables

        System.out.println("Boolean flag: " + flag);
        System.out.println("Character grade: " + grade);
        System.out.println("Byte b: " + b);
        System.out.println("Short s: " + s);
        System.out.println("Integer k: " + k);
        System.out.println("Long l: " + l);
        System.out.println("Float pi: " + pi);
        System.out.println("Double e: " + e);
        System.out.println("Double a: " + a);

    }

    
}
```

---

## 📤 **Output**

```
Boolean flag: true
Character grade: A
Byte b: 12
Short s: 24
Integer k: 257
Long l: 890
Float pi: 3.1416
Double e: 2.71828
Double a: 6.022E23
```

---

## 🤔 Aur Bhi Kuch Important Baatein:

* Ek hi line mein multiple variables declare aur initialize kiye ja sakte hain, jaise line 2, 6, aur 9 mein hua hai.

* Local variables (jo kisi method ya block ke andar bane hote hain) unhe use karne se pehle initialize karna zaroori hota hai. Warna error milega.

* Agar tum class ke andar variables declare karte ho (instance variables), aur unhe initialize nahi karte ho, toh Java default values de deta hai:

    * Numbers → `0`

    * `boolean` → `false`

    * `char` → null character (`\u0000`)
