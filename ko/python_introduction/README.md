# Introduction to Python

>이 챕터의 일부는 Geek Girls Carrots (http://django.carrots.pl/) 튜토리얼을 근간으로 하고 있어요.

자 이제 코드를 작성해볼까요 ^^

## Python prompt
파이썬과 놀기 위해서, 우리는 여러분의 컴퓨터의 *command line* 을 열어야 해요.

 -- 이미 어떻게 하는 지 알고 계셔야 합니다.[Command Line 소개 챕터](../intro_to_command_line/README.md)에서 이미 배우셨으니까요.

준비가 되셨으면 아래의 설명대로 따라해보세요.

파이썬 콘솔을 열기 원합니다. 그래서 우리는 python3라고 타이핑할꺼에요.

    $ python3
    Python 3.4.2 (...)
    Type "copyright", "credits" or "license" for more information.
    >>>

## 두둥! 당신의 첫번째 파이썬 명령어

파이썬3라고 입력한 후에는 프롬프트가 '>>>'로 바뀔꺼에요. 그건 우리가 이제 파이썬언어에 해당하는 명령만을 사용할 수 있다는 걸 의미해요.
그렇다고 '>>>'를 직접 입력하실 필요는 없어요. - 파이썬이 여러분을 위해서 대신 할 겁니다.
어느때던지 파이썬 콘솔에서 빠져나가고 싶으면, 그냥  `exit()` 를 입력하거나 윈도우의 경우에는 단축키 `Ctrl + Z` 그리고 맥/리눅스의 경우에는  `Ctrl + D` 를 입력하면  더 이상  `>>>` 가 나타나지 않을 거에요.
그렇지만 지금은 파이썬 콘솔 밖으로 나갈 필요가 없습니다. 우리는 더 배우길 원하니까요. 약간 단순한 걸 시작해볼까요
예를 들어, 덧셈같은거요. '2+3' 을 입력하고 엔터를 치세요.
    >>> 2 + 3
    5

멋져욧! 답이 어떻게 출력되었는지 봤나요? 파이썬이 수학을 알다니! 다른 비슷한 것들도 해보죠:
- `4 * 5`
- `5 - 1`
- `40 / 2`

방금 실습한 몇 가지 예제들이 즐거우셨길 바래요. 자 그리고 다시 원래 문맥으로 돌아와서 ^^;
방금 보셨듯이, 파이썬은 엄청난 계산기에요.  음 아직도 못 믿으시겠다면 무엇이든지 더 해보세요.
## Strings

이름이 어떻게 되세요?  쌍따옴표로 이름을 감싸고 입력해보세요:

    >>> "Ola"
    'Ola'

방금 당신은 첫번째 문자열을 만드셨습니다.문자열은 컴퓨터가 처리할 수 있는 문자의 집합같은 거에요. 문자열은 반드시 처음 그리고 끝이 같은 문자로 끝나야합니다. 그래서 ' 홑따옴표 또는 " 쌍따옴표는 파이썬에게 그 내부에 문자열이 있음을 알려줘요.


문자열끼리는 서로 연결할 수 있어요 예문처럼 해보세요:

    >>> "Hi there " + "Ola"
    'Hi there Ola'

또한 아래와 같이 문자열 곱하기를 이용해 반복해서 나타낼 수 있어요:

    >>> "Ola" * 3
    'OlaOlaOla'

만약에 문자열안에 아스트로피(')를 사용하고 싶은 경우에는, 두가지 방법을 사용할 수 있어요.

더블쿼터(")를 사용하기:
    >>> "Runnin' down the hill"
    "Runnin' down the hill"

또는 백슬러시('\')와 함께 사용해서 표시할 수 있습니다.

    >>> 'Runnin\' down the hill'
    "Runnin' down the hill"

좋아요, 그쵸? 당신의 이름을 대문자로 표현하려면 아래와 같이 하면 됩니다:

    >>> "Ola".upper()
    'OLA'

그저 'upper' __function__ 을 문자열에 사용하면 되요! ('upper()')와 같은 함수는 파이썬에서 호출할 때 문자열을 받아서 동작합니다.
만약 이름의 전체 길이가  몇 글자로 되어 있는지 알고 싶은 경우에도 함수를 사용하면 됩니다.
    >>> len("Ola")
    3

왜 함수를 호출할 때 ('"ola".upper()')처럼 문자열의 마지막에  '.' 를 붙여서 사용하는지 그리고 문자열을 삽입해서 사용하는 지 의문이 생길 수 있습니다. 음. 그건 각각의 상황에 따라서 조금 다른데요.  ('"Ola".upper()') 처럼 사용할 때는 함수가 "Ola"라는 스트링오브젝트에 속하게 되어 동작합니다. upper()는 문자열에만 동작가능한 함수에요. 그런데 아무런 오브젝트에 속하지 않은 채로 __method__ 로서 함수를 호출할 때가 있죠. 'len()' 처럼요.  그래서 이 경우에는 len 함수에 '"Ola"'라는 인자를 받아서 사용합니다.

### 요약

좋습니다. 문자열에 대해서는 충분히 학습한 것 같네요. 
OK, enough of strings. So far you've learned about:

- __the prompt__ - typing commands (code) into the Python prompt results in answers in Python
- __numbers and strings__ - in Python numbers are used for math and strings for text objects
- __operators__ - like + and *, combine values to produce a new one
- __functions__ - like upper() and len(), perform actions on objects.

These are the basics of every programming language you learn. Ready for something harder? We bet you are!

## Errors

Let's try something new. Can we get the length of a number the same way we could find out the length of our name? Type in `len(304023)` and hit Enter:

    >>> len(304023)
    Traceback (most recent call last):
      File "<stdin>", line 1, in <module>
    TypeError: object of type 'int' has no len()

We got our first error! It says that objects of type "int" (integers, whole numbers) have no length. So what can we do now? Maybe we can write our number as a string? Strings have a length, right?

    >>> len(str(304023))
    6

It worked! We used the `str` function inside of the `len` function. `str()` converts everything to strings.

- The `str` function converts things into __strings__
- The `int` function converts things into __integers__

> Important: we can convert numbers into text, but we can't necessarily convert text into numbers - what would `int('hello')` be anyway?

## Variables

An important concept in programming is variables. A variable is nothing more than a name for something so you can use it later. Programmers use these variables to store data, make their code more readable and so they don't have to keep remembering what things are.

Let's say we want to create a new variable called `name`:

    >>> name = "Ola"

You see? It's easy! It's simply: name equals Ola.

As you've noticed, your program didn't return anything like it did before. So how do we know that the variable actually exists? Simply enter `name` and hit Enter:

    >>> name
    'Ola'

Yippee! Your first variable :)! You can always change what it refers to:

    >>> name = "Sonja"
    >>> name
    'Sonja'

You can use it in functions too:

    >>> len(name)
    5

Awesome, right? Of course, variables can be anything, so numbers too! Try this:

    >>> a = 4
    >>> b = 6
    >>> a * b
    24

But what if we used the wrong name? Can you guess what would happen? Let's try!

    >>> name = "Maria"
    >>> names
    Traceback (most recent call last):
      File "<stdin>", line 1, in <module>
    NameError: name 'names' is not defined

An error! As you can see, Python has different types of errors and this one is called a **NameError**. Python will give you this error if you try to use a variable that hasn't been defined yet. If you encounter this error later, check your code to see if you've mistyped any names.

Play with this for a while and see what you can do!


## The print function

Try this:

    >>> name = 'Maria'
    >>> name
    'Maria'
    >>> print(name)
    Maria

When you just type `name`, the Python interpreter responds with the string *representation* of the variable 'name', which is the letters M-a-r-i-a, surrounded by single quotes, ''.  When you say `print(name)`, Python will "print" the contents of the variable to the screen, without the quotes, which is neater.

As we'll see later, `print()` is also useful when we want to print things from inside functions, or when we want to print things on multiple lines.


## Lists

Beside strings and integers, Python has all sorts of different types of objects. Now we're going to introduce one called __list__. Lists are exactly what you think they are: they are objects which are lists of other objects :)

Go ahead and create a list:

    >>> []
    []

Yes, this list is empty. Not very useful, right? Let's create a list of lottery numbers. We don't want to repeat ourselves all the time, so we will put it in a variable, too:

    >>> lottery = [3, 42, 12, 19, 30, 59]

All right, we have a list! What can we do with it? Let's see how many lottery numbers there are in a list. Do you have any idea which function you should use for that? You know this already!

    >>> len(lottery)
    6

Yes! `len()` can give you a number of objects in a list. Handy, right? Maybe we will sort it now:

    >>> lottery.sort()

This doesn't return anything, it just changed the order in which the numbers appear in the list. Let's print it out again and see what happened:

    >>> print(lottery)
    [3, 12, 19, 30, 42, 59]

As you can see, the numbers in your list are now sorted from the lowest to highest value. Congrats!

Maybe we want to reverse that order? Let's do that!

    >>> lottery.reverse()
    >>> print(lottery)
    [59, 42, 30, 19, 12, 3]

Easy, right? If you want to add something to your list, you can do this by typing this command:

    >>> lottery.append(199)
    >>> print(lottery)
    [59, 42, 30, 19, 12, 3, 199]

If you want to show only the first number, you can do this by using __indexes__. An index is the number that says where in a list an item occurs. Computer people like to start counting at 0, so the first object in your list is at index 0, the next one is at 1, and so on. Try this:

    >>> print(lottery[0])
    59
    >>> print(lottery[1])
    42

As you can see, you can access different objects in your list by using the list's name and the object's index inside of square brackets.

For extra fun, try some other indexes: 6, 7, 1000, -1, -6 or -1000. See if you can predict the result before trying the command. Do the results make sense?

You can find a list of all available list methods in this chapter of the Python documentation: https://docs.python.org/3/tutorial/datastructures.html

## Dictionaries

A dictionary is similar to a list, but you access values by looking up a key instead of an index. A key can be any string or number. The syntax to define an empty dictionary is:

    >>> {}
    {}

This shows that you just created an empty dictionary. Hurray!

Now, try writing the following command (try replacing your own information too):

    >>> participant = {'name': 'Ola', 'country': 'Poland', 'favorite_numbers': [7, 42, 92]}

With this command, you just created a variable named `participant` with three key-value pairs:

- The key `name` points to the value `'Ola'` (a `string` object),
- `country` points to `'Poland'` (another `string`),
- and `favorite_numbers` points to `[7, 42, 92]` (a `list` with three numbers in it).

You can check the content of individual keys with this syntax:

    >>> print(participant['name'])
    Ola

See, it's similar to a list. But you don't need to remember the index - just the name.

What happens if we ask Python the value of a key that doesn't exist? Can you guess? Let's try it and see!

    >>> participant['age']
    Traceback (most recent call last):
      File "<stdin>", line 1, in <module>
    KeyError: 'age'

Look, another error! This one is a **KeyError**. Python is helpful and tells you that the key `'age'` doesn't exist in this dictionary.

When to use a dictionary or a list? Well, that's a good point to ponder on. Just have a solution in mind before looking at the answer in the next line.

- Do you just need an ordered sequence of items? Go for a list.
- Do you need to associate values with keys, so you can look them up efficiently (by key) later on? Use a dictionary.

Dictionaries, like lists, are *mutable*, meaning that they can be changed after they are created. You can add new key/value pairs to the dictionary after it is created, like:

    >>> participant['favorite_language'] = 'Python'

Like lists, using `len()` method on the dictionaries, returns the number of key-value pairs in the dictionary. Go ahead and type in the command:

    >>> len(participant)
    4

I hope it makes sense up to now. :) Ready for some more fun with dictionaries? Hop onto the next line for some amazing things.

You can use the `del` command to delete an item in the dictionary. Say, if you want to delete the entry corresponding to the key `'favorite_numbers'`, just type in the following command:

    >>> del participant['favorite_numbers']
    >>> participant
    {'country': 'Poland', 'favorite_language': 'Python', 'name': 'Ola'}

As you can see from the output, the key-value pair corresponding to  the 'favorite_numbers' key has been deleted.

As well as this, you can also change a value associated with an already created key in the dictionary. Type:

    >>> participant['country'] = 'Germany'
    >>> participant
    {'country': 'Germany', 'favorite_language': 'Python', 'name': 'Ola'}

As you can see, the value of the key `'country'` has been altered from `'Poland'` to `'Germany'`. :) Exciting? Hurrah! You just learnt another amazing thing.

### Summary

Awesome! You know a lot about programming now. In this last part you learned about:

- __errors__ - you now know how to read and understand errors that show up if Python doesn't understand a command you've given it
- __variables__ - names for objects that allow you to code more easily and to make your code more readable
- __lists__ - lists of objects stored in a particular order
- __dictionaries__ - objects stored as key-value pairs

Excited for the next part? :)

