### 一、单选择题(每小题2分，共10分)
1、编译Java Application 源程序文件将产生相应的字节码文件，这些字节码文件的扩展名为(   B   )。

         A.    .java                      B.    .class
         C.    .html                      D.    .exe

2、设 x = 1 , y = 2 , z = 3，则表达式 y＋＝z－－/＋＋x 的值是( A    )。

         A.    3                        B.    3. 5
         C.    4                        D.    5

3、在Java Applet程序用户自定义的Applet子类中，一般需要重载父类的(   D   )方法来完成一些画图操作。

    A.   start( )                    B.   stop( )
    C.   init( )                     D.   paint( )

4、不允许作为类及类成员的访问控制符的是(   C   )。
    A.   public                    B.   private
    C.   static                     D.   protected

5、为AB类的一个无形式参数无返回值的方法method书写方法头，使得使用类名AB作为前缀就可以调用它，该方法头的形式为(    A )。

    A. static void method( )                    B. public void method( )    
    C. final void method( )                      D. abstract void method( )

###二、填空题（每空格1分，共20分）
1、开发与运行Java程序需要经过的三个主要步骤为________、_________ 和 __________。

2、如果一个Java Applet源程序文件只定义有一个类，该类的类名为MyApplet，则类MyApplet必须是___________类的子类并且存储该源程序文件的文件名为             _______。

3、如果一个Java Applet程序文件中定义有3个类，则使用Sun公司的JDK编译
器__________编译该源程序文件将产生__________个文件名与类名相同而扩展名为        __________的字节码文件。

4、在Java的基本数据类型中，char型采用Unicode编码方案，每个Unicode码占
用__________字节内存空间，这样，无论是中文字符还是英文字符，都是占
用__________字节内存空间。

5、设 x = 2 ，则表达式 ( x + + )／3 的值是_________。

6、若x = 5，y = 10，则x < y和x >= y的逻辑值分别为 _______ 和 _______。

7、__________方法是一种仅有方法头，没有具体方法体和操作实现的方法，该方法必须在抽象类之中定义。___________方法是不能被当前类的子类重新定义的方法。

8、创建一个名为 MyPackage 的包的语句是____________，该语句应该放在程序的位置为：_____________。

9、设有数组定义：`int   MyIntArray[ ] = { 10 , 20 , 30 , 40 , 50 , 60 , 70}`;   则执行以下几个语句后的输出结果是____________。

``` java
   int s = 0 ;
   for ( int i = 0 ; i < MyIntArray.length ; i + + )
                 if ( i % 2 = = 1 )    s += MyIntArray[i] ;
   System.out.println( s );
```
10、在Java程序中，通过类的定义只能实现______重继承，但通过接口的定义可以实现_______重继承关系。

###三、写出下列程序完成的功能。(每小题5分，共20分)
1、
```
public class   Sum
{ public static void   main( String args[ ])
   {  double   sum = 0.0 ;
       for ( int i = 1 ; i <= 100 ; i + + )
           sum += 1.0/(double) i ;
      System.out.println( "sum="+sum );
   }
}
```
<br><br><br><br><br><br><br>
2、 
```
import java.io.* ;
    public class Reverse
    {   public static void   main(String args[ ])
        {   int   i , n =10 ;
            int a[ ] = new int[10];
            for ( i = 0 ; i < n ; i ++ )
            try {
                 BufferedReader br = new BufferedReader(
                         new InputStreamReader(System.in));
                 a[i] = Integer.parseInt(br.readLine( )); // 输入一个整数
            } catch ( IOException e ) { } ;
            for ( i = n－1 ; i >= 0 ; i ―― )
                System.out.print(a[i]+" ");
        System.out.println( );
        }
   }
```
<br><br><br><br><br><br><br>
3、 
```
import     java.awt.*;
    public    class    abc
    { public   static   void    main(String args[])
          {      new FrameOut();       }
    }
    class   FrameOut   extends    Frame     // Frame为系统定
     {   Button btn;                                        // 义的窗框类
         FrameOut( )
         {       super("按钮");
                 btn = new Button("按下我");
                 setLayout(new   FlowLayout( ));
                 add(btn);
                 setSize(300,200);
                 show( );
          }
      }
```
<br><br><br><br><br><br><br>
4、
```
import    java.io.*;
   public    class   abc
   {   public   static   void   main(String args[])
         {   SubClass    sb = new   SubClass( );        
             System.out.println(sb.max( ));
         }
     }
    class    SuperClass
   {   int a = 10 , b = 20 ; }
   class SubClass extends SuperClass
   {   int max( ) { return   ((a>b)?a:b); } }
```
<br><br><br><br><br><br><br>

