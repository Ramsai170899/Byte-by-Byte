## **Unit 5: Data Representation and Processing**

### **Understanding Binary and Number Systems**

Data representation in computers relies on various number systems to encode and process information efficiently. The most common systems used in computing are:

1. **Binary (Base-2)**
2. **Decimal (Base-10)**
3. **Hexadecimal (Base-16)**
4. **Octal (Base-8)**

---

### **Binary, Decimal, Hexadecimal, and Octal Systems**

#### **1. Binary Number System (Base-2)**
- Consists of only two digits: **0** and **1**.
- Used in computers because digital circuits operate using electrical signals (ON = 1, OFF = 0).
- Each digit in a binary number is called a **bit**.
- Example: \( 1011_2 \) (Binary) = \( 1×2^3 + 0×2^2 + 1×2^1 + 1×2^0 = 8 + 0 + 2 + 1 = 11_{10} \) (Decimal).

#### **2. Decimal Number System (Base-10)**
- The number system we use in daily life, consisting of digits from **0 to 9**.
- Each position represents powers of 10.
- Example: \( 352_{10} \) = \( 3×10^2 + 5×10^1 + 2×10^0 \).

#### **3. Hexadecimal Number System (Base-16)**
- Uses 16 symbols: **0-9** and **A-F**, where:
  - \( A = 10 \), \( B = 11 \), \( C = 12 \), \( D = 13 \), \( E = 14 \), \( F = 15 \).
- Commonly used in computing for memory addresses and colors in web development.
- Example: \( 2F_{16} \) = \( 2×16^1 + 15×16^0 = 32 + 15 = 47_{10} \).

#### **4. Octal Number System (Base-8)**
- Uses digits **0 to 7**.
- Often used in computing as a shorthand for binary numbers (groups of three bits).
- Example: \( 75_8 \) = \( 7×8^1 + 5×8^0 = 56 + 5 = 61_{10} \).

---

### **Conversion Between Number Systems**

1. **Binary to Decimal**  
   Multiply each bit by \( 2^n \) (where \( n \) is the position from right, starting at 0) and sum the results.  
   Example: \( 1101_2 \) → \( 1×2^3 + 1×2^2 + 0×2^1 + 1×2^0 = 8+4+0+1 = 13_{10} \).

2. **Decimal to Binary**  
   - Divide the decimal number by 2.
   - Write down the remainder.
   - Repeat until the quotient is 0.
   - Read the remainder from bottom to top.
   Example: \( 13_{10} \) → \( 1101_2 \).

3. **Binary to Hexadecimal**  
   - Group bits into sets of 4 from the right.
   - Convert each 4-bit group into a hexadecimal digit.
   Example: \( 11011011_2 \) → \( 1101 \) (D) and \( 1011 \) (B) → \( DB_{16} \).

4. **Binary to Octal**  
   - Group bits into sets of 3 from the right.
   - Convert each group to an octal digit.
   Example: \( 101110_2 \) → \( 101 \) (5) and \( 110 \) (6) → \( 56_8 \).

---

### **Data Representation in Computers**

Computers store and process different types of data, such as characters, images, sounds, and videos, in **binary format**.

#### **1. Representation of Characters (ASCII & Unicode)**
- **ASCII (American Standard Code for Information Interchange)**  
  - Uses **7 or 8 bits** to represent characters (letters, numbers, symbols).  
  - Example: 'A' = **65 (01000001 in binary)**.
  
- **Unicode**  
  - Extends ASCII to support multiple languages and symbols.
  - Uses **16-bit or 32-bit encoding**.
  - Example: 'अ' (Devanagari) = **U+0905**.

#### **2. Image Representation**
- Images are stored as **pixels**, each having a specific **color code**.
- **Grayscale images** store intensity values (0 to 255 for 8-bit images).
- **Colored images** use RGB (Red, Green, Blue) values.
- Example: A 24-bit image uses 8 bits per color channel (RGB), allowing **16.7 million colors**.

#### **3. Sound Representation**
- **Analog sound** is sampled and stored as digital data.
- **Bit depth** (e.g., 16-bit, 24-bit) determines sound quality.
- **Sampling rate** (e.g., 44.1 kHz) defines how often sound is recorded per second.

#### **4. Video Representation**
- Videos are sequences of images (frames per second).
- Common formats include **MP4, AVI, MOV**.
- Higher frame rates (e.g., 60fps) produce smoother motion.

---

### **Boolean Logic and Digital Circuits**

Boolean logic is the foundation of digital computing, using **true (1) and false (0)** values.

#### **Logic Gates**
Logic gates perform basic logical operations on binary inputs:

1. **AND Gate**  
   - Output is 1 only if both inputs are 1.  
   - Truth Table:  
     | A | B | Output |
     |---|---|--------|
     | 0 | 0 |   0    |
     | 0 | 1 |   0    |
     | 1 | 0 |   0    |
     | 1 | 1 |   1    |

2. **OR Gate**  
   - Output is 1 if **at least one input** is 1.  

3. **NOT Gate**  
   - Inverts the input (0 → 1, 1 → 0).  

4. **NAND Gate** (NOT + AND)  
   - Output is 0 only if both inputs are 1.

5. **NOR Gate** (NOT + OR)  
   - Output is 1 only if both inputs are 0.

6. **XOR Gate (Exclusive OR)**  
   - Output is 1 if **only one input** is 1.

7. **XNOR Gate (Exclusive NOR)**  
   - Output is 1 if inputs are **the same**.

---

### **Boolean Algebra**
Boolean algebra simplifies logical expressions using:
- **Laws of Boolean Algebra**:
  - **Identity Law**: \( A + 0 = A \), \( A \times 1 = A \)
  - **Null Law**: \( A + 1 = 1 \), \( A \times 0 = 0 \)
  - **Idempotent Law**: \( A + A = A \), \( A \times A = A \)
  - **Complement Law**: \( A + A' = 1 \), \( A \times A' = 0 \)
  - **De Morgan’s Theorems**:
    - \( (A.B)' = A' + B' \)
    - \( (A + B)' = A' . B' \)

These laws are used in **circuit simplification**, reducing the number of logic gates in a circuit.

---

### **Conclusion**
Understanding data representation and Boolean logic is crucial in computing. Number systems enable efficient storage and processing, while Boolean logic forms the basis of digital circuits. These concepts help in computer programming, electronics, and digital design.
