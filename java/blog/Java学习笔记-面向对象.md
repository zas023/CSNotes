### һ Java�����������췽����
>java�еĹ��췽����һ���������͵ķ��������ڳ�ʼ������Java���캯���ڶ��󴴽�ʱ�����á� ������ֵ�����ṩ��������ݣ�����Ϊʲô������Ϊ���캯����

    ����java���캯���Ĺ���:

- ���캯�����Ʊ���������������ͬ
- ���캯������û����ʽ��������

>���������͵Ĺ��캯����

    1. Ĭ�Ϲ��캯��(�޲������캯��)
    2. ���������캯��

#### 1. Ĭ�Ϲ��캯��(�޲������캯��)

``` Java
//û�в����Ĺ��캯����ΪĬ�Ϲ��캯����Ĭ�Ϲ��캯�����﷨���£�
<class_name>(){}

//Ĭ�Ϲ��캯����ʾ����
class Bike {
    Bike() {
        System.out.println("Bike is created");
    }

    public static void main(String args[]) {
        Bike b = new Bike();
    }
}

//�����ʾ���������н������ -
Bike is created
```

    ����
    1. �������û�й��캯�������������Զ�����һ��Ĭ�Ϲ��캯����
    2. Ĭ�Ϲ��캯����������Ϊ�����ṩĬ��ֵ���磺0��null�ȡ� 
    3. ���캯�����ص�ǰ���ʵ��(����ָ������ֵ���ͣ������᷵��һ��ֵ)��

#### 2. ���캯���ͷ���֮�������

|���캯��|Java����|
 :-: | -: |
���������ڳ�ʼ�������״̬(����)��|	�������ڱ�¶�������Ϊ��
���캯�������з������͡�|	����һ�㶼�з������͡�
���캯����ʽ���á�|	����Ҫ��ʽ���á�
���û��ָ���κι��캯����java�������ṩһ��Ĭ�Ϲ��캯����|	���κ�����±������������ṩĬ�ϵķ������á�
���캯�����Ʊ�������������ͬ��|	�������ƿ��Ի���Բ�����������ͬ(����)��

### �� Java �̳�
>�̳���java��������̼�����һ���ʯ����Ϊ���������ֵȼ���ε��ࡣ�̳п������Ϊһ���������һ�������ȡ���ԵĹ��̡�

    Java�еļ̳���һ�ֻ��ƣ���ʾΪһ�������ȡ��������������Ժ���Ϊ��

- ��Java�м̳��ǣ����Դ������������๹���µ��ࡣ ������������̳�ʱ���Ϳ����ظ�ʹ�ø���ķ������ֶΣ�Ҳ�����ڼ̳е�����������µķ������ֶΡ�

- �̳б�ʾIS-A��ϵ��Ҳ��Ϊ���ӹ�ϵ����˵:һ����������һ�������һ�����ࡣ

---
    �����A����B�ĸ��࣬����B����C�ĸ��࣬����Ҳ��C��A�����࣬��C�Ǵ���A�̳ж����ġ���Java�У���ļ̳��ǵ�һ�̳У�Ҳ����˵��һ������ֻ��ӵ��һ������

    �̳����ʹ�õ������ؼ�����extends��implements��

    �������ؼ��ֵ�ʹ�þ�����һ���������һ�������Ƿ���IS-A(��һ��)��ϵ��

    ͨ��ʹ���������ؼ��֣�������ʵ��һ�������ȡ��һ����������ԡ�

    ����Java���������java.lang.Object��̳ж����ģ�����Object��������������࣬������Object�⣬�����������һ�����ࡣ

#### 1. Ϊʲô��java��ʹ�ü̳У�
    ���ڷ�������(��˿���ʵ������ʱ�Ķ�̬��)����ߴ���������ԡ���Java�У�����ɼ̳и����еķ�����������Ҫ���±�д��ͬ�ķ���������ʱ���ಢ����ԭ�ⲻ���ؼ̳и���ķ�������������һ�����޸ģ������Ҫ���÷�������д(����)��

