# LoopsIntro
67. Loops Intro

67. Giới thiệu vòng lặp

Trong C#, các vòng lặp được sử dụng để thực thi lặp đi lặp lại một khối mã cho đến khi một điều kiện cụ thể được đáp ứng. Có ba loại vòng lặp trong C#: vòng lặp `for`, vòng lặp `while` và vòng lặp `do-while`.

1. `for` Loop:
Vòng lặp `for` được sử dụng khi bạn biết trước số lần lặp. Nó bao gồm ba phần: khởi tạo, điều kiện và tăng/giảm. Vòng lặp sẽ tiếp tục thực thi khối mã miễn là điều kiện còn đúng.

Cú pháp:
```csharp
for (initialization; condition; increment / decrement)
{
    // Code to be executed in each iteration
}
```
Ví dụ:
```csharp
for (int i = 1; i <= 5; i++)
{
    Console.WriteLine("Iteration: " + i);
}
```
2. `while` Loop:
Vòng lặp `while` được sử dụng khi bạn muốn lặp lại việc thực thi một khối mã miễn là một điều kiện là đúng. Nó kiểm tra điều kiện trước mỗi lần lặp.

Cú pháp:
```csharp
while (condition)
{
    // Code to be executed in each iteration
}
```
Ví dụ:
```csharp
int i = 1;
while (i <= 5)
{
    Console.WriteLine("Iteration: " + i);
    i++;
}
```
3. Vòng lặp `do-while`:
Vòng lặp `do-while` tương tự như vòng lặp `while`, nhưng nó kiểm tra điều kiện sau khi thực thi khối mã. Điều này có nghĩa là khối mã sẽ luôn được thực thi ít nhất một lần.

Cú pháp:
```csharp
do
{
    // Code to be executed in each iteration
} while (condition) ;
```
Ví dụ:
```csharp
int i = 1;
do
{
    Console.WriteLine("Iteration: " + i);
    i++;
} while (i <= 5);
```
Vòng lặp cung cấp một cách hiệu quả để tự động hóa các tác vụ lặp đi lặp lại và lặp lại các tập hợp dữ liệu trong C#. Chúng giúp làm cho mã ngắn gọn và hiệu quả hơn.

69. For Loops

Vòng lặp `for` được sử dụng để lặp lại một khối mã trong một số lần cụ thể. Nó đặc biệt hữu ích khi bạn biết trước số lần bạn muốn vòng lặp chạy. Vòng lặp bao gồm ba thành phần:

1. Khởi tạo(Initialization): Phần này được thực hiện một lần trước khi vòng lặp bắt đầu. Nó thường liên quan đến việc khởi tạo một biến đếm.

2. Điều kiện(Condition): Phần này là biểu thức Boolean được đánh giá trước mỗi lần lặp. Nếu điều kiện là `true`, thì vòng lặp tiếp tục; mặt khác, vòng lặp kết thúc.

3. Lặp lại(Iteration): Phần này được thực hiện sau mỗi lần lặp và thường cập nhật biến đếm.

Cú pháp của vòng lặp `for`:

```csharp
for (initialization; condition; iteration)
{
    // Code to be executed in each iteration
}
```
Đây là cách hoạt động của vòng lặp `for`:

1. Câu lệnh `khởi tạo` được thực thi trước, khởi tạo biến đếm.
2. Tiếp theo, `điều kiện` được đánh giá. Nếu điều kiện là `true`, thân vòng lặp được thực thi. Nếu nó là `false`, thì vòng lặp kết thúc và chương trình tiếp tục với mã theo sau vòng lặp.
3. Sau mỗi lần lặp của thân vòng lặp, câu lệnh `iteration` được thực thi, cập nhật biến đếm.
4. Sau đó, vòng lặp quay lại bước `điều kiện` và lặp lại quy trình cho đến khi điều kiện trở thành `sai`.

Ví dụ: In các số từ 1 đến 5 bằng vòng lặp `for`:

```csharp
for (int i = 1; i <= 5; i++)
{
    Console.WriteLine(i);
}
```

Output:
```
1
2
3
4
5
Vòng lặp `for` rất linh hoạt và có thể được sử dụng cho nhiều tình huống, bao gồm việc lặp qua mảng, tập hợp hoặc thực hiện các tác vụ cụ thể với số lần cố định. Đó là một cấu trúc cơ bản trong lập trình C# và là một công cụ cần thiết để kiểm soát luồng thực thi.

My code: 
using Microsoft.VisualBasic;
using System;

namespace LoopsIntro
{
    internal class Program
    {
        static void Main(string[] args)
        {
            for (int counter = 1; counter < 20; counter+=2)
            {
                Console.WriteLine(counter + " is lower than 20");
            }
            Console.WriteLine("For loop is done");
            Console.Read();            
        }
    }
}



70. Do While Loops

Vòng lặp `do-while` trong C# là một loại vòng lặp khác cho phép bạn lặp lại một khối mã miễn là một điều kiện nhất định là đúng. Sự khác biệt chính giữa vòng lặp `do-while` và vòng lặp `while` là vòng lặp `do-while` đảm bảo rằng thân vòng lặp sẽ được thực thi ít nhất một lần, ngay cả khi điều kiện ban đầu là sai.

Cú pháp của vòng lặp `do-while` như sau:

```csharp
do
{
    // Code to be executed in each iteration
} while (condition) ;
```
Đây là cách hoạt động của vòng lặp `do-while`:

1. Mã bên trong thân vòng lặp được thực thi trước.
2. Sau đó, `điều kiện` được đánh giá. Nếu điều kiện là `true`, thân vòng lặp sẽ được thực thi lại và quá trình lặp lại.
3. Nếu điều kiện là `false`, thì vòng lặp kết thúc và chương trình tiếp tục với đoạn mã sau vòng lặp.

Ví dụ: In các số từ 1 đến 5 bằng vòng lặp `do-while`:

```csharp
int i = 1;
do
{
    Console.WriteLine(i);
    i++;
} while (i <= 5);
```

Output:
```
1
2
3
4
5
```
Trong ví dụ này, mặc dù điều kiện `i <= 5` là đúng cho lần lặp đầu tiên, thân vòng lặp được thực hiện ít nhất một lần vì đó là vòng lặp `do-while`.

Vòng lặp `do-while` hữu ích khi bạn cần thực thi một đoạn mã ít nhất một lần trước khi kiểm tra điều kiện. Nó đặc biệt hữu ích khi bạn muốn lặp lại một thao tác phụ thuộc vào đầu vào của người dùng hoặc khi bạn cần thực hiện khởi tạo trước khi kiểm tra điều kiện vòng lặp. Chỉ cần đảm bảo rằng vòng lặp cuối cùng sẽ kết thúc, nếu không bạn có nguy cơ bị mắc kẹt trong một vòng lặp vô hạn.

My code: 
using System;

namespace DoWhileLoops
{
    internal class Program
    {
        static void Main(string[] args)
        {
            int lengthOfText = 0;
            string wholeText = "";

            do
            {
                Console.WriteLine("Please enter the name of a friend");
                string nameOfAFriend = Console.ReadLine();
                int currentLength = nameOfAFriend.Length;
                lengthOfText += currentLength;
                wholeText += nameOfAFriend;
            } while (lengthOfText < 20);

            Console.WriteLine("Thanks, that was enough!" + wholeText);

            Console.Read();
        }
    }
}

71. While Loops
71. Vòng lặp While
Trong C#, vòng lặp `while` được sử dụng để thực thi lặp lại một khối mã miễn là một điều kiện cụ thể là đúng. Vòng lặp tiếp tục thực thi khối mã cho đến khi điều kiện trở thành sai. Cú pháp chung của vòng lặp `while` như sau:

```csharp
while (condition)
{
    // Code to be executed repeatedly
}
```
Đây là một ví dụ về việc sử dụng vòng lặp `while` để in các số từ 1 đến 5:

```csharp
using System;