## Compare things

A big part of programming includes comparing things. What's the easiest thing to compare? Numbers, of course. Let's see how that works:

    >>> 5 > 2
    True
    >>> 3 < 1
    False
    >>> 5 > 2 * 2
    True
    >>> 1 == 1
    True
    >>> 5 != 2
    True

We gave Python some numbers to compare. As you can see, Python can compare not only numbers, but it can also compare method results. Nice, huh?

Do you wonder why we put two equal signs `==` next to each other to compare if numbers are equal? We use a single `=` for assigning values to variables. You always, __always__ need to put two `==` if you want to check if things are equal to each other. We can also state that things are unequal to each other. For that, we use the symbol `!=`, as shown in the example above.

Give Python two more tasks:

    >>> 6 >= 12 / 2
    True
    >>> 3 <= 2
    False

`>` and `<` are easy, but what do `>=` and `<=` mean? Read them like this:

- x `>` y means: x is greater than y
- x `<` y means: x is smaller than y
- x `<=` y means: x is smaller or equal to y
- x `>=` y means: x is greater or equal to y

Awesome! Wanna do one more? Try this:

    >>> 6 > 2 and 2 < 3
    True
    >>> 3 > 2 and 2 < 1
    False
    >>> 3 > 2 or 2 < 1
    True

You can give Python as many numbers to compare as you want, and it will give you an answer! Pretty smart, right?

- __and__ - if you use the `and` operator, both comparisons have to be True in order for the whole command to be True
- __or__ - if you use the `or` operator, only one of the comparisons has to be True in order for the whole command to be True

Have you heard of the expression "comparing apples to oranges"? Let's try the Python equivalent:

    >>> 1 > 'django'
    Traceback (most recent call last):
      File "<stdin>", line 1, in <module>
    TypeError: unorderable types: int() > str()

Here you see that just like in the expression, Python is not able to compare a number (`int`) and a string (`str`).
Instead, it shows a **TypeError** and tells us the two types can't be compared together.

## Boolean

Incidentally, you just learned about a new type of object in Python. It's called a __Boolean__ -- and it probably is the easiest type there is.

There are only two Boolean objects:
- True
- False

But for Python to understand this, you need to always write it as True (first letter uppercased, with the rest of the letter lowercased). __true, TRUE, tRUE won't work -- only True is correct.__ (The same applies to False as well, of course.)

Booleans can be variables, too! See here:

    >>> a = True
    >>> a
    True

You can also do it this way:

    >>> a = 2 > 5
    >>> a
    False

Practice and have fun with Booleans by trying to run the following commands:

- `True and True`
- `False and True`
- `True or 1 == 1`
- `1 != 2`