#### 2. �̳е��﷨

```
class Subclass-name extends Superclass-name  
{  
   //methods and fields  
}
```

    extends�ؼ��ֱ�ʾ���ڴ��������������������ࡣ ��extends���ĺ��������ӹ��ܡ���Java�������У��̳е����Ϊ������࣬�����Ϊ�ӻ����ࡣ

#### 3. java�̳�����

##### 3.1. ��һ�̳�ʾ��

``` Java
class Animal {
    void eat() {
        System.out.println("eating...");
    }
}

class Dog extends Animal {
    void bark() {
        System.out.println("barking...");
    }
}

class TestInheritance {
    public static void main(String args[]) {
        Dog d = new Dog();
        d.bark();
        d.eat();
    }
}

//ִ���������õ����½�� 

barking...
eating...
```

##### 3.2 �༶�̳�ʾ��
``` Java
class Animal {
    void eat() {
        System.out.println("eating...");
    }
}

class Dog extends Animal {
    void bark() {
        System.out.println("barking...");
    }
}

class BabyDog extends Dog {
    void weep() {
        System.out.println("weeping...");
    }
}

class TestInheritance2 {
    public static void main(String args[]) {
        BabyDog d = new BabyDog();
        d.weep();
        d.bark();
        d.eat();
    }
}

//ִ���������õ����½�� -

weeping...
barking...
eating...
```

##### 3.3 �༶�̳�ʾ��

``` Java
class Animal {
    void eat() {
        System.out.println("eating...");
    }
}

class Dog extends Animal {
    void bark() {
        System.out.println("barking...");
    }
}

class Cat extends Animal {
    void meow() {
        System.out.println("meowing...");
    }
}

class TestInheritance3 {
    public static void main(String args[]) {
        Cat c = new Cat();
        c.meow();
        c.eat();
        // c.bark();//C.T.Error
    }
}

//ִ���������õ����½�� -

meowing...
eating...
```

>Ϊʲô��Java�в�֧�ֶ��ؼ̳У�

    Ϊ�˽��͸����Բ������ԣ�Java�в�֧�ֶ��ؼ̳С�����һ����A��B��C�������ࡣ C��̳�A��B�ࡣ ���A��B������ͬ�ķ��������Ҵ���������������A��B��ĵ��÷����������塣
 
```
class A {
    void msg() {
        System.out.println("Hello");
    }
}

class B {
    void msg() {
        System.out.println("Welcome");
    }
}

class C extends A,B
{//suppose if it were  

 Public Static

    void main(String args[]) {
        C obj = new C();
        obj.msg();// Now which msg() method would be invoked?
    }
}
```
      ����ʱ���������ʱ����ã�����̳�2���࣬java���ڱ���ʱ������� ���������������Ƿ�����ͬ�ķ����������б������ʱ������������Ĵ����Ǳ������ġ�

### �� �ۺ�
>���һ������һ�����ʵ������(���е���)��������Ϊ�ۺϡ� �ۺϱ�ʾHAS-A��ϵ��

    ��ʱʹ�þۺϣ�
    
- ��û��is-a��ϵʱ��ͨ���ۺ�Ҳ����õ�ʵ�ִ������á�
- ֻ�������漰�Ķ������������������ά�ֹ�ϵΪis-aʱ����Ӧʹ�ü̳�; ���򣬾ۺ�����õ�ѡ��

``` Java
//Address.java
public class Address {
    String city, province;

    public Address(String city, String province) {
        this.city = city;
        this.province = province;
    }

}

//Emp.java
public class Emp {
    int id;
    String name;
    Address address;

    public Emp(int id, String name, Address address) {
        this.id = id;
        this.name = name;
        this.address = address;
    }

    void display() {
        System.out.println(id + " " + name);
        System.out.println(address.city + " " + address.province);
    }

    public static void main(String[] args) {
        Address address1 = new Address("����", "�㶫");
        Address address2 = new Address("����", "����");

        Emp e = new Emp(111, "Wang", address1);
        Emp e2 = new Emp(112, "Zhang", address2);

        e.display();
        e2.display();

    }
}

//ִ��������룬�õ����½�� -

111 Wang
���� �㶫
112 Zhang
���� ����
```

### �� ��д(Override)������(Overload)

#### 1.��д
>��������о����븸����������ͬ�ķ�������java�г�Ϊ�������ǡ����仰˵����������ṩ�����丸���ṩ������һ���������ض�ʵ�֣���������Ϊ�������ǡ����Է�������������ǰ���������̳к��Ӹ����з���������ͬ��

    Java�������ǵ��÷�

- ������д�����ṩ�б��ڳ����ṩ�ķ������ض�ʵ�֡�
- ������д��������ʱ��̬�ԡ�

---  
    Java�������ǵĹ���

- ���������븸���е�������ͬ��
- ������������븸������ͬ�Ĳ�����
- ������IS-A��ϵ(�̳�)��

##### 1.1 ���û�з������ǵ�����
``` Java
//����ڳ����в�ʹ�÷������ǿ������ٵ����⡣

class Vehicle {
    void run() {
        System.out.println("Vehicle is running");
    }
}

class Bike extends Vehicle {

    public static void main(String args[]) {
        Bike obj = new Bike();
        obj.run();
    }
}

//ִ��������룬���������� -

Vehicle is running
```
    �����ǣ��������������ṩһ��run()�����������ΪʲôҪʹ�÷������ǡ�
``` Java
//�������ǵ�ʾ��
//���������������У��ڸ����к������ж�������run����������������һЩ�ض���ʵ�֡� ���������ƺͲ�������ͬ�ģ�������֮����IS-A��ϵ���������run�����������ˡ�

class Vehicle {
    void run() {
        System.out.println("Vehicle is running");
    }
}

class Bike2 extends Vehicle {
    void run() {
        System.out.println("Bike is running safely");
    }

    public static void main(String args[]) {
        Bike2 obj = new Bike2();
        obj.run();
    }
}

//ִ������������ -

Bike is running safely
```

>���Ը��Ǿ�̬������

    ���ǲ����Եģ���̬�������ܱ����ǡ�
    ��Ϊ��̬�����ǰ��࣬��ʵ�������󶨶��� ��̬����������ʵ�����ڶ�����

#### 2. ����
>���һ�������ж��������ͬ���Ƶ�������ͬ�ķ��������Ϊ�������ء����ֻ��Ҫִ��һ��������������ͬ�ķ������ƽ����ӳ���Ŀɶ��ԡ�
�������ִ�и�����ֵ����Ӳ���(���)�����ǲ������������̶������Ϊ����������дadd1(int��int)������Ϊ����������дadd2(int��int��int)���������ܶ���������Ա��˵������������ķ�������Ϊ����Ϊ�������Ʋ�ͬ��
��ˣ�ִ�з��������ܱȽ������������塣

    �������ص��ŵ�

- ������������˳���Ŀɶ��ԡ�
- ���ط�����ͬ�ķ�ʽ

---
    ��java�����ط��������ַ�ʽ�����Ƿֱ��ǣ�

- ͨ���ı����������
- ͨ��������������

---
    ע�⣺��java�У�ֻͨ�����ķ����ķ���������ʵ�ַ��������ǲ����Եġ�


``` Java
class Adder {
    static int add(int a, int b) {
        return a + b;
    }
    static int add(int a, int b, int c) {
        return a + b + c;
    }
    static double add(double a, double b) {
        return a + b;
    }
}

class TestOverloading2 {
    public static void main(String[] args) {
        System.out.println(Adder.add(11, 11));
        System.out.println(Adder.add(12.3, 12.6));
    }
}

//�������ִ�к����������� -

22
24.9
```