namespace WhileLoopsExample
{
    class Program
    {
        static void Main(string[] args)
        {
            int count = 1;

            while (count <= 5)
            {
                Console.WriteLine(count);
                count++; // Increment the count by 1 in each iteration
            }
        }
    }
}
```

Output:
```
1
2
3
4
5
```
Giải trình:
1. Trong ví dụ trên, chúng ta khai báo một biến `count` và khởi tạo nó là 1.
2. Vòng lặp `while` bắt đầu bằng từ khóa `while`, theo sau là điều kiện `count <= 5`.
3. Thân vòng lặp thực thi miễn là điều kiện `count <= 5` là đúng.
4. Bên trong vòng lặp, chúng ta in giá trị của `count` bằng cách sử dụng `Console.WriteLine(count)`.
5. Sau đó, chúng tôi tăng giá trị của `count` lên 1 trong mỗi lần lặp bằng cách sử dụng `count++`.
6. Vòng lặp tiếp tục thực hiện cho đến khi điều kiện `count <= 5` trở thành sai, tức là khi `count` trở thành 6.

Hãy nhớ rằng nếu điều kiện ban đầu là sai, vòng lặp sẽ không bao giờ thực hiện hoặc nếu điều kiện luôn đúng, nó sẽ dẫn đến một vòng lặp vô tận. Điều cần thiết là bao gồm mã bên trong vòng lặp mà cuối cùng sẽ thay đổi điều kiện thành sai để tránh vòng lặp vô hạn.

My code:
using System;

namespace WhileLoops
{
    internal class Program
    {
        static void Main(string[] args)
        {
            int counter = 0;
            string enteredText = "";
            while (enteredText.Equals(""))
            {
                Console.WriteLine("Please press enter to increase amount by one and anything else" +
                    " + enter if you want to finish counting");
                enteredText = Console.ReadLine();

                counter++;
                Console.WriteLine("Current people count is {0}", counter);
            }
            Console.WriteLine("{0} people are inside the bus. Press enter to close the program", counter);
            Console.Read();
        }
    }
}

Coding Exercise 4: Loops

Today your task is to practice the use of loops. There are two methods you have to fill:

in the ForLoop method you have to  print on a new line each value from -3 to 3 included using the for loop;

in the WhileLoop method you need to print values from 3 to -3 using the while loop;

solution in my code:
using System;

namespace Coding.Exercise
{
    public class Exercise
    {
        public static void ForLoop()
        {
            for (int counter = -3; counter < 4; counter++)
            {
                Console.WriteLine(counter);
            }
        }

        public static void WhileLoop()
        {
            int i = 3;
            while (i > -4)
            {
                Console.WriteLine(i--);
            }
        }

        public static void Run()
        {
            WhileLoop();
            ForLoop();

        }

    }
}

72. break and continue

Trong C#, `break` và `continue` là các câu lệnh luồng điều khiển được sử dụng trong các vòng lặp để thay đổi luồng thực thi.

1. ` break `:
    - Câu lệnh `break` được sử dụng để thoát khỏi vòng lặp (for, while hoặc do-while) trước thời hạn dựa trên một điều kiện nhất định.
    - Khi gặp câu lệnh `break` bên trong một vòng lặp, vòng lặp đó ngay lập tức kết thúc và điều khiển di chuyển đến câu lệnh theo sau vòng lặp.
    - Nó thường được sử dụng khi bạn muốn thoát khỏi một vòng lặp sớm nếu một điều kiện cụ thể được đáp ứng.

Ví dụ:
```csharp
for (int i = 1; i <= 10; i++)
{
    if (i == 5)
        break; // Exit the loop when i becomes 5
    Console.WriteLine(i);
}
```
Output:
```
1
2
3
4
```
2. ` continue `:
    - Câu lệnh ` continue ` được sử dụng để bỏ qua phần còn lại của vòng lặp hiện tại và chuyển sang bước lặp tiếp theo của vòng lặp.
    - Khi gặp câu lệnh ` continue ` bên trong một vòng lặp, nó sẽ bỏ qua mã còn lại trong thân vòng lặp và chuyển sang bước lặp tiếp theo, bắt đầu lại vòng lặp.
    - Nó thường được sử dụng khi bạn muốn bỏ qua các bước lặp cụ thể dựa trên các điều kiện nhất định.

Ví dụ:
```csharp
for (int i = 1; i <= 10; i++)
{
    if (i % 2 == 0)
        continue; // Skip even numbers and move to the next iteration
    Console.WriteLine(i);
}
```
Output:
```
1
3
5
7
9
```
Tóm lại, `break` được sử dụng để thoát khỏi vòng lặp sớm, trong khi `continue` được sử dụng để bỏ qua phần còn lại của bước lặp hiện tại và chuyển sang bước lặp tiếp theo trong vòng lặp.

My code: 
using System;

namespace breakandcontinue
{
    internal class Program
    {
        static void Main(string[] args)
        {
            for (int counter = 0; counter < 10; counter++)
            {
                if (counter % 2 == 0)
                {
                    Console.WriteLine("Now comes an odd number!");
                    continue;
                }
                Console.WriteLine(counter);
            }
            Console.Read();
        }
    }
}

Coding Exercise 5: break and continue practice

break and continue practice
Implement conditions for the given while loop.

To pass the tests, your loop should skip all divisible by 3 values and stops running when i = 10.

Warning: You cannot touch the given parts of the code! You can add your conditions only inside the loop!

Warning2: This while loop is an infinite loop! To avoid it causing you issues we implemented the current if statement that you can find. This, with the proper solution in place, should not be needed anymore. Before running the tests, find a way to stop it without reaching the pre-placed break!

Solution in my code: 
using System;

namespace Coding.Exercise
{
    public class Exercise
    {
        public static void Run()
        {
            int i = -10;

            while (true)
            {

                if (i % 3 == 0)
                {
                    i++;
                    continue;
                }
                if (i == 10)
                {
                    break;
                }
                if (i == 11)
                {
                    Console.WriteLine(" FINAL BREAK REACHED! This should not happen!");
                    break;
                }
                Console.WriteLine(i++);
            }
        }
    }
}

73. Challenge - Loops 1 – Average

Challenge - Loops 1 - Average
Imagine you are a developer and get a job in which you need to create a program for a teacher. He needs a program written in c# that calculates the average score of his students. So he wants to be able to enter each score individually and then get the final average score once he enters -1.
So the tool should check if the entry is a number and should add that to the sum. Finally once he is done entering scores, the program should write onto the console what the average score is.
The numbers entered should only be between 0 and 20. Make sure the program doesn't crash if the teacher enters an incorrect value.
Test your program thoroughly.

Solution in my code:
using System;

namespace AverageCalculator
{
    class Program
    {
        static void Main(string[] args)
        {
            string input = "0";
            int count = 0;
            int total = 0;
            int currentNumber = 0;
            while (input != "-1")
            {
                Console.WriteLine("Last number was {0}", currentNumber);
                Console.WriteLine("Please enter the next score");
                Console.WriteLine("Current amount of entries {0}", count);
                Console.WriteLine("Please enter -1 once you are ready to caculate the average");
                
                input = Console.ReadLine();
                if (input.Equals("-1"))
                {
                    Console.WriteLine("---------------------------------------");
                    // Calculate average and let the teacher know
                    double average = (double)total / (double)count;
                    Console.WriteLine("The average score of your student is {0}", average);
                }
                if (int.TryParse(input, out currentNumber) && currentNumber > 0 && currentNumber < 21)
                {
                    total += currentNumber;
                }
                else
                {
                    if (!(input.Equals("-1")))
                    {
                        Console.WriteLine("Please enter a value between 1 and 20!");
                    }
                    continue;
                }

                count++;
            }

            Console.ReadLine();
        }
    }
}
