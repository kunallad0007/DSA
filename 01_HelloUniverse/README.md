# Introduction
Data structures aur algorithms banane ke liye humein computer ko detailed instructions deni padti hain. Aise communication ka ek accha tareeka hai ek high-level programming language ka use karna — jaise ki Java. Is chapter mein, hum Java programming language ka ek overview denge. Agle chapter mein hum object-oriented design principles pe focus karenge.

Hum yeh maan kar chal rahe hain ki readers ko kisi na kisi high-level programming language ka basic idea hai, lekin Java zaruri nahi hai. Yeh book Java language ka full description nahi degi (kyunki uske liye already bahut references available hain), lekin is book mein jitni Java ki zarurat padhegi, wo sab cheezein yahan introduce ki jaayengi.

---

## 🔸 “Hello Universe!” Program Se Shuruaat

Java primer (introduction) hum ek simple program se shuru karte hain jo screen par "Hello Universe!" print karta hai. Yeh program Figure 1.1 mein diya gaya hai, aur uska breakdown bhi diya gaya hai.

Java mein jo bhi executable statements hoti hain, wo functions (Java mein unhe methods bola jaata hai) ke andar likhi jaati hain. Har method kisi class ka part hota hai.

Hamari pehli example mein Universe naam ki ek class hai. Ye class bahut simple hai — ismein sirf ek hi method hai:
```
public static void main(String[] args)
```
Yeh method static hai aur iska naam main hai — Java program run hone ke baad sabse pehle isi method ko execute kiya jaata hai.

Jo bhi statements curly braces {} ke andar likhe hote hain, unhe ek block bola jaata hai. Poori Universe class ek block hai, aur usmein likha main method bhi ek block ke andar hai.

-----------------------------------------------------------------------

## 🔸 Java ke Identifiers

Java mein jab hum kisi class, method, ya variable ka naam dete hain, to use identifier bola jaata hai. Identifier kuch bhi ho sakta hai — bas shart yeh hai ki:

Wo ek letter (a-z ya A-Z) se start hona chahiye,

Aur usmein letters, numbers, aur underscore _ use kiya ja sakta hai.

Java Unicode support karta hai, isliye aap kisi bhi language ke characters use kar sakte ho (jaise Hindi, Chinese etc.).

Lekin, kuch exceptions bhi hain — jaise Java ke reserved words (if, class, for, etc.), jinko hum variable ya class names ke roop mein use nahi kar sakte. In exceptions ki list Table 1.1 mein di gayi hai.

-----------------------------------------------------------------------

### ✅ Java Code: HelloUniverse.java
```
public class Universe {
    public static void main(String[] args) {
        System.out.println("Hello Universe!");
    }
}
```
---
### 🧠 Hinglish Explanation with Comments:

```
// Java program ka naam hai Universe
public class Universe {

    // yeh hai main method — Java program yahin se start hota hai
    public static void main(String[] args) {

        // yeh line output console par "Hello Universe!" print karegi
        System.out.println("Hello Universe!");
    }
}
```

---

### 🔍 Line-by-line Breakdown:

| **Line**                                | **Explanation**                                                                 |
|-----------------------------------------|---------------------------------------------------------------------------------------------|
| `public class Universe`                 | Yahan hum ek class define kar rahe hain jiska naam hai Universe. Java mein sab kuch class ke andar hota hai. |
| `public static void main(String[] args)`| main method Java program ka entry point hota hai. Jab program run hota hai, sabse pehle yahi method call hota hai. |
| `System.out.println("Hello Universe!");`| Ye line console (output screen) par "Hello Universe!" print karwa deti hai.               |
| `{ }`                                   | Curly braces ek block define karte hain — jo statements unke beech likhe jaate hain, wo ek unit ki tarah execute hote hain. |

---
### 🎓 Some Extra Concepts:

| **Keywords**                                | **Explanation**                               |
|---------------------------------------------|---------------------------------------------------------------|
| `public`                 | Sab jagah se access kiya ja sakta hai |
| `static`| Object banaye bina method ko call kar sakte hain|
| `void`| Is method ka koi return value nahi hai |
| `String[] args	` |Command line arguments ko store karne ke liye hota hai|