Congrats! Booleans are one of the coolest features in programming, and you just learned how to use them!

# Save it!

So far we've been writing all our python code in the intepreter, which limits us to one line of code at a time. Normal programs are saved in files and executed by our programming language __interpreter__ or __compilier__. So far we've been running our programs one line at a time in the Python __interpreter__. We're going to need more than one line of code for the next few tasks, so we'll quickly need to:

- Exit the Python interpreter
- Open up our code editor of choice
- Save some code into a new python file
- Run it!

To exit from the Python interpreter that we've been using, simply type the ```exit()``` function:

    >>>exit()
    $

This will put you back into the command prompt.

Earlier, we picked out a code editor from the [code editor](../code_editor/README.md) section. We'll need to open the editor now and write some code into a new file:

    print('Hello, Django girls!')

Obviously, you're a pretty seasoned python developer now, so feel free to write some code that you've learned today.

Now we need to save the file and give it a descriptive name. Let's call the file **python_intro.py** and save it to your desktop. We can name the file anything we want, the important part here is to make sure the file ends in __.py__, this tells our computer that this is a **python executable file** and Python can run it.

With the file saved, it's time to run it! Using the skills you've learned in the command line section, use the terminal to **change directories** to the desktop.

On a Mac, the command will look something like this:

    cd /Users/<your_name>/Desktop

