<div align="center">

## Learning C/C\+\+ Part II: IF statements and variables


</div>

### Description

Hello, this is Alexander. Since I finally got an email from someone who liked my previous lesson, I am going to make the second installment. This one will be about variables, and stuff like 'if' statements.
 
### More Info
 


<span>             |<span>
---                |---
**Submitted On**   |
**By**             |[Alexander of CProgramming\.com](https://github.com/Planet-Source-Code/PSCIndex/blob/master/ByAuthor/alexander-of-cprogramming-com.md)
**Level**          |Beginner
**User Rating**    |4.4 (22 globes from 5 users)
**Compatibility**  |C\+\+ \(general\)
**Category**       |[Miscellaneous](https://github.com/Planet-Source-Code/PSCIndex/blob/master/ByCategory/miscellaneous__3-1.md)
**World**          |[C / C\+\+](https://github.com/Planet-Source-Code/PSCIndex/blob/master/ByWorld/c-c.md)
**Archive File**   |[](https://github.com/Planet-Source-Code/alexander-of-cprogramming-com-learning-c-c-part-ii-if-statements-and-variables__3-442/archive/master.zip)





### Source Code

<table border="0" width="100%">
 <tbody>
  <tr>
   <td width="100%"><font size="2" face="verdana,arial">
    <p><font face="Verdana">'IF' is the most important word in programming
    for many programs. Without it there is no conditional statements. This
    means that there can be only one way a program can execute. It would
    almost impossible to make a program without this one simple word.</font></p>
    <p><font face="Verdana">&nbsp;&nbsp;&nbsp;&nbsp; There are many things
    to understand when using IF statements. First, you must understand stuff
    like OR NOT etc. This are the most important, so I will describe how to
    use them in C and C++ programming below: (NOTE: ZERO IS FALSE! ONE IS
    TRUE!)</font></p>
    <p><font face="Verdana">NOT: This just says that the program should
    reverse the value...for example NOT(1) would be 0. NOT(0) would be 1.
    NOT(any number but zero) would be 0. In C and C++ NOT is written as - !
    - just one simple little character. It is very useful and can save lots
    of time.</font></p>
    <p><font face="Verdana">AND: This is another important command, and it
    is used to say that if this AND this is true... for example (1)AND(0)
    would come out as 0. (1)AND(1) would come out as 1. (ANY REAL NUMBER BUT
    ZERO)AND(0) would be 0. (ANY REAL NUMBER BUT ZERO)AND(ANY REAL NUMBER
    BUT ZERO) would be 1. The AND is written as - &amp;&amp; - in C++. It is
    just two simple characters.</font></p>
    <p><font face="Verdana">OR: Very useful is the OR statement! For example
    (1)OR(0) would be 1! (0)OR(0) would be 0. (ANY REAL NUMBER)OR(ANY REAL
    NUMBER BUT ZERO) would be 1! It is simple, either one can be true and
    make the whole thing true. The OR is written as - || - in C++. It is
    also two simple characters.</font></p>
    <p><font face="Verdana">&nbsp;&nbsp;&nbsp;&nbsp; The next thing to learn
    is to combine them... What is !(1 &amp;&amp; 0)? Of course, it would be
    1. This is because 1 &amp;&amp; 0 evaluates two 0 and ! 0 equals 1.</font></p>
    <p><font face="Verdana">&nbsp;&nbsp;&nbsp;&nbsp; Try some of
    these...they are not hard. If you have questions about them, you can
    email me at lallain@concentric.net.</font></p>
    <p><font face="Verdana">A. !(1 || 0) ANSWER: 0</font></p>
    <p><font face="Verdana">B. !(1 || 1 &amp;&amp; 0) ANSWER: 0 (AND is
    evaluated before OR)</font></p>
    <p><font face="Verdana">C. !((1 || 0) &amp;&amp; 0) ANSWER: 1
    (Parenthesis are useful)</font></p>
    <p><font face="Verdana">&nbsp;&nbsp;&nbsp;&nbsp; If you find you enjoy
    this you might want to look more at Boolean Algebra, which is also very
    helpful to programmers as it can be good for helping program conditional
    statements.</font></p>
    <p><font face="Verdana">IF is used like this IF(TRUE)</font></p>
    <p><font face="Verdana">{ DO WHAT IS IN THE BRACKETS }</font></p>
    <p><font face="Verdana">ELSE is basically ELSE</font></p>
    <p><font face="Verdana">{ DO WHAT IS IN THE BRACKETS }</font></p>
    <p><font face="Verdana">Let's look at a simple program for you to try
    out on your own...</font></p>
    <p><font face="Verdana">#include &lt;iostream.h&gt; //For output</font></p>
    <p><font face="Verdana">#include &lt;conio.h&gt; //For getch()</font></p>
    <p><font face="Verdana">void main() //Most important part of the
    program!</font></p>
    <p><font face="Verdana">{</font></p>
    <p><font face="Verdana">int age; //Need a variable...</font></p>
    <p>&nbsp;</p>
    <p><font face="Verdana">cout&lt;&lt;&quot;Please input your age: &quot;;
    //Asks for age</font></p>
    <p><font face="Verdana">cin&gt;&gt;age; //The input is put in age</font></p>
    <p>&nbsp;</p>
    <p><font face="Verdana">if(age&lt;100) //If the age is less than 100</font></p>
    <p><font face="Verdana">{</font></p>
    <p><font face="Verdana">cout&lt;&lt;&quot;You are pretty young!&quot;;
    //Just to show you the output</font></p>
    <p><font face="Verdana">}</font></p>
    <p><font face="Verdana">if(age==100) //Remember, if the age equals 100
    needs two =</font></p>
    <p><font face="Verdana">{</font></p>
    <p><font face="Verdana">cout&lt;&lt;&quot;You are old&quot;; //Just to
    show you it works...</font></p>
    <p><font face="Verdana">}</font></p>
    <p><font face="Verdana">if(age&gt;100)</font></p>
    <p><font face="Verdana">{</font></p>
    <p><font face="Verdana">cout&lt;&lt;&quot;You are really old&quot;;
    //Proof that it works for all conditions</font></p>
    <p><font face="Verdana">}</font></p>
    <p><font face="Verdana">}</font></p>
    <p><font face="Verdana">&nbsp;&nbsp;&nbsp;&nbsp; Now, this program did
    not use &amp;&amp; || ! or anything in it. This is because it didn't
    need too. I think you should probably be able to make your own if
    statements with them without&nbsp;having to worry too much about
    problems.</font></p>
    </font></td>
  </tr>
 </tbody>
</table>