>Ϊʲô�������ز���ͨ�����ķ����ķ������ͣ�

    ��java�У�ֻͨ���ı䷽���ķ���������ʵ�ַ��������ǲ����ܵģ���Ϊ��������ģ���ԡ� ������������ģ��������ô�������ģ�

``` Java
class Adder {
    static int add(int a, int b) {
        return a + b;
    }

    static double add(int a, int b) {
        return a + b;
    }
}

class TestOverloading3 {
    public static void main(String[] args) {
        System.out.println(Adder.add(11, 11));// ambiguity
    }
}

//�������ִ�к����������� -

Compile Time Error: method add(int,int) is already defined in class Adder
Java
```

System.out.println(Adder.add(11,11));//���java���ȷ��Ӧ�õ����ĸ�sum()������

    ע�⣺����ʱ������������ʱ���� ���ԣ������������ͬ�ķ���������ͬ�Ĳ�����java��������Ⱦ������ʱ�����

>��������java main()������

    ������ȫ���Եġ� ����ͨ����������������������������main������ ����JVM����main()��������ֻ�����ַ���������Ϊ������ ����������һ���򵥵����ӣ�

``` Java
class TestOverloading4{  
    public static void main(String[] args){System.out.println("main with String[]");}  
    public static void main(String args){System.out.println("main with String");}  
    public static void main(){System.out.println("main without args");}  
}

//�������ִ�к����������� -

main with String[]
```

#### �������غͷ�����д������
|��������|������д|
 :-: | -: |
��������������߳���Ŀɶ��ԡ�|	������д�����ṩ�Ѿ����䳬���ṩ�ķ������ض�ʵ�֡�
��������������ִ�С�|	������д�����ھ���IS-A(�̳�)��ϵ���������С�
�ڷ������ص�����£��������벻ͬ��|	�ڷ�����д������£�����������ͬ��
���������Ǳ���ʱ��̬�Ե����ӡ�|	������д/����������ʱ��̬�Ե����ӡ�
�������ز��ܽ�ͨ���ı䷽���ķ���������ִ�С����������еķ������Ϳ�����ͬ��ͬ�� ���Ǳ�����Ĳ������͡�|	�ڷ�����д/�����з������ͱ�����ͬ��Э�䡣

### �� ��̬
>��̬��ͬһ����Ϊ���ж����ͬ������ʽ����̬��������

    ��̬���Ƕ�����ֱ�����ʽ�����֡�

    ��������˵"����"������������кܶ಻ͬ�ı���ʵ�֣�������Сè��С��������ȵȡ���ô�ҵ������˵"�����һֻ����"������Ա����Сè��С���������涼���ԣ����Ǿ�˵"����"�������;߱���̬�ԡ�

``` Java
//����
public interface Vegetarian{}
public class Animal{}
public class Deer extends Animal implements Vegetarian{}
```

    ��ΪDeer����ж��ؼ̳У����������ж�̬�ԡ�����ʵ���������£�

- һ�� Deer IS-A����һ���� Animal
- һ�� Deer IS-A����һ���� Vegetarian
- һ�� Deer IS-A����һ���� Deer
- һ�� Deer IS-A����һ����Object

---
    ��Java�У����еĶ��󶼾��ж�̬�ԣ���Ϊ�κζ�����ͨ��IS-A���Ե����ͺ�Object�ࡣ

    1. ����һ�������Ψһ��������ͨ�������ͱ�����

    2. �����ͱ���ֻ����һ�����ͣ�һ���������������ͱ��������;Ͳ��ܱ��ı��ˡ�

    3. �����ͱ��������ܹ�������Ϊ��������ǰ������Щ����û�б�����Ϊfinal�����������ú���������ͬ�Ļ�������ݵĶ�������������Ϊ�����ͻ��߽ӿ����͡�

``` Java
//�����ǽ������ͱ���Ӧ����Deer���������ʱ������������ǺϷ��ģ�

Deer d = new Deer();
Animal a = d;
Vegetarian v = d;
Object o = d;
//���е������ͱ���d,a,v,o��ָ�������ͬ��Deer����
```

#### �鷽��
>��������������д�ķ���ʱ�����õ�������ķ����������Ǹ����б���д�ķ�����

    Ҫ����ø����б���д�ķ����������ʹ�ùؼ���super��

``` Java
public class Employee
{
   private String name;
   private String address;
   private int number;
   public Employee(String name, String address, int number)
   {
      System.out.println("Constructing an Employee");
      this.name = name;
      this.address = address;
      this.number = number;
   }
   public void mailCheck()
   {
      System.out.println("Mailing a check to " + this.name
       + " " + this.address);
   }
   public String toString()
   {
      return name + " " + address + " " + number;
   }
   public String getName()
   {
      return name;
   }
   public String getAddress()
   {
      return address;
   }
   public void setAddress(String newAddress)
   {
      address = newAddress;
   }
   public int getNumber()
   {
     return number;
   }
}
```

``` Java
public class Salary extends Employee
{
   private double salary; //Annual salary
   public Salary(String name, String address, int number, double
      salary)
   {
       super(name, address, number);
       setSalary(salary);
   }
   public void mailCheck()
   {
       System.out.println("Within mailCheck of Salary class ");
       System.out.println("Mailing check to " + getName()
       + " with salary " + salary);
   }
   public double getSalary()
   {
       return salary;
   }
   public void setSalary(double newSalary)
   {
       if(newSalary >= 0.0)
       {
          salary = newSalary;
       }
   }
   public double computePay()
   {
      System.out.println("Computing salary pay for " + getName());
      return salary/52;
   }
}
```

    ����������ϸ�Ķ�����Ĵ��룬���Ը���������������

``` Java
public class VirtualDemo
{
   public static void main(String [] args)
   {
      Salary s = new Salary("Mohd Mohtashim", "Ambehta, UP", 3, 3600.00);
      Employee e = new Salary("John Adams", "Boston, MA", 2, 2400.00);
      System.out.println("Call mailCheck using Salary reference --");
      s.mailCheck();
      System.out.println("\n Call mailCheck using Employee reference--");
      e.mailCheck();
    }
}

//����ʵ���������н�����£�
Constructing an Employee
Constructing an Employee
Call mailCheck using Salary reference --
Within mailCheck of Salary class
Mailing check to Mohd Mohtashim with salary 3600.0

Call mailCheck using Employee reference--
Within mailCheck of Salary class
Mailing check to John Adams with salary 2400.0
```

    �����У�����ʵ����������Salary����һ��ʹ��Salary����s����һ��ʹ��Employee���á�
    ����ʱ����������鵽mailCheck()������Salary���е�������

    �ڵ���s.mailCheck()ʱ��Java�����(JVM)����Salary���mailCheck()������

    ��Ϊe��Employee�����ã����Ե���e��mailCheck()����������ȫ��ͬ�Ľ����

    �����������e.mailCheck()����ʱ����������鵽Employee���е�mailCheck()������

    �ڱ����ʱ�򣬱�����ʹ��Employee���е�mailCheck()������֤����䣬 ���������е�ʱ��Java�����(JVM)���õ���Salary���е�mailCheck()������

    ����Ϊ����Ϊ���ⷽ�����ã��÷�������Ϊ���ⷽ����

    Java�����еķ������������ַ�ʽ���֣���ˣ���д�ķ�����������ʱ���ã����ܱ����ʱ��Դ���������ñ�����ʲô�������͡�

### �� ������
>���������ĸ����У����еĶ�����ͨ���������ģ����Ƿ����������������е��඼������������ģ����һ������û�а����㹻����Ϣ�����һ������Ķ�������������ǳ����ࡣ

    ��������˲���ʵ��������֮�⣬�������������Ȼ���ڣ���Ա��������Ա�����͹��췽���ķ��ʷ�ʽ����ͨ��һ����
    
    ���ڳ����಻��ʵ�����������Գ�������뱻�̳У����ܱ�ʹ�á�Ҳ����Ϊ���ԭ��ͨ������ƽ׶ξ���Ҫ��Ҫ��Ƴ����ࡣ
    
    ������������༯�ϵĳ����ķ������������ڸ��౾���ǳ���ģ����Բ���ʹ����Щ������

### �� ��װ
>����������ʽ��Ʒ����У���װ��Ӣ�Encapsulation����ָ��һ�ֽ������Ժ�ʽ�ӿڵ�ʵ��ϸ�ڲ��ݰ�װ�����������ķ�����

    ��װ���Ա���Ϊ��һ���������ϣ���ֹ����Ĵ�������ݱ��ⲿ�ඨ��Ĵ���������ʡ�

    Ҫ���ʸ���Ĵ�������ݣ�����ͨ���ϸ�Ľӿڿ��ơ�

    ��װ����Ҫ�Ĺ��������������޸��Լ���ʵ�ִ��룬�������޸���Щ�������Ǵ���ĳ���Ƭ�Ρ�

### �� �ӿ�
>�ӿڣ�Ӣ�ģ�Interface������JAVA�����������һ���������ͣ��ǳ��󷽷��ļ��ϣ��ӿ�ͨ����interface��������һ����ͨ���̳нӿڵķ�ʽ���Ӷ����̳нӿڵĳ��󷽷���

    �ӿڲ������࣬��д�ӿڵķ�ʽ��������ƣ������������ڲ�ͬ�ĸ����������������Ժͷ������ӿ��������Ҫʵ�ֵķ�����

    ����ʵ�ֽӿڵ����ǳ����࣬�������Ҫ����ӿ��е����з�����

    �ӿ��޷���ʵ���������ǿ��Ա�ʵ�֡�һ��ʵ�ֽӿڵ��࣬����ʵ�ֽӿ��������������з���������ͱ�������Ϊ�����ࡣ���⣬��Java�У��ӿ����Ϳ���������һ�����������ǿ��Գ�Ϊһ����ָ�룬���Ǳ�����һ���Դ˽ӿ�ʵ�ֵĶ���

---
    �ӿ��������Ƶ㣺

- һ���ӿڿ����ж��������
- �ӿ��ļ�������.java��β���ļ��У��ļ���ʹ�ýӿ�����
- �ӿڵ��ֽ����ļ�������.class��β���ļ��С�
- �ӿ���Ӧ���ֽ����ļ����������������ƥ���Ŀ¼�ṹ�С� 

---
    �ӿ����������
- �ӿڲ�������ʵ��������
- �ӿ�û�й��췽����
- �ӿ������еķ��������ǳ��󷽷���
- �ӿڲ��ܰ�����Ա����������static��final������
- �ӿڲ��Ǳ���̳��ˣ�����Ҫ����ʵ�֡�
- �ӿ�֧�ֶ��ؼ̳С�

#### 8.1 �ӿڵ�����

```
[�ɼ���] interface �ӿ����� [extends ����������] {
        // ��������
        // ���󷽷�
}

public interface NameOfInterface
{
   //�κ����� final, static �ֶ�
   //���󷽷�
}
```
    �ӿ����������ԣ�
- �ӿ�����ʽ����ģ�������һ���ӿڵ�ʱ�򣬲���ʹ��abstract�ؼ��֡�
- �ӿ���ÿһ������Ҳ����ʽ����ģ�����ʱͬ������Ҫabstract�ؼ��ӡ�
- �ӿ��еķ������ǹ��еġ�

#### 8.2 �ӿڵ�ʵ��
>����ʵ�ֽӿڵ�ʱ����Ҫʵ�ֽӿ������еķ������������������Ϊ������ࡣ

    ��ʹ��implements�ؼ���ʵ�ֽӿڡ����������У�Implements�ؼ��ַ���class�������档

``` Java
//ʵ��һ���ӿڵ��﷨������ʹ�������ʽ��

... implements �ӿ�����[, �����ӿ�, �����ӿ�..., ...] ...

//ʵ����
public class MammalInt implements Animal{

   public void eat(){
      System.out.println("Mammal eats");
   }

   public void travel(){
      System.out.println("Mammal travels");
   } 

   public int noOfLegs(){
      return 0;
   }

   public static void main(String args[]){
      MammalInt m = new MammalInt();
      m.eat();
      m.travel();
   }
} 

//����ʵ���������н������:
Mammal eats
Mammal travels
```
    ��д�ӿ��������ķ���ʱ����Ҫע�����¹���

- ����ʵ�ֽӿڵķ���ʱ�������׳�ǿ�����쳣��ֻ���ڽӿ��У����߼̳нӿڵĳ��������׳���ǿ�����쳣��
- ������д����ʱҪ����һ�µķ�����������Ӧ�ñ�����ͬ��������ݵķ���ֵ���͡�
- ���ʵ�ֽӿڵ����ǳ����࣬��ô��û��Ҫʵ�ָýӿڵķ�����

---
    ��ʵ�ֽӿڵ�ʱ��ҲҪע��һЩ����

- һ�������ͬʱʵ�ֶ���ӿڡ�
- һ����ֻ�ܼ̳�һ���࣬������ʵ�ֶ���ӿڡ�
- һ���ӿ��ܼ̳���һ���ӿڣ������֮��ļ̳бȽ����ơ�

#### 8.3 �ӿڵļ̳�
>һ���ӿ��ܼ̳���һ���ӿڣ�����֮��ļ̳з�ʽ�Ƚ����ơ��ӿڵļ̳�ʹ��extends�ؼ��֣��ӽӿڼ̳и��ӿڵķ�����

    ��Java�У���Ķ��ؼ̳��ǲ��Ϸ������ӿ�������ؼ̳У���

``` Java
//�ڽӿڵĶ��ؼ̳���extends�ؼ���ֻ��Ҫʹ��һ�Σ��������ż̳нӿ�:

public interface Hockey extends Sports, Event
```
#### 8.4 ��ǽӿ�
>��õļ̳нӿ���û�а����κη����Ľӿڡ�

    ��ʶ�ӿ���û���κη��������ԵĽӿ�.��������������������һ���ض�������,����������������������һЩ���顣

    ��ʶ�ӿ����ã��������˵���Ǹ�ĳ���������꣨�Ǹ�������ʹ����ӵ��ĳ����ĳЩ��Ȩ��

``` Java
//���磺java.awt.event���е�MouseListener�ӿڼ̳е�java.util.EventListener�ӿڶ������£�
package java.util;
public interface EventListener
{}
```

    û���κη����Ľӿڱ���Ϊ��ǽӿڡ���ǽӿ���Ҫ������������Ŀ�ģ�

- ����һ�������ĸ��ӿڣ�
        
        ����EventListener�ӿڣ������ɼ�ʮ�������ӿ���չ��Java API�������ʹ��һ����ǽӿ�������һ��ӿڵĸ��ӿڡ����磺��һ���ӿڼ̳���EventListener�ӿڣ�Java�����(JVM)��֪���ýӿڽ�Ҫ������һ���¼��Ĵ�������

- ��һ��������������ͣ�
    
        ��������Ǳ�ǽӿ������Ŀ�ģ�ʵ�ֱ�ǽӿڵ��಻��Ҫ�����κνӿڷ���(��Ϊ��ǽӿڸ�����û�з���)�����Ǹ���ͨ����̬�Ա��һ���ӿ����͡�
