### Java �������
>Java��Ϊһ������������ԡ�֧�����»������
    1. ��̬
    2. �̳�
    3. ��װ
    5. ����
    6. ��
    7. ����
    8. ʵ��
    9. ����
    10. ��Ϣ����


- ���󣺶��������һ��ʵ������״̬����Ϊ�����磬һ������һ����������״̬�У���ɫ�����֡�Ʒ�֣���Ϊ�У�ҡβ�͡��С��Եȡ�
- �ࣺ����һ��ģ�壬������һ��������Ϊ��״̬��

---
#### 1. Java�еĶ���
>����״̬����Ϊ��ʵ��ɳ�Ϊ����(Ů����Ҳ���Խж���)�� ���ӣ����г�����ǣ��ʣ����ӣ������ȡ���������������߼�(���κ�����)�� ���ζ��������������ϵͳ��

    һ�������������ص㣺

- ״̬�� ��ʾһ�����������(ֵ)��
- ��Ϊ�� ��ʾ�������Ϊ(����)�����磺��ȡ��ȡ�
- ��ʶ�� �����ʶͨ��ͨ��ΨһIDʵ�֡���ID��ֵ���ⲿ�û����ɼ��� ���ǣ�����JVM�ڲ�ʹ����Ψһ�ر�ʶÿ������

    ���磺 ������һ���������������ǣ��ݴ��ɫ�ǰ�ɫ����Щ��������״̬(����ֵ)����������·��������·����������Ϊ��

>���������һ��ʵ���� ���Ǵ��������ģ�����ͼ�� ���Զ�����һ�����ʵ����

    �����壺

- ������һ����ʵ�����ʵ�塣
- ������һ������ʱʵ�塣
- �����Ǿ���״̬����Ϊ��ʵ�塣
- ���������һ��ʵ����

---

#### 2. Java�е���
>���Ǿ��й�ͬ���Ե�һ��������Ǵ��������ģ�����ͼ������һ���߼�ʵ�塣 ��������������ڵ�ʵ�塣

    Java�е�����԰�����

- �ֶ�
- ����
- ���캯��
- �����
- Ƕ����ͽӿ�

``` Java
//����һ������﷨��
class <class_name>{  
    field;  
    method;  
}
```

##### 2.1. Java�е�ʵ������
>ʵ�����������ڲ������ڷ����ⲿ����ı�����Ϊʵ�������� ʵ�������ڱ���ʱ����ȡ�ڴ档 ��������ʱ��ȡ����(ʵ��)����ʱ���ڴ档 ����Ϊʲô��������Ϊʵ��������

##### 2.2. Java�еķ���
>��java�еķ������ƺ��������ڱ�¶�������Ϊ��

    �������ŵ�

- �����������
- �����Ż�

##### 2.3. Java�е�new�ؼ���
>new�ؼ�������������ʱ�����ڴ档���ж����ڶ��ڴ������л�ȡ�ڴ档

#### 2.4���췽��
>ÿ���඼�й��췽�������û����ʽ��Ϊ�ඨ�幹�췽����Java����������Ϊ�����ṩһ��Ĭ�Ϲ��췽����

    �ڴ���һ�������ʱ������Ҫ����һ�����췽�������췽�������Ʊ�������ͬ����һ��������ж�����췽����

``` Java
//������һ�����췽��ʾ����
public class Puppy{
   public Puppy(){
   }

   public Puppy(String name){
      // �������������һ��������name
   }
}
```

#### 2.5��������
    �����Ǹ����ഴ���ġ���Java�У�ʹ�ùؼ���new������һ���µĶ��󡣴���������Ҫ����������

- ����������һ�����󣬰����������ƺͶ������͡�
- ʵ������ʹ�ùؼ���new������һ������
- ��ʼ����ʹ��new��������ʱ������ù��췽����ʼ������

``` Java
//������һ��������������ӣ�
public class Puppy{
   public Puppy(String name){
      //�������������һ��������name
      System.out.println("Passed Name is :" + name ); 
   }
   public static void main(String []args){
      // �������佫����һ��Puppy����
      Puppy myPuppy = new Puppy( "tommy" );
   }
}

//���벢��������ĳ��򣬻��ӡ������Ľ����
Passed Name is :tommy
```

#### ��Java�д�������Ĳ�ͬ��������Щ��
    ��java���кܶ෽���������������������Ƿֱ��ǣ�

- ͨ��new�ؼ���
- ͨ��newInstance()����
- ͨ��clone()����
- ͨ�������л�
- ͨ������������
- �ڽ��������½��У���ѧϰ��Щ����������������

#### ��������
    ����ֻ�Ǳ�ʾû������û�����õĶ���(Ҳ���ǲ�ʹ��ʵ������)��Ϊ����������ֻ���ڴ�������ʱʹ�á����ֻ��Ҫʹ��һ����������������һ���ܺõķ����� ���磺

``` Java
new Puppy();//��������
Puppy p = new Puppy();// ʹ��ʵ�����������Բ�����������
```

---

### Դ�ļ���������
>����һ��Դ�ļ��ж������࣬���һ���import����package���ʱ��Ҫ�ر�ע����Щ����

- һ��Դ�ļ���ֻ����һ��public��
- һ��Դ�ļ������ж����public��
- Դ�ļ�������Ӧ�ú�public�����������һ�¡����磺Դ�ļ���public���������Employee����ôԴ�ļ�Ӧ������ΪEmployee.java��
- ���һ���ඨ����ĳ�����У���ôpackage���Ӧ����Դ�ļ������С�
- ���Դ�ļ�����import��䣬��ôӦ�÷���package�����ඨ��֮�䡣���û��package��䣬��ôimport���Ӧ����Դ�ļ�����ǰ�档
- import����package����Դ�ļ��ж���������඼��Ч����ͬһԴ�ļ��У����ܸ���ͬ���಻ͬ�İ�������
- ���������ַ��ʼ��𣬲�����Ҳ�ֲ�ͬ�����ͣ��������final��ȡ���Щ���ڷ��ʿ����½ڽ��ܡ�

    ���������ᵽ�ļ������ͣ�Java����һЩ������࣬�磺�ڲ��ࡢ�����ࡣ

---
### Java��
>����Ҫ��������ͽӿڽ��з��ࡣ������Java����ʱ�����ܱ�д�ɰ���ǧ���࣬��˺��б�Ҫ����ͽӿڽ��з��ࡣ

---
### Import���
>��Java�У��������һ���������޶�����������������������ôJava�������Ϳ��Ժ����׵ض�λ��Դ��������ࡣImport�����������ṩһ�������·����ʹ�ñ����������ҵ�ĳ���ࡣ

``` Java
//���磬����������н����������������java_installation/java/io·���µ�������
import java.io.*;
```

### һ���򵥵�����

``` Java
class Employee{
    String name;
    int age;
    String designation;
    double salary;
    // Employee ��Ĺ�����
    public Employee(String name){
        this.name = name;
    }
    // ����age��ֵ
    public void empAge(int empAge){
        age =  empAge;
    }
    /* ����designation��ֵ*/
    public void empDesignation(String empDesig){
        designation = empDesig;
    }
    /* ����salary��ֵ*/
    public void empSalary(double empSalary){
        salary = empSalary;
    }
    /* ��ӡ��Ϣ */
    public void printEmployee(){
        System.out.println("Name:"+ name );
        System.out.println("Age:" + age );
        System.out.println("Designation:" + designation );
        System.out.println("Salary:" + salary);
    }
}

public class EmployeeExample {

    public static void main(String args[]){
        /* ʹ�ù����������������� */
        Employee empOne = new Employee("James Smith");
        Employee empTwo = new Employee("Mary Anne");

        // ��������������ĳ�Ա����
        empOne.empAge(26);
        empOne.empDesignation("Senior Software Engineer");
        empOne.empSalary(1000);
        empOne.printEmployee();

        empTwo.empAge(21);
        empTwo.empDesignation("Software Engineer");
        empTwo.empSalary(500);
        empTwo.printEmployee();
    }
}

//���н����
Name:James Smith
Age:26
Designation:Senior Software Engineer
Salary:1000.0
Name:Mary Anne
Age:21
Designation:Software Engineer
Salary:500.0
```