### 四、写出下面程序的运行结果(每小题10分，共30分)
1、 
``` java
import java.io.*;
public class abc
{         public static void main(String args[ ])
          {    AB s = new AB("Hello!","I love JAVA.");
               System.out.println(s.toString( ));
          }
}
class   AB {
String   s1;
String   s2;
AB( String str1 , String str2 )
{ s1 = str1; s2 = str2; }
public   String   toString( )
{ return s1+s2;}
}
```
<br><br><br><br><br><br><br>
2、 
```
import    java.io.* ;
    public   class abc
    {
          public   static   void    main(String args[ ])
          {    int   i , s = 0 ;
               int a[ ] = { 10 , 20 , 30 , 40 , 50 , 60 , 70 , 80 , 90 };
               for ( i = 0 ; i < a.length ; i ++ )
                     if ( a[i]%3 = = 0 ) s += a[i] ; 
               System.out.println("s="+s);
           }
     }
```
<br><br><br><br><br><br><br>
3、
```
import   java.io.* ;
   public class abc
   {
         public static void   main(String args[ ])
　 )
        { System.out.println("a="+a+"\nb="+b); }
    }
    class   SubClass   extends   SuperClass
    { int c;
       SubClass(int aa,int bb,int cc)
       {   super(aa,bb);
           c=cc;
       }
    }
   class   SubSubClass   extends   SubClass
   {   int a;
       SubSubClass(int aa,int bb,int cc)
       {   super(aa,bb,cc);
           a=aa+bb+cc;
        }
       void show()
        { System.out.println("a="+a+"\nb="+b+"\nc="+c); }
}
```
<br><br><br><br><br><br><br>
### 五、使用Java语言编写程序。(每小题10分，共20分)
1、编写一个字符界面的Java Application 程序，接受用户输入的10个整数，并输出这10个整数的最大值和最小值。
<br><br><br><br><br><br><br>
2、编写一个完整的Java Applet 程序使用复数类Complex验证两个复数 1+2i 和3+4i 相加产生一个新的复数 4+6i 。
     复数类Complex必须满足如下要求：
(1) 复数类Complex 的属性有：
RealPart :    int型，代表复数的实数部分
ImaginPart : int型，代表复数的虚数部分
(2) 复数类Complex 的方法有：
Complex( ) : 构造函数，将复数的实部和虚部都置0
Complex( int r , int i ) : 构造函数，形参 r 为实部的初值，i为虚部的初值。
Complex complexAdd(Complex a) : 将当前复数对象与形参复数对象相加，所得的结果仍是一个复数值，返回给此方法的调用者。
String ToString( ) : 把当前复数对象的实部、虚部组合成 a+bi 的字符串形式，其中a 和 b分别为实部和虚部的数据。
<br><br><br><br><br><br><br>

##《JAVA语言程序设计》期末考试模拟试题 参考答案及评分标准
                                                                                                          
### 一、单选择题(每小题2分，共10分)
1、B     2、A     3、D     4、C     5、A
### 二、填空题（每空格1分，共20分）
1、编辑源程序、编译生成字节码、解释运行字节码
2、Applet、MyApplet
3、javac.exe、3、 . class
4、2 、2
5、0
6、true 、 false
7、抽象(abstract)方法、最终(final)方法
8、package   MyPackage ;     应该在程序第一句。
9、120
10、单、多
### 三、写出下列程序完成的功能。(每小题5分，共20分)
1、计算 1/1+1/2+1/3+...+1/100 的值。
2、从标准输入(即键盘)读入10个整数存入整型数组a中，然后逆序输出这10个整数。
3、创建一个标题为"按钮"的窗框，窗框中显示有"按下我"字样的按钮。
4、求两个数的最大值。
### 四、写出下面程序的运行结果(每小题10分，共30分)
1、Hello! I love JAVA.
2、s = 180
3、a=60
     b=20
     c=30
### 五、使用Java语言编写程序。(每小题10分，共20分)
1、参考程序如下：
```
import   java.io.* ; 
public   class   abc 
{
   public static void   main(String args[ ]) 
   { int   i , n = 10 , max = 0 , min = 0 , temp = 0;
          try { 
                BufferedReader br = new BufferedReader(
                            new InputStreamReader(System.in));
                max = min = Integer.parseInt(br.readLine( )); 
         } catch ( IOException e ) { } ;
      for ( i = 2 ; i <= n ; i ++ ) {
          try { 
                BufferedReader br = new BufferedReader(
                            new InputStreamReader(System.in));
                temp = Integer.parseInt(br.readLine( )); 
         if (temp > max ) max=temp;
         if (temp < min) min=temp;
         } catch ( IOException e ) { } ;
    }
      System.out.println("max="+max+"\nmin="+min); 
   }
}
```
2、参考程序如下：
```
import java.applet.* ;      
import java.awt.* ;
public class abc extends Applet    
{
   Complex a,b,c ;
   public void init( )    
   {
     a = new Complex(1,2);   
     b = new Complex(3,4);   
     c = new Complex();     
   }
   public void paint(Graphics g)    
   {
     c=a.complexAdd(b);
     g.drawString("第一个复数："+a.toString(),10,50);
     g.drawString("第二个复数："+b.toString(),10,70);
     g.drawString("两复数之和："+c.toString(),10,90);
   }
}
    
class Complex
{
    int RealPart ;    // 复数的实部     
    int ImaginPart ; // 复数的虚部
    Complex() { RealPart = 0 ; ImaginPart = 0 ; } 
    Complex(int r , int i)    
    { RealPart = r ;    ImaginPart = i ;   }
    Complex complexAdd(Complex a)
    {
         Complex temp = new Complex( ); // 临时复数对象
         temp.RealPart=RealPart+a.RealPart;
         temp.ImaginPart=ImaginPart+a.ImaginPart;
         return temp;
    }
    public String toString( )         
    {   return ( RealPart+" + "+ImaginPart+" i ");   }
}
```
