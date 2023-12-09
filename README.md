# Negative Binary Numbers
## Created by Erin Shawhan
![Binary numbers](digitization-5194814_1280.jpg)
### Overview
This is a tutorial on representing **negative numbers** in binary intended for beginners wanting to learn more about binary and digital information. The **binary number system** is a base-2 number system, meaning that it only uses two symbols, 0 and 1. In binary, single digits are referred to as **"bits"**. In the number system we use everyday, the base-10 **decimal system** (symbols 0-9), we can represent negative numbers by putting a negative sign in front of the number. However, in binary, we can only use 0s and 1s to represent negative numbers. In this tutorial, I will cover **3 ways** to represent negative numbers in binary: *sign magnitude*, *1's complement*, and *2's complement*.

### Sign Magnitude
With sign magnitude, one of the bits (typically the far left bit - known as the most significant bit) is designated to indicate if a number in positive or negative. Since a specific bit will be designated as the sign indicator, we must specify the number of bits we will be using to represent a to not change a significant bit. **A zero is usually used to represent a positive number, whereas a 1 is used to represent a negative number.** Although sign magnitude can be used to represent negative binary numbers, it is rarely used in the real world because it is not practical to perform math operations on them.

#### Example:
Let's look at an example of using sign magnitude to represent a negative binary number. The number 5 in binary (represented in 8 bits) is 00000101. In this case, to represent the number -5, we would change the leftmost bit to a 1. This would make -5 in binary 10000101.

### 1's Complement
With 1's complement, **the bits of a binary number are inverted to represent the negative of the binary number**. So, if a bit in the positive number is a 1, then we would turn it into a zero and vice versa to represent the positive number.

#### Example:
Here's an example of how to use 1's complement to represent a negative binary number. The number 8 in binary (using 8 bits) is 00001000. In order to represent -8, we change each bit into the opposite bit. This makes -8 in binary 11110111.

### 2's Complement
In order to represent a negative binary number with 2's complement, **the leftmost bit becomes the negative of the value it would normally represent**. In order to find the value of a positive binary number in decimal you can multiply the value of the bit, 0 or 1, (starting with the rightmost bit) by 2 to the power of the place of the digit (starting at 0). You then add each product together to get the decimal value. In the case of 2's complement, when we multiply the leftmost digit by 2^n, we instead multiply the negative value of the digit. So, if the value was 1 it would become -1 and if the value was 0 it would become -0. As with the previous two methods, it important to distinguish the number of bits being used to represent the number, as it will change the value. 2's complement can be quite useful because, unlike the other two methods, we are able to perform arithmetic on 2's complement negative numbers.

#### Example:
Let's look at an example to see how 2's complement is calculated. So, for example, to find the decimal value of the binary number 1010, we would solve the following equations 0x2^0=0, 1x2^1=2, 0x2^3=0, and 1x2^4=8. We would then add each value, 0+2+0+8=10. After multiplying and adding all of the values we get 10, so the binary number 1010 represents the decimal number 10. However, if we were to look at the binary number 1010 in 2's complement, it would become a different value. Instead of the leftmost digit representing 1, it would now represent -1. The values of each digit would become 0, 2, 0, and -8 (-1x2^3), and after adding each value together, we would get -6. So, the binary number 1010 with 2's complement is the decimal number -6.

### Conclusion
Although representing negative numbers in binary can be confusing and very different from in decimal, it is possible and can be a good tool when working with digital information! Through different methods, such as sign magnitude, 1's complement, and 2's complement, we can learn various ways of representing negative binary numbers. I hope that this tutorial helped you learn more about negative numbers in binary and feel more comfortable working with negative binary numbers in the future!
