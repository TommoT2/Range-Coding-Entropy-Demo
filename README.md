# Range-Coding-Entropy-Demo

📊 Range Coding & Entropy: High-Precision Data Compression Demo

A pure client-side JavaScript demonstration of Range Coding (a form of Arithmetic Coding), designed to illustrate how lossless data compression can achieve the theoretical limits defined by information entropy.

This project is an excellent educational tool for students and developers interested in Information Theory, advanced Lossless Compression techniques, and the underlying principles of bit-efficient encoding often utilized by modern Large Language Models (LLMs).

✨ Key Features

Entropy Calculation: Automatically calculates the theoretical Shannon Entropy (minimum required bits per symbol) of the input data.

Near-Perfect Compression: Demonstrates how Range Coding encodes an entire input string into a single, high-precision fractional number, achieving compression ratios extremely close to the calculated entropy limit.

Lossless Verification: Includes full encoding and decoding logic to verify that the original data is reconstructed without loss, highlighting the importance of the method.

High-Precision Aritmetic (Crucial): Leverages the Big.js library to handle the extreme decimal precision (120 decimal places) required to perform the recursive interval calculation losslessly. This illustrates a critical technical challenge in implementing Range Coding.

Educational Context: Directly ties the compression technique to the concept of removing coding redundancy, a core component of academic courses on digital representation and data compression.

🚀 Getting Started

This project is a single, self-contained HTML file and requires no build steps or server environment.

Clone the Repository:

git clone [https://github.com/YourUsername/YourRepoName.git](https://github.com/YourUsername/YourRepoName.git)


Open the File:
Simply open the index.html file in any modern web browser.

Use GitHub Pages:
The project is perfectly suited for hosting via GitHub Pages for immediate public access.

🧠 Why Range Coding? (Context for LLMs and Theory)

Unlike Huffman Coding, which is restricted to using a whole number of bits per symbol (e.g., 2 or 3 bits), Range Coding allows the use of fractional bits (e.g., 1.63 bits per symbol).

This efficiency aligns with the workings of Generative AI models (LLMs), which operate on a probability distribution:

High Probability → Low Information Content → Requires Fewer Bits (Smaller interval size).

Low Probability → High Information Content → Requires More Bits (Larger interval size for precision).

Range Coding provides a tangible mathematical model for how data redundancy can be mathematically exploited to minimize the data representation size.