On Linux, it will be like this (the word "Desktop" might be translated to your language):

    cd /home/<your_name>/Desktop

And on windows, it will be like this:

    cd C:\Users\<your_name>\Desktop

If you get stuck, just ask for help.

and then use Python to execute the code in the file like this:

    $ python3 python_intro.py
    Hello, Django girls!

Alright! You just ran your first python program that was saved to a file. Feel awesome?

You can now move on to an essential tool in programming:

## If...elif...else

Lots of things in code should only be executed when given conditions are met. That's why Python has something called __if statements__.

Replace the code in your **python_intro.py** file to this:

    if 3 > 2:

If we saved this and ran it, we'd see an error like this:

    $ python3 python_intro.py
    File "python_intro.py", line 2
             ^
    SyntaxError: unexpected EOF while parsing

Python expects us to give further instructions to it which are supposed to be executed if the condition `3 > 2` turns out to be true (or `True` for that matter). Let’s try to make Python print “It works!”. Change your code in your **python_intro.py** file to this:

    if 3 > 2:
        print('It works!')

Notice how we've indented the next line of code by 4 spaces? We need to do this so Python knows what code to run if the code results in true. You can do one space, but nearly all Python programmers do 4 to make things look neat. A single tab will also count as 4 spaces.

Save it and give it another run:

    $ python3 python_intro.py
    It works!

### What if not?

In previous examples, code was executed only when the conditions were True. But Python also has `elif` and `else` statements:

    if 5 > 2:
        print('5 is indeed greater than 2')
    else:
        print('5 is not greater than 2')

When this was run it would print out:

    $ python3 python_intro.py
    5 is indeed greater than 2

If 2 were a greater number than 5, then the second command would be executed. Easy, right? Let's see how `elif` works:

    name = 'Sonja'
    if name == 'Ola':
        print('Hey Ola!')
    elif name == 'Sonja':
        print('Hey Sonja!')
    else:
        print('Hey anonymous!')

and executed:

    $ python3 python_intro.py
    Hey Sonja!

See what happened there?

### Summary

In the last three exercises you learned about:

- __comparing things__ - in Python you can compare things by using `>`, `>=`, `==`, `<=`, `<` and the `and`, `or` operators
- __Boolean__ - a type of object that can only have one of two values: `True` or `False`
- __Saving files__ - storing code in files so you can execute larger programs.
- __if...elif...else__ - statements that allow you to execute code only when certain conditions are met.

Time for the last part of this chapter!

## Your own functions!

Remember functions like `len()` that you can execute in Python? Well, good news, you will learn how to write your own functions now!

A function is a set of instructions that Python should execute. Each function in Python starts with the keyword `def`, is given a name and can have some parameters. Let's start with an easy one. Replace the code in **python_intro.py** with the following:

    def hi():
        print('Hi there!')
        print('How are you?')

    hi()

Okay, our first function is ready!

You may wonder why we've written the name of the function at the bottom of the file. This is because Python reads the file and executes it from top to bottom. So in order to use our function, we have to re-write it at the bottom.

Let's run this now and see what happens:

    $ python3 python_intro.py
    Hi there!
    How are you?

That was easy! Let's build our first function with parameters. We will use the previous example - a function that says 'hi' to the person running it - with a name:

    def hi(name):

As you can see, we now gave our function a parameter that we called `name`:

    def hi(name):
        if name == 'Ola':
            print('Hi Ola!')
        elif name == 'Sonja':
            print('Hi Sonja!')
        else:
            print('Hi anonymous!')

    hi()

As you can see, we needed to put two indents before the `print` function, because `if` needs to know what should happen when the condition is met. Let's see how it works now:

    $ python3 python_intro.py
    Traceback (most recent call last):
    File "python_intro.py", line 10, in <module>
      hi()
    TypeError: hi() missing 1 required positional argument: 'name'

Oops, an error. Luckily, Python gives us a pretty useful error message.
It tells us that the function `hi()` (the one we defined) has one required argument (called `name`) and that we forgot to pass it when calling the function.
Let's fix it at the bottom of the file:

    hi("Ola")

and run it again:

    $ python3 python_intro.py
    Hi Ola!

And if we change the name?

    hi("Sonja")

and run it:

    $ python3 python_intro.py
    Hi Sonja!

Now what do you think will happen if you write another name in there? (Not Ola or Sonja) Give it a try and see if you're right. It should print out this:

    Hi anonymous!

This is awesome, right? This way you don't have to repeat yourself every time you want to change the name of the person the function is supposed to greet. And that's exactly why we need functions - you never want to repeat your code!

Let's do something smarter -- there are more names than two, and writing a condition for each would be hard, right?

    def hi(name):
        print('Hi ' + name + '!')

    hi("Rachel")

Let's call the code now:

    $ python3 python_intro.py
    Hi Rachel!

Congratulations! You just learned how to write functions :)!

## Loops

That's the last part already. That was quick, right? :)

As we mentioned, programmers are lazy, they don't like to repeat themselves. Programming is all about automating things, so we don't want to greet every person by their name manually, right? That's where loops come in handy.

Still remember lists? Let's do a list of girls:

    girls = ['Rachel', 'Monica', 'Phoebe', 'Ola', 'You']

We want to greet all of them by their name. We have the `hi` function to do that, so let's use it in a loop:

    for name in girls:

The ```for``` statement behaves similarly to the ```if``` statement, code below both of these need to be indented four spaces.

Here is the full code that will be in the file:

    def hi(name):
        print('Hi ' + name + '!')

    girls = ['Rachel', 'Monica', 'Phoebe', 'Ola', 'You']
    for name in girls:
        hi(name)
        print('Next girl')

and when we run it:

    $ python3 python_intro.py
    Hi Rachel!
    Next girl
    Hi Monica!
    Next girl
    Hi Phoebe!
    Next girl
    Hi Ola!
    Next girl
    Hi You!
    Next girl

As you can see, everything you put inside a `for` statement with an indent will be repeated for every element of the list `girls`.

You can also use `for` on numbers using the `range` function:

    for i in range(1, 6):
        print(i)

Which would print:

    1
    2
    3
    4
    5

`range` is a function that creates a list of numbers following one after the other (these numbers are provided by you as parameters).

Note that the second of these two numbers is not included in the list that is output by Python (meaning `range(1, 6)` counts from 1 to 5, but does not include the number 6).

## Summary

That's it. __You totally rock!__ This really wasn't so easy, so you should feel proud of yourself. We're definitely proud of you for making it to here!

You might want to briefly do something else - stretch, walk around for a bit, rest your eyes - before going on to the next chapter. :)

![Cupcake](images/cupcake.png)
