> 本文由 [简悦 SimpRead](http://ksria.com/simpread/) 转码， 原文地址 [blog.csdn.net](https://blog.csdn.net/java945870697/article/details/126193367?spm=1001.2100.3001.7377&utm_medium=distribute.pc_feed_blog_category.none-task-blog-classify_tag-20-126193367-null-null.nonecase&depth_1-utm_source=distribute.pc_feed_blog_category.none-task-blog-classify_tag-20-126193367-null-null.nonecase)

#### 目录

*   [1.Java 基础](#1Java_5)
*   *   [1.1 说说 JVM 内存模型](#11_JVM_6)
    *   [1.2 说说 JVM 的垃圾回收算法](#12_JVM_21)
    *   [1.3 类加载机制](#13__28)
    *   [1.4 谈谈你对泛型的了解](#14___38)
    *   [1.5 创建线程的方式](#15__40)
    *   [1.6 说说反射机制](#16__160)
    *   [1.7 动态代理有哪几种](#17__168)
    *   [1.8 JVM 中怎么判断能被垃圾回收机制回收](#18_JVM_175)
    *   [1.9 谈谈 Java 中的值传递和引用传递](#19_Java_183)
    *   [1.10 Java 的四种引用方式](#110_Java_190)
    *   [1.11 JVM 堆内存分配](#111_JVM_197)
    *   [1.12 JVM 垃圾收集器有哪些](#112_JVM_206)
    *   [1.13 HashCode() 和 equals() 的区别](#113_HashCodeequals_210)
    *   [1.14 常见的设计模式](#114__217)
    *   [1.15 Object 类的方法有哪些](#115_Object_224)
    *   [1.16 抽象类和接口的区别](#116__233)
    *   [1.17 final、finally、finalize 的区别](#117_finalfinallyfinalize_239)
*   [2. 多线程](#2_252)
*   *   [2.1 谈谈 synchronized 的原理及底层实现](#21_synchronized_253)
    *   [2.2 synchronized 与 Lock 的区别](#22_synchronizedLock_262)
    *   [2.3 什么是可重入锁](#23__267)
    *   [2.4 死锁产生的条件（如何解决？怎么判断死锁？）](#24__274)
    *   [2.5 讲一讲 ThreadLocal](#25_ThreadLocal_292)
    *   [2.6 ThreadLocal 的内存泄漏，如何避免呢？](#26_ThreadLocal_298)
    *   [2.7 谈谈进程和线程](#27__306)
    *   [2.8 谈一谈 ReentrantLock](#28_ReentrantLock_310)
    *   [2.9 ReentrantLock 和 Synchronized 区别](#29_ReentrantLockSynchronized_317)
    *   [2.10 讲一讲 CAS](#210_CAS_324)
    *   [2.11 讲一讲 volatile 关键字](#211_volatile_330)
    *   [2.12 线程池核心参数和工作原理](#212__336)
    *   [2.13 wait()、sleep() 和 yield() 方法的区别](#213_waitsleepyield_351)
*   [3. 集合](#3_365)
*   *   [3.1 ArrayList 底层原理](#31_ArrayList_366)
    *   [3.2 ArrayList 和 LinkedList 的区别](#32_ArrayListLinkedList_372)
    *   [3.3 HashMap 1.7 和 1.8 的区别](#33_HashMap_17_18_382)
    *   [3.4 HashMap1.8 为什么使用红黑树](#34_HashMap18_396)
    *   [3.5 什么是哈希碰撞，怎么解决？](#35__400)
    *   [3.6 请你说说 ConcurrentHashMap](#36_ConcurrentHashMap_412)
    *   [3.7 请你说说 CopyOnWriteArraylist](#37_CopyOnWriteArraylist_419)
    *   [3.8 HashMap 和 Hashtable 的区别](#38_HashMapHashtable_425)
    *   [3.9 List 与 Set 接口有什么区别](#39_ListSet_433)
*   [4. 异常](#4_440)
*   *   [4.1 throw 和 throws 的区别](#41_throwthrows_441)
    *   [4.2 异常分类](#42__447)
*   [5.Spring、SpringBoot、SpringMVC](#5SpringSpringBootSpringMVC_467)
*   *   [5.1 谈谈 IOC 和 AOP](#51_IOCAOP_468)
    *   [5.2 SpringBoot 启动流程](#52_SpringBoot_474)
    *   [5.3 SpringBoot 的自动装配](#53_SpringBoot_483)
    *   [5.4 @Autowired 和 @Resource 注解的区别](#54_AutowiredResource_487)
    *   [5.5 Spring 事务失效原因](#55__Spring_494)
    *   [5.6 说说 BeanFactory 和 FactoryBean 的区别](#56_BeanFactoryFactoryBean_501)
    *   [5.7 SpringBoot 自定义注解](#57_SpringBoot_507)
    *   [5.8 SpringMVC 的三层框架](#58_SpringMVC_521)
    *   [5.9 SpringMVC 的执行流程](#59_SpringMVC_526)
    *   [5.10 说说 Spring Boot 的起步依赖 (starter 自动化配置)](#510_Spring_Bootstarter_534)
    *   [5.11 bean 的生命周期](#511_bean_538)
    *   [5.12 bean 的作用域](#512_bean_545)
    *   [5.13 Springmvc 拦截器和过滤器的区别](#513_Springmvc_552)
    *   [5.14 @RestController 和 @Controller 的区别](#514_RestControllerController_559)
    *   [5.15 @Component 和 @Bean 的区别](#515_ComponentBean_565)
    *   [5.16 springboot 中事务如何开启](#516_springboot_571)
    *   [5.17 bean 实例化的三种方式](#517_bean_575)
*   [6.Mybatis](#6Mybatis_589)
*   *   [6.1 Mybatis 的三种传值方式](#61_Mybatis_590)
    *   [6.2 Mybatis 的一级缓存和二级缓存](#62_Mybatis_658)
*   [7.Mysql](#7Mysql_664)
*   *   [7.1 索引查询失效的几个情况](#71_665)
    *   [7.2 Mysql 的事务特性 及事务的传播方式](#72_Mysql___675)
    *   [7.3 Mysql 的事务隔离级别](#73_Mysql_690)
    *   [7.4 Mysql 数据库常用的锁](#74_Mysql_701)
    *   [7.5 Mysql 与 Redis 的区别](#75_MysqlRedis_727)
    *   [7.6 Innodb 和 Myisam 的区别](#76_InnodbMyisam_738)
    *   [7.7 请你说说 InnoDB 的 MVCC 机制（难点）](#77_InnoDBMVCC_747)
    *   [7.8 数据库索引为什么使用 B + 数](#78_B_758)
    *   [7.9 讲一讲 sql 优化](#79_sql_763)
    *   [7.10 count(*) 和 count(1) 的区别](#710_countcount1_771)
    *   [7.11 mysql 索引](#711_mysql_777)
    *   [7.12 left join、right join、inner join 的区别](#712_left_joinright_joininner_join_782)
    *   [7.13 为什么 mysql 默认隔离级别设置为 RR（可重复读）](#713_mysqlRR_788)
    *   [7.14 MySQL 普通索引和唯一索引区别](#714_MySQL_794)
    *   [7.15 常见 mysql 的慢查询优化方式](#715_mysql_805)
    *   [7.16 mysql 主从复制](#716_mysql_810)
    *   [7.17 当前读与快照读的区别](#717__822)
    *   [7.18 sql 语句执行顺序](#718_sql_830)
*   [8.Redis](#8Redis_837)
*   *   [8.1 谈谈 Redis 的应用场景](#81_Redis__838)
    *   [8.2 如何利用 Redis 实现一个分布式锁？](#82_Redis_845)
    *   [8.3 Redis 的基本数据类型及底层数据结构](#83_Redis_874)
    *   [8.4 Redis 如何与数据库保持双写一致性](#84_Redis_923)
    *   [8.5 Redis 的持久化策略](#85_Redis_927)
    *   [8.6 说说缓存穿透、击穿、雪崩以及如何避免](#86__932)
    *   [8.7 redis 是单线程还是多线程，为什么？](#87_redis_943)
    *   [8.8 什么是 IO 多路复用机制？](#88_IO_949)
*   [9.MQ](#9MQ_960)
*   *   [9.1 为什么要使用 MQ](#91_MQ_961)
    *   [9.2 如何解决 MQ 消息丢失问题？](#92_MQ_972)
*   [10.Dubbo](#10Dubbo_978)
*   [11. 计算机网络](#11_981)
*   *   [11.1 TCP 和 UDP 的区别](#111_TCPUDP_982)
    *   [11.2 TCP 三次握手和四次挥手过程](#112_TCP_987)
    *   [11.3 七层网络协议](#113__1000)
    *   [在这里插入图片描述](#httpsimgblogcsdnimgcnbfa51de4756e4b0c8cdc7edebe522c77png_1001)
    *   [11.3 Http 和 Https 详解](#113_HttpHttps_1003)
    *   [11.4 Http 状态码](#114_Http_1009)
    *   [11.5 TCP 粘包](#115_TCP_1018)
*   [12.Linux](#12Linux_1033)
*   *   [12.1 linux 常用命令](#121_linux_1034)
*   [13.JWT](#13JWT_1050)

1.Java 基础
---------

### 1.1 说说 JVM 内存模型

JVM 由三部分组成：**类加载子系统、执行引擎、运行时数据区。**

**类加载子系统**：可以根据指定的全限定名来载入类或接口。  
**执行引擎**：负责执行那些被载入类的方法中的指令。  
**运行时数据区**：包含五部分的内容：栈、堆、本地方法栈（为 [Native 方法](https://so.csdn.net/so/search?q=Native%E6%96%B9%E6%B3%95&spm=1001.2101.3001.7020)提供服务）、方法区 (元空间)、程序计数器（用来保存线程执行的位置）。

**栈**：存放的是一个个的栈帧，每个栈帧对应一个被调用的方法，在栈帧中包含**局部变量**和**对象的引用**  
**堆**：存储**对象实例**的以及**数组**

**线程私有**：栈、本地方法栈、程序计数器  
**线程共享**：堆、方法区

### 1.2 说说 JVM 的垃圾回收算法

1.  **标记 - 清除**，先标记要清除的对象，然后统一回收这些对象，不需要额外的空间，但是需要两次扫描**耗时严重**并且会**产生内存碎片**；
2.  **标记 - 复制（年轻代）**，将内存分为两块，每次只使用其中一块，当这块内存用完，就将还活着的对象复制到另外一块上面，效率高且**没有内存碎片**，但是**需要双倍的空间**，年轻代中使用复制算法；
3.  **标记 - 整理（老年代）**，标记存活对象，然后将标记的存活对象按内存地址依次排序，清除边界外未标记的对象，**没有内存碎片**，**但是需要移动对象**。

### 1.3 [类加载](https://so.csdn.net/so/search?q=%E7%B1%BB%E5%8A%A0%E8%BD%BD&spm=1001.2101.3001.7020)机制

类加载机制总共包括个阶段：**加载，验证，准备，解析，初始化**

**加载**：通过类加载器，使用字节码文件创建类对象。  
**验证**：主要是验证当前的字节流包含的信息是否符合当前的虚拟机环境。  
**准备**：为类变量（static 修饰的变量）分配内存，并赋值.  
**解析**：主要是将常量池的符号引用变成直接引用。  
**初始化**：执行类构造器方法的过程。

### 1.4 谈谈你对泛型的了解

### 1.5 创建线程的方式

1.  **继承 Thread 类**

```
public class ThreadTEST {
    public static void main(String[] args) {
        Thread.currentThread().setName("main thread");
        MyThread myThread1 = new MyThread();
        MyThread myThread2 = new MyThread();
 
        myThread1.start();
        myThread2.start();
    }
}
 
class MyThread extends Thread {
    @Override
    public void run() {
        for (int i = 0; i < 5; i++) {
            System.out.println(Thread.currentThread().getName() + i);
        }
    }
}
```

2.  **实现 Runnable 接口**

```
public class RunnableTest {
 
    public static void main(String[] args) {
        Thread thread = new Thread(new MyRunnable());
        //开启线程
        thread.start();
        for(int i = 0; i <5;i++){
            System.out.println(Thread.currentThread().getName() + i);
        }
    }
}
 
class MyRunnable implements Runnable {
 
    @Override
    public void run() {
        for (int i = 0; i < 10; i++) {
            System.out.println(Thread.currentThread().getName() + i);
        }
    }
}
```

3.  **实现 Callable 接口**

```
public class CallableTest {
 
    public static void main(String[] args) {
        //执行Callable 方式，需要FutureTask 实现实现，用于接收运算结果
        FutureTask<Integer> futureTask = new FutureTask<Integer>(new MyCallable());
        new Thread(futureTask).start();
        //接收线程运算后的结果
        try {
            Integer sum = futureTask.get();
            System.out.println(sum);
        } catch (InterruptedException e) {
            e.printStackTrace();
        } catch (ExecutionException e) {
            e.printStackTrace();
        }
    }
}
 
class MyCallable implements Callable<Integer> {
 
    @Override
    public Integer call() throws Exception {
        int sum = 0;
        for (int i = 0; i < 100; i++) {
            sum += i;
        }
        return sum;
    }
}
```

注：**Callable 和 Runnable 的区别**？  
1.Runnable 重写的方法是 run()，Callable 重写的方法是 call()。  
2.Runnable 没有返回值，Callable 可以通过 FutureTask 接收返回值。

4.  **线程池创建线程**

```
//线程池实现
public class ThreadPoolExecutorTest {
 
    public static void main(String[] args) {
        //创建线程池
        ExecutorService executorService = Executors.newFixedThreadPool(10);
        ThreadPool threadPool = new ThreadPool();
        for(int i =0;i<5;i++){
            //为线程池分配任务
            executorService.submit(threadPool);
        }
        //关闭线程池
        executorService.shutdown();
    }
}
 
class ThreadPool implements Runnable {
 
    @Override
    public void run() {
        for(int i = 0 ;i<10;i++){
            System.out.println(Thread.currentThread().getName() + ":" + i);
        }
    }
 
}
```

### 1.6 说说反射机制

反射就是在**程序运行期间动态的获取对象的属性和方法**的功能叫做反射。  
获取 Class 对象的三种方式：

1.  对象. getClass()
2.  类名. class
3.  Class.forName(路径)

### 1.7 动态代理有哪几种

1.  **JDK 原生动态代理**  
    JDK 原生动态代理是 Java 原生支持的，不需要任何外部依赖，它是**基于接口进行代理**。
    
2.  **CGLIB 动态代理**  
    CGLIB **通过继承的方式进行代理**（让需要代理的类成为 Enhancer 的父类），无论目标对象有没有实现接口都可以代理。
    

### 1.8 JVM 中怎么判断能被垃圾回收机制回收

1.  **引用计数法**  
    给对象添加一个引用计数器，每当有一个地方引用，计数器就加 1。当引用失效，计数器就减 1。任何时候计数器为 0 的对象就是不可能再被使用的。
    
2.  **可达性分析算法**  
    通过一系列的称为”GC Roots“的对象作为起点，从这些节点开始向下搜索，当一个对象到 GC Roots 没有任何引用链相连的话，则证明此对象时不可用的。
    

### 1.9 谈谈 Java 中的值传递和引用传递

在 Java 中所有的参数传递，不管基本类型还是引用类型，**都是值传递**。

1.  如果是**对基本数据类型的数据进行操作**，由于原始内容和副本都是存储实际值，并且是在不同的栈帧内，因此**形参的操作，不影响原始内容**。
2.  如果是对**引用类型的数据进行操作**（两种情况）：  
    2.1 形参和实参保持**指向同一个对象地址**，则形参的操作，**会影响**实参指向的对象的内容。  
    2.2 形参**被改动指向新的对象地址**，则形参的操作，**不会影响**实参指向的对象的内容

### 1.10 Java 的四种引用方式

1.  **强引用**：以 **new 关键字**创建的引用都是强引用，被强引用引用的**对象永远都不会被回收**
2.  **软引用**：以 **SoftRererenc 引用对象**，被弱引用引用的对象只有**在内存空间不足时会被垃圾回收**
3.  **弱引用**：以 **WeakReference 引用对象**，被弱引用引用的对象**一定会被回收**，它**只能存活到下一次垃圾回收**
4.  **虚引用**：**以 PhantomReference 引用对象**，一个对象被引用**引用后不会有任何影响**，也无法通过该引用来获取该对象，**只是其再被垃圾回收时会收到一个系统通知**

### 1.11 JVM 堆内存分配

*   新生代 - 1/3  
    Eden 区 8/10  
    From Survivor 1/10  
    To Survivor 1/10
*   老年代 - 2/3

### 1.12 JVM 垃圾收集器有哪些

串行垃圾回收器（Serial）、并行垃圾回收器（Parallel）、并发清除回收器（CMS）、G1 回收器。

### 1.13 HashCode() 和 equals() 的区别

1.  **不重写**方法时，hashCode() 返回的是**对象的地址值**，equals() 用来**比较两个对象的地址值是否相等**。
2.  **重写**方法时，hashCode() 返回的是**一个 int 整**数，equals() **比较的是两个对象中成员信息是否相同**。
3.  若两个对象 equals(Object obj) 返回 true，则 hashCode（）有必要也返回相同的 int 数。**但是**，若两个对象 hashCode（）返回相同 int 数，则 equals（Object obj）不一定返回 true。

### 1.14 常见的设计模式

1.  单例设计模式（饿汉式：线程安全 、懒汉式：线程不安全）
2.  工厂模式：[spring 中 bean 的实例化方式](https://editor.csdn.net/md?articleId=126193367#517_bean_504)  
    在创建对象时不会**暴露创建逻辑**，并且是通过使用一个共同的接口来指向新创建的对象，可以根据参数的不同返回不同类的实例

### 1.15 Object 类的方法有哪些

1.  getClass()：获取对象类型
2.  hashCode()
3.  equals()
4.  toString()
5.  wait()
6.  finalize（）

### 1.16 抽象类和接口的区别

1.  抽象类只能被继承 extends，接口需要实现 implement，**一个类可以实现多个接口**，但**一个类只能继承一个抽象类**。
2.  抽象类可以有**构造器**，而接口没有构造器
3.  抽象类中可以没有抽象方法，而接口中的方法都是抽象的

### 1.17 final、finally、finalize 的区别

final：修饰声明属性、方法、类  
finally：是异常处理的一部分，表示总是执行  
finalize：当垃圾回收器将要回收对象所占内存之前调用 finalize（）方法来完成最后的处理

2. 多线程
------

### 2.1 谈谈 synchronized 的原理及底层实现

1.  修饰**普通方法**：锁的是当前实例对象
2.  修饰**静态方法**：锁的是当前类的 Class 对象
3.  修饰**代码块**：需要指定一个对象加锁

同步代码块通过 **monitorenter** 和 **monitorexit** 执行来进行加锁。**当线程执行到 monitorenter 的时候要先获得锁，才能执行后面的方法**。**当线程执行到 monitorexit 的时候则要释放锁**。每个对象自身维护着一个被加锁次数的计数器，当计数器不为 0 时，只有获得锁的线程才能再次获得锁

### 2.2 synchronized 与 Lock 的区别

1.  synchronized 是**关键字**，而 Lock 是**接口**
2.  **Lock 不会主动释放锁**，需要手动释放锁
3.  Lock 可以通过 **tryLock() 查看是否加锁成功**，而 synchronized 无法获悉是否加锁成功。

### 2.3 什么是可重入锁

可重入就是说某个线程**已经获得某个锁**，**可以再次获取锁**而不会出现死锁。

可重入锁有 **synchronized**、**ReentrantLock**。

### 2.4 死锁产生的条件（如何解决？怎么判断死锁？）

死锁是指两个或两个以上的进程在执行过程中，**由于竞争资源或者由于彼此通信而造成的一种阻塞的现象**，若无外力作用，它们都将无法推进下去。

1.  **互斥使用**：一个资源每次只能被一个进程使用。
2.  **不可剥夺**: 进程已获得的资源，在末使用完之前，不能强行剥夺。
3.  **请求与保持**：一个进程因请求资源而阻塞时，对已获得的资源保持不放。
4.  **循环等待**: 若干进程之间形成一种头尾相接的循环等待资源关系。

_**解决办法**_：  
1. 破坏不可剥夺：线程在申请不到资源时主动释放掉已有的资源。  
2. 破坏请求与保持：可以一次性给线程申请所有的资源。  
3. 破坏循环等待：将资源线性排列，申请时先申请序号小的，再申请序号大的。

_**判断死锁**_：  
JDK 提供了 **jps 命令**来检测某个 java 进程中心线程的情况。  
方法：1. **使用 jps 命令**查看 java 进程号。 2. 使用 jstack 命令连接上进程号

### 2.5 讲一讲 ThreadLocal

ThreadLocal 叫做**线程变量**，该变量是**当前线程独有的变量**，ThreadLocal 在每个线程中都创建了一个副本，每个线程可以访问自己内部的副本变量。

当**一个线程有多个 threadlocal** 时，ThreadLocalMap 集合可以用来管理多个 ThreadLocal ThreadLocalMap **底层是数组**，**数组的元素是 Entry**，**Entry 的 key 就是 ThreadLocal 的引用**

### 2.6 ThreadLocal 的内存泄漏，如何避免呢？

**Entry 的 key 是弱引用**，**弱引用的特点是，如果这个对象只存在弱引用，那么在下一次垃圾回收的时候必然会被清理掉**。所以 key 会在垃圾回收的时候被回收掉， 而 key 对应的 value 则不会被回收， 这样会导致一种现象：key 为 null，value 有值。key 为空的话 value 是无效数据，久而久之，value 累加就会导致内存泄漏。

**避免**：  
在使用完 ThreadLocal 变量后，**需要我们手动 remove 掉**，防止 ThreadLocalMap 中 Entry 一直保持对 value 的强引用，导致 value 不能被回收

### 2.7 谈谈进程和线程

**进程是资源分配**的基本单位，**线程是程序执行**的基本单位。进程有自己的独立地址空间，每启动一个进程，系统就会为它分配地址空间。一个进程里面可以包含多个线程。

### 2.8 谈一谈 ReentrantLock

ReentrantLock 是可重入锁，底层是通过 AQS 实现的。  
ReentrantLock 共有三个核心内部类：**Sync、NonfairSync、FairSync**。其中 **Sync 继承了 AQS**

AQS 中有三个核心属性：**head**（指向队列头部）、**tail**（指向队列尾部）、**state**（表示状态，修改状态又是通过 CAS 来实现的）

### 2.9 ReentrantLock 和 Synchronized 区别

1.  Synchronized 是关键字，ReentrantLock 是实现类
2.  见 2.2

### 2.10 讲一讲 CAS

CAS 是**比较和替换**，是基于乐观锁的思想实现的。

CAS 应用：原子类（AtomicInteger）中的 incrementAndGet() 方法就是基于 CAS 实现的。

### 2.11 讲一讲 volatile 关键字

volatile 关键字是一个**轻量级的同步机制**。volatile 关键字**可以保证可见性和有序性**，**不能保证原子性**。

1.  可见性：当有一个线程将主内存中的变量值做了修改，其他线程都将马上收到通知，立即获得最新值。
2.  有序性：有序性的保证就是**通过禁止指令重排序来实现的**。**通过加内存屏障**来实现禁止指令重排序

### 2.12 线程池核心参数和工作原理

**核心参数**：

1.  核心线程数
2.  最大线程数
3.  空闲线程存活时间
4.  空闲线程存活时间单位
5.  工作队列
6.  线程工厂
7.  拒绝策略

**工作原理**：

![](https://img-blog.csdnimg.cn/473a0e4c0959468eae4ad1a5e69a4626.png)

### 2.13 wait()、sleep() 和 yield() 方法的区别

1.  **所属类不同**：wait() 是 **Object 类**中的非静态方法，而 sleep()、yield() 是 **Thread 类**中的静态方法
2.  **作用不同**：wait() 用于**线程同步**、sleep() **用于休眠当前线程**，并在指定的时间点被自动唤醒、yield() **临时暂停当前正在执行的线程**，来让有同样优先级的正在等待的线程有机会执行
3.  **资源释放**：**wait() 释放对象锁**；**sleep() 不释放对象锁**，抱着锁睡觉；**yield() 仅释放线程所占用的 CPU**。
4.  被唤醒后的状态不同：  
    wait() 被 notify() 或者 notifyAll() 唤醒后，先进入阻塞状态（先获得锁），然后进入就绪状态；  
    sleep() 被唤醒（或通过 **interrupt() 唤醒**）后，进入就绪状态；  
    yield() 不需要唤醒，一直处于就绪状态，获得 CPU 后继续运行。

**join 方法可以用来插队，有线程在 cpu 运行时，另一个线程使用 join 方法把在运行的线程退回等待状态，自己进入 cpu 运行。**

3. 集合
-----

### 3.1 ArrayList 底层原理

1.  ArrayList 是**基于数组实现**的 List 类。会自动扩容，采用 Array.copyOf() 实现。
2.  **扩容机制**：初始大小是 0，当有数据插入时，**默认大小 DEFAULT_CAPACITY = 10**。后续都是按照 **1.5 倍进行扩容**的。

### 3.2 ArrayList 和 LinkedList 的区别

ArrayList

*   基于**动态数组**的数据结构
*   对于随机访问的 get 和 set，其效率优于 LinkedList
*   对于随机操作的 add 和 remove，ArrayList 不一定比 LinkedList 慢 (ArrayList 底层由于是动态数组，因此并不是每一次 add 和 remove 都需要创建新数组)

LinkedList

*   基于**链表**的数据结构

### 3.3 HashMap 1.7 和 1.8 的区别

**1. 数据结构**

1.7 数据结构为：数组 + 链表。  
1.8 数据结构为： 数组 + 链表 + 红黑树。

**2.put 过程**  
**1.7**：计算 key 的 hash 值，根据 hash 值找到数组的下标。如果当前的位置上有值，则遍历当前位置上所有对象，如果 **key 完全相同的，就覆盖这个值**。如果 key 都不相同，就将要当前值封装成 entry ，加入当前**链表的头结点处（头插）**，如果当前位置没有值，就直接封装成 entry 加入当前位置。

1.8：根据 key 计算 hashcode，然后计算再数组中的下标，如果当前位置上没有值，就直接插入，如果当前位置上有值，就进行遍历，如果存在一个 **key 完全相同，就进行覆盖**，如果不存在就通过**尾插法插入**到链表或者红黑树。如果**链表的长度大于 8 并且数组长度大于 64，就自动转为红黑树。**

**3. 扩容机制**：默认长度为 16，负载因子为 0.75，每次扩容会变为原来的 2 倍，就是 2 的 N 次方

### 3.4 HashMap1.8 为什么使用红黑树

因为在链表模式下，当发生过多的[哈希碰撞](https://editor.csdn.net/md?articleId=126193367#35__49)的时候，链表会越来越长，查询速度会变慢

### 3.5 什么是哈希碰撞，怎么解决？

如果不同的输入得到了同一个哈希值，就发生了 "哈希碰撞"。

解决：

1.  **再次 Hash**
2.  **开放地址法**  
    公式:**Hi=(H(key)+di) MOD m** i=1,2,…,k(k<=m-1)  
    其中，m 为哈希表的表长；di 是产生冲突的时候的增量序列。
3.  **链地址法**：将所有哈希地址相同的记录全部链接在同一链表中。

### 3.6 请你说说 ConcurrentHashMap

ConcurrentHashMap 是一个**线程安全的集合**，它的底层是数组 + 链表 / 红黑树构成的。

*   在 1.7 的时候，采用 segment 数组 + hashEntry 的方式实现的，**锁加在 Segment** 的上面。
*   在 1.8 的时候，采用 CAS 和 synchronized 方式处理并发。以 put 操作为例，CAS 方式确定 key 的数组下标，synchronized 保证链表节点的同步效果。

### 3.7 请你说说 CopyOnWriteArraylist

对于 CopyOnWriteArrayList 来说，**写操作需要加锁**。它并不会直接操作原数组，而是**先复制一个数组再进行操作**，写操作执行结束后在**将复制后的数组赋值给原数组**。CopyOnWriteArrayList 在写操作的同时允许读操作，大大提高了读操作的性能。

### 3.8 HashMap 和 Hashtable 的区别

1.  hashmap 是**线程不安全**的，hashtable 是**线程安全**的。
2.  HashMap 的键值则**都可以为 null**，Hashtable 是**不允许键或值为 null** 的。
3.  HashMap 的**初始容量为：16**，Hashtable **初始容量为：11**，两者的负载因子默认都是：0.75。
4.  HashMap 扩容时是当前容量翻倍，**即: capacity×2**，Hashtable 扩容时是容量翻倍 + 1 **即: capacity×2+1。**

### 3.9 List 与 Set 接口有什么区别

1.  List 元素**有序且可重复**，Set **无序且不可重复**。
2.  List **支持 for 循环和迭代器**遍历，Set **只支持迭代器**遍历。
3.  List **查询元素效率高**，Set **删除和插入元素效率高**。

4. 异常
-----

### 4.1 throw 和 throws 的区别

1.  throw 在**方法体内**使用，throws 在**方法声明上**使用
2.  throw 后面接的是**异常对象**，只能接一个。throws 后面接的是**异常类型**，可以接多个
3.  throw 是在方法中出现不正确情况时，手动来抛出异常，结束方法的，**执行了 throw 语句一定会出现异常**。而 throws 是用来声明当前方法有可能会出现某种异常的，**声明了异常不一定会出现异常**。

### 4.2 异常分类

包括：**Error** 和 **Exception**  
Exception 包括：**编译时异常**和**运行时异常**

**编译时异常**：

1.  ClassNotFoundException：类找不到的异常
2.  SQLException：数据库操作异常
3.  TimeoutException：执行超时异常

**运行时异常**：

1.  NullPointerException: 空指针异常
2.  ArrayIndexOutofBoundsException：数组越界异
3.  ClassCastException：类型转换异常
4.  IllegalArgumentException：非法的参数异常

![](https://img-blog.csdnimg.cn/0cfd03baa84a49379e513eb78d2f8c9d.png)

5.Spring、SpringBoot、SpringMVC
-----------------------------

### 5.1 谈谈 IOC 和 AOP

**IOC**：控制反转。**控制：对象的创建的控制权限；反转：将对象的控制权限交给 spring**。之前我们创建对象时用 new，现在直接从 spring 容器中取，维护对象之间的依赖关系，降低对象之间的耦合度。

**AOP**：面向切面编程。在不改变原有业务逻辑的情况下，**将公共逻辑封装成切面，跟业务逻辑代码分离**。可以减少系统的重复代码和降低模块之间的耦合。

### 5.2 SpringBoot 启动流程

1.  首先从 main 中找到 run() 方法，在执行 run() 方法之前 **new 一个 SpringApplication 对象**
2.  进入 run() 方法，**创建应用监听器**开始监听
3.  然后**加载 SpringBoot 配置环境**，把配置环境加入到监听对象中
4.  然后**加载应用上下文**，当做 run() 方法的返回对象
5.  最后**创建 Spring 容器**，实现 **starter 自动化配置**和 **bean 的实例化**工作

### 5.3 SpringBoot 的自动装配

SpringBoot **通过 @EnableAutoConfiguration 注解**开启自动配置，**加载 spring.factory 中注册的各种 AutoConfiguration 类**，**满足 @Conditional 注解的条件时**，**就实例化**该 AutoConfiguration 类中定义的 Bean，并注入 Spring 容器，即可完成 Springboot 的自动装配。

### 5.4 @Autowired 和 @Resource 注解的区别

1.  @Autowired 是 **spring 提供的注解**，@Resource 是 **JDK 提供的注解**
2.  @Autowied 是只能**按类型注入**，@Resource 默认**按名称注入**，也支持按类型注入。

@Autowied 注解，如果我们想使用按名称装配, 可以**结合 @Qualifier 注解**一起使用

### 5.5 Spring 事务失效原因

1.  bean 对象没有被 spring 容器管理。
2.  方法的访问修饰符不是 public
3.  数据库不支持事务
4.  调用事务方法时，不能用 this.xxx。在 SpringIoC 容器中返回的**调用的对象是代理对象**而不是真实的对象。

### 5.6 说说 BeanFactory 和 FactoryBean 的区别

BeanFactory 是所有 Spring Bean 容器的顶级接口，它为 Spring 容器定义了一套规范，并提供了 **getBean** 方法从容器中**获取指定的 Bean 实例**。

FactoryBean 是一个工厂 Bean，它可以动态去生成某一类型的 Bean 的一个实例。其中 **getObject() 方法就是用来实现动态构建 Bean 的一个过程**。

### 5.7 SpringBoot 自定义注解

自定义注解定义为：@interface。通常使用另外两个元注解定义：

1.  **@Target** ：功能：指明修饰的注解的**使用范围**

*   METHOD: 方法
*   TYPE: 类，接口或者枚举
*   PACKAGE: 包

2.  **@Retention**：指明修饰的注解的**生存周期**

*   RUNTIME： 运行级别保留
*   CLASS: 编译级别保留
*   SOURCE：源码级别保留

### 5.8 SpringMVC 的三层框架

Modle 层（**模型**，数据访问层）、Cotroller 层（**控制**，逻辑控制层）、View 层（**视图**，页面显示层）

### 5.9 SpringMVC 的执行流程

1.  用户向服务器发送请求，请求被 Spring **前端控制 DispatcherServlet** 捕获。
2.  DispatcherServlet 对**请求 URL 进行解析**，**得到请求资源标识符**（URI）。然后根据该 URI，调用 **HandlerMapping** 获得该 Handler 配置的所有相关的对象
3.  DispatcherServlet 根据获得的 Handler，**选择一个合适的 HandlerAdapte**r。开始执行 Handler（Controller), Handler 执行完成后，向 DispatcherServlet **返回一个 ModelAndView 对象**。
4.  DispatcherServlet 根据返回的 ModelAndView，**选择一个适合的 ViewResolver（视图解析器）**。
5.  通过 ViewResolver 结合 Model 和 View，来渲染视图,**DispatcherServlet 将渲染结果返回给客户端**。

### 5.10 说说 Spring Boot 的起步依赖 (starter 自动化配置)

starter 配置，**约定大于配置**，spring boot 将日常企业应用研发中的**各种场景都抽取出来**，做成一个个的 starter（启动器），**starter 中整合了该场景下各种可能用带的依赖**，用户只需要在 Maven 中引入 starter 依赖，spring boot 就能自动扫描到要加载的信息并启动响应的默认配置

### 5.11 bean 的生命周期

1.  通过构造器创建 bean 实例
2.  为 bean 的属性设置值
3.  调用 bean 的初始化方法
4.  当容器关闭时，调用 bean 的销毁方法

### 5.12 bean 的作用域

1.  **singleton 单例模式**（默认）：使用 singleton 定义的 Bean **将只有一个实例**。
2.  **prototype 原型模式**：每次通过容器的 getBean 方法 Bean 时，**都将产生一个新的 Bean 实例**。
3.  **request**：对于每次 HTTP 请求，使用 request 定义的 Bean 都将产生一个新实例
4.  **session**：对于每次 HTTP Session，使用 session 定义的 Bean 都将产生一个新实例。
5.  **global session**：每个全局的 HTTP Session，使用 session 定义的 Bean 都将产生一个新实例。

### 5.13 Springmvc 拦截器和过滤器的区别

1.  拦截器**只对 Controller 请求起作用**，而过滤器可以对几乎**所有请求**起作用
2.  拦截器是基于 **Java 的反射机制**，而过滤器是基于**函数回调**
3.  在 Spring 容器的生命周期中，**拦截器可以多次调用**，而**过滤器只能在容器初始化时被调用一次**

### 5.14 @RestController 和 @Controller 的区别

1.  @RestController 相当于 @Controller 和 @ResponseBody 合在一起的作用；
2.  如果使用 @RestController 注解 Controller 层的话，则返回的是 return 里面的内容，无法返回到指定的页面

### 5.15 @Component 和 @Bean 的区别

1.  作⽤对象不同: @Component 注解**作用于类**，⽽ @Bean 注解**作用于方法**
2.  @Component 通常是**通过类路径扫描自动装配到 Spring 容器中**  
    @Bean 用于**显式声明单个 bean，而不是让 Spring 像上面那样自动执行它**

### 5.16 springboot 中事务如何开启

Spring boot 是默认启动事务的，只需要在（**service 层中添加**）类或者方法上添加 **@Transactional 注解**即可

### 5.17 bean 实例化的三种方式

1.  **使用无参构造方法实例化（xml 配置）**
2.  **静态工厂方式实例化**
3.  **实例工厂方式实例化**

静态工厂方式实例化：通过**静态工厂**创建并返回 Bean。其实质是**将 Bean 对应的类**交给我们自己的**静态工厂管理**。Spring 只是帮我们**调用了**静态工厂创建实例的方法。

实例工厂方式实例化：通过**实例工厂**创建并返回 Bean，其实质就是把**创建实例的工厂类**和**调用工厂类的方法**的过程也交由 Spring 管理。

6.Mybatis
---------

### 6.1 Mybatis 的三种传值方式

1.  **使用 @Param 注解**  
    接口内的抽象方法

```
/**
接口内的抽象方法
**/
public abstract User selectUser(@Param("id") int userId);
```

映射文件的 sql 语句

```
<!--
  映射文件的sql语句
-->
 <select id="selectUser" resultType="User">
        select * from user where userId = #{id};
    </select>
```

2.  **使用对象传值**

```
/**
接口内的抽象方法
**/
public abstract List<User> selectUser1(User user);
```

```
<!--
  映射文件的sql语句
-->
<select id="selectUser1" resultType="User">
        select * from user where userId = #{UserId} or sex = #{sex}
    </select>
```

3.  **使用 Map 传值**

```
/**
接口内的抽象方法
**/
public abstract List<User> selectUserByMap(Map<String,Object> map);
```

```
<!--
  映射文件的sql语句
-->
<select id="selectUserByMap" resultType="User">
        select * from user where userId = #{id} or sex = #{sex}
    </select>
```

```
Map<String,Object> map = new HashMap<>();
        map.put("id",37);
        map.put("sex","男");
```

### 6.2 Mybatis 的一级缓存和二级缓存

**一级缓存**：**作用域默认是 SqlSession**。**Mybatis 默认开启一级缓存**。 在同一个 SqlSession 中，执行相同的查询 SQL，**第一次会去数据库进行查询，并写到缓存中**；**第二次以后则直接去一级缓存中取**。当执行的 SQL 查询中间**发生了增删改的操作**，mybatis **会把 SqlSession 的缓存清空**。

**二级缓存**：**作用域是 nameSpace**。Mybatis 需要**手动设置启动二级缓存**。一个会话，查询一条数据，这个数据会被放在当前会话的一级缓存中；**如果会话被关闭了**，**一级缓存汇总的数据会被保存到二级缓存**。新的会话查询信息就会参照二级缓存。

7.Mysql
-------

### 7.1 索引查询失效的几个情况

**1.like 以 % 开头，索引无效；当 like 前缀没有 %，后缀有 % 时，索引有效。**  
**2、or 语句前后没有同时使用索引。**  
当 or 左右查询字段只有一个是索引，该索引失效，只有当 or 左右查询字段均为索引时，才会生效  
![](https://img-blog.csdnimg.cn/4ad452d45d9e4dbcafe38348eb9b4243.png)  
**3、如果列类型是字符串，那一定要在条件中将数据使用引号引用起来，否则不使用索引**  
**4、在索引列上使用 IS NULL 或 IS NOT NULL 操作。**  
**5、在索引字段上使用 <>，!=。**

### 7.2 Mysql 的事务特性 及事务的传播方式

**1. 原子性**：事务最小的执行单位，不允许分割。事务的原子性确保动作要么全部执行，要么全部不执行。  
**2. 一致性**：执行事务的前后，数据保持一致。例如转账的业务中，无论事务是否成功，转账者和收款人的总额应该是不变的。  
**3. 隔离性**：并发访问数据库时，一个用户的事务不应该被其他事务所影响，各并发事务之间数据库是独立的。  
**4. 持久性**：一个事务被提交后，它对数据库中数据的改变是持久的，即使数据库发生故障也不应该对其有影响。

1.  **PROPAGATION_REQUIRED**：如果当前没有事务，就创建一个新事务，如果当前存在事务，就加入该事务，这是最常见的选择，也是 Spring 默认的事务传播行为。(**required 需要，没有新建，有就加入**)
2.  **PROPAGATION_SUPPORTS**：支持当前事务，如果当前存在事务，就加入该事务，如果当前不存在事务，就以非事务执行。（**supports 支持，有则加入，没有就不管了，非事务运行**）
3.  **PROPAGATION_MANDATORY**：支持当前事务，如果当前存在事务，就加入该事务，如果当前不存在事务，就抛出异常。（**mandatory 强制性，有则加入，没有异常**）
4.  **PROPAGATION_REQUIRES_NEW**：创建新事务，无论当前存不存在事务，都创建新事务。（**requires_new 需要新的，不管有没有，直接创建新事务**）
5.  **PROPAGATION_NOT_SUPPORTED**：以非事务方式执行操作，如果当前存在事务，就把当前事务挂起。（**not supported 不支持事务，存在就挂起**）
6.  **PROPAGATION_NEVER**：以非事务方式执行，如果当前存在事务，则抛出异常。（**never 不支持事务，存在就异常**）
7.  **PROPAGATION_NESTED**：如果当前存在事务，则在嵌套事务内执行。如果当前没有事务，则按 REQUIRED 属性执行。（**nested 存在就在嵌套的执行，没有就找是否存在外面的事务，有则加入，没有则新建**）

### 7.3 Mysql 的事务隔离级别

**1. 读取未提交**（READ-UNCOMMITTED）：最低的隔离级别，允许读取尚未提交的数据变更，**可能造成脏读、不可重复读、幻读。**

**2. 读取已提交**（READ-COMMITTED）：允许读取并发事务已经提交的数据，**可以避免脏读，但是可能造成不可重复、幻读。**

**3. 可重复读**（REPEATABLE-READ）：_**mysql 默认隔离级别**_。对同一字段多次读取的结果都是一致的，除非本身事务修改，**可以避免脏读和不可重复读，但是可能造成幻读。**

**4. 可串行化**（SERIALIZABLE）：最高的隔离级别，**完全服从 ACID 的隔离级别**，所以的事务依次执行，**可以避免脏读、不可重复读、幻读。**

### 7.4 Mysql 数据库常用的锁

**1. 行级锁**  
行锁是指加锁的时候锁住的是表的某一行或多行记录，多个事务访问同一张表时，只有被锁住的记录不能访问，其他的记录可正常访问；**行级锁并不是直接锁记录，而是锁索引**。  
**特点**：_粒度小，加锁比表锁麻烦，不容易冲突，相比表锁支持的并发要高；_

**2. 表级锁**  
表锁是指上锁的时候锁住的是整个表，当下一个事务访问该表的时候，必须等前一个事务释放了锁才能进行对表进行访问；  
**特点：** _粒度大，加锁简单，容易冲突；_

**3. 共享锁**  
共享锁又称**读锁**，简称 S 锁。当一个事务对数据**加上读锁之后**，其他事务**只能对该数据加读锁，而无法对数据加写锁**，直到所有的读锁释放之后其他事务才能对其进行加写锁。 加了共享锁之后，无法再加排它锁，这也就可以避免读取数据的时候会被其它事务修改，从而导致重复读问题。

**4. 排他锁**  
排他锁又称**写锁**，简称 X 锁；当一个事务对数据**加上写锁之后**，其他事务将**不能再为数据加任何锁**，直到该锁释放之后，其他事务才能对数据进行加锁。加了排他锁之后，其它事务就无法再对数进行读取和修改，所以也就避免了脏写和脏读的问题。

**5. 记录锁**  
记录锁也属于**行锁中的一种**，只不过记录锁的范围只是表中的某一条记录，记录锁是说事务在加锁后**锁住的只是表的某一条记录**。

**6. 间隙锁**  
间隙锁属于**行锁中的一种**，间隙锁是在事务加锁后其**锁住的是表记录的某一个区间**，当表的相邻 ID 之间出现空隙则会形成一个区间，遵循左开右闭原则。

**7. 临键锁**  
临键锁也属于行锁的一种，总结来说它就是**记录锁和间隙锁的组合**，临键锁会把**查询出来的记录锁住**，**同时也会把该范围查询内的所有间隙空间也会锁住**，**再之它会把相邻的下一个区间也会锁住**。

### 7.5 Mysql 与 Redis 的区别

1.  在类型上，mysql 是关系型数据库，而 redis 是缓存数据库；
2.  在作用上，mysql 用于持久化的存储数据到硬盘，而 redis 用于存储使用较为频繁的数据到缓存中；

**扩展：什么是关系型数据库？什么是非关系型数据库？**

答：**关系型数据库**，是指采用了关系模型来组织数据的数据库，其以行和列的形式存储数据，以便于用户理解，关系型数据库这一系列的行和列被称为表，一组表组成了数据库。  
**非关系型数据库**，NoSQL，泛指非关系型的数据库。区别于关系数据库，它们**不保证关系数据的 ACID 特性**。

### 7.6 Innodb 和 Myisam 的区别

1.  **InnoDB 支持事务，MyISAM 不支持**，这一点是非常之重要。事务是一种高级的处理方式，如在一些列增删改中只要哪个出错还可以回滚还原，而 MyISAM 就不可以了。
2.  innodb 支持**外键**，而 myisam **不支持外键**。
3.  innodb **默认表锁**，使用**索引检索条件时是行锁**，而 myisam 是**表锁**。
4.  innodb 是**聚簇索引**，，myisam 是**非聚簇索引**，索引和数据是分离的。
5.  innodb 和 myisam 的索引都是基于 b + 树，但他们具体实现不一样，innodb 的 b + 树的**叶子节点是存放数据的**，myisam 的 b + 树的**叶子节点是存放指针的**。

### 7.7 请你说说 InnoDB 的 MVCC 机制（难点）

MVCC 中文全程叫**多版本并发控制**，是数据库引擎实现中常用的**处理读写冲突的手段**，目的在于**提高数据库高并发场景下的吞吐性能**。

MVCC 底层核心原理：**隐藏字段（事务 id trx_id 和 回滚指针 roll_pointer）、Undo Log 版本链 、 ReadView**

MVCC 只在**读已提交（每次 Select 都会获取一次 ReadView）和可重复读（只在第一次 Select 时获取一次 ReadView**）两个隔离级别下工作

![](https://img-blog.csdnimg.cn/07b990b413bb4812a13ca81868b27966.png)

### 7.8 数据库索引为什么使用 B + 数

索引的数据结构会被**存储在磁盘中**，每次查询都需要到磁盘中访问，对于红黑树，树的高度可能会非常的高，会进行很多次的磁盘 IO，效率会非常低，**B + 树的高度一般为 2-4**，也就是说在最坏的条件下，也最多进行 **2 到 4 次磁盘 IO**，这在实际中性能时非常不错的

### 7.9 讲一讲 sql 优化

1.  查询 SQL 尽量不要使用 select *，而是具体字段
2.  避免在 where 子句中使用 or 来连接条件
3.  使用 varchar 代替 char （**varchar 按数据内容实际长度存储**，存储空间小 /**char 按声明大小存储**，不足补空格）
4.  优化 like 语句

### 7.10 count(*) 和 count(1) 的区别

*   如果表多个列并且**没有主键**，则 count（1） 的执行效率优于 count（*）
    
*   如果表只有一个字段，则 select count（*）最优
    

### 7.11 mysql 索引

MySQL 索引是一种帮助**快速查找数据的数据结构**，可以把它理解为书的目录，通过索引能够快速找到数据所在位置。场景的索引数据结构有：**Hash 表**（通过 hash 算法快速定位数据，但不适合范围查询，因为需要每个 key 都进行一次 hash）、**二叉树**（查找和修改效率都比较高），但是在 **InnoDB 引擎中使用的索引是 B+Tree**，相较于二叉树，**B+Tree 这种多叉树，更加矮宽**，更适合存储在磁盘中。使用索引增加了数据查找的效率

### 7.12 left join、right join、inner join 的区别

1.  inner join: 内连接, **显示两个表中有联系的所有数据**
2.  left join: 左链接, **以左表为参照**, 显示所有数据, 右表中没有则以 null 显示
3.  right join: 右链接, **以右表为参照**, 显示所有数据, 左表中没有则以 null 显示

### 7.13 为什么 mysql 默认隔离级别设置为 RR（可重复读）

因为在主从复制过程中，是 ** 基于 binlog（二进制日志）** 实现的。在 mysql5.0 之前，**binlog 只支持 statement 格式**（记录的是修改 SQL 语句），而这种格式在读已提交 (Read Commited) 这个隔离级别下主从复制是有问题的，**可能会出现从机执行的顺序与主机不一致**。

解决方式：1） 隔离级别设为可重复读 (Repeatable Read), 在该隔离级别下引入间隙锁。2）将 binglog 的格式修改为 row 格式，此时是基于行的复制。

### 7.14 MySQL 普通索引和唯一索引区别

普通索引：就是各类索引中最为普通的索引。其特点是**允许出现相同的索引内容，允许空（null）值**  
唯一索引：就是**不可以出现相同的索引内容**，但是**可以为空（null）值**

1. **查询过程**：

*   对于普通索引来说，查找到满足条件的第一个记录 后，需要查找下一个记录，直到碰到第一个不满足条件的记录。
*   对于唯一索引来说，由于索引定义了唯一性，查找到第一个满足条件的记录后，就会停止继续检索。

2.  更新过程

### 7.15 常见 mysql 的慢查询优化方式

1.  在配置文件中设置慢查询时间，开启慢查询日志。
2.  直接分析 mysql 慢查询日志 , 利用 explain 关键字执行 SQL 查询语句，来分析 sql 慢查询语句

### 7.16 mysql 主从复制

mysql 主从复制是指将主服务器的数据复制到一个或多个从服务器上。

作用: **数据备份、提高性能、读写分离**

步骤：

1.  主服务器（master）把数据更改记录到二进制日志（binlog）中。
2.  从服务器（slave）把主服务器的二进制日志复制到自己的中继日志（relay log）中。
3.  从服务器重做中继日志中的日志, 应用到自己的数据库上, 以达到数据的最终一致性

### 7.17 当前读与快照读的区别

1.  当前读：就是它读取的是 **记录的最新版本**，读取时还要保证其他并发事务不能修改当前记录，会对读取的记录进⾏**加锁**。  
    eg： _update、insert 、delete、select lock in share mode(共享锁),select for update_
    
2.  快照读：**不加锁的 select 操作**就是快照读。  
    **快照读的前提是隔离级别不能为：未提交读和串行化级别**，因为未提交读总是读取最新的数据⾏，⽽不是符合当前事务版本的数据⾏。⽽串⾏化则会对所有读取的⾏都加锁
    

### 7.18 sql 语句执行顺序

from->where->group by->having->select->order by->limit

8.Redis
-------

### 8.1 谈谈 Redis 的应用场景

1.  缓存  
    热点数据缓存（例如报表、明星出轨），对象缓存、全页缓存、可以提升热点数据的访问数据。
2.  分布式锁  
    详见：[8.2 如何利用 Redis 实现一个分布式锁](https://editor.csdn.net/md?articleId=126193367#82_Redis_48)

### 8.2 如何利用 Redis 实现一个分布式锁？

**1. SETNX + EXPIRE**  
这个方案中，setnx 和 expire 两个命令分开了，「不是原子操作」。如果执行完 setnx 加锁，正要执行 expire 设置过期时间时，进程 crash 或者要重启维护了，那么这个锁就 “长生不老” 了，「别的线程永远获取不到锁啦」。

**2. SETNX + value 值是（系统时间 + 过期时间）**  
这个方案的优点是，巧妙移除 expire 单独设置过期时间的操作，把「过期时间放到 setnx 的 value 值」里面来。解决了方案一发生异常。

**3. 使用 Lua 脚本 (包含 SETNX + EXPIRE 两条指令)**  
实际上，我们还可以使用 Lua 脚本来保证原子性（包含 setnx 和 expire 两条指令）

**4.SET 的扩展命令（SET EX PX NX）**  
除了使用，使用 Lua 脚本，保证 SETNX + EXPIRE 两条指令的原子性，我们还可以巧用 Redis 的 SET 指令扩展参数！（SET key value[EX seconds][PX milliseconds][NX|XX]），它也是原子性的！

> SET key value[EX seconds][PX milliseconds][NX|XX]  
> NX : 表示 key 不存在的时候，才能 set 成功，也即保证只有第一个客户端请求才能获得锁，而其他客户端请求只能等其释放锁，才能获取。  
> EX seconds : 设定 key 的过期时间，时间单位是秒。  
> PX milliseconds: 设定 key 的过期时间，单位为毫秒  
> XX: 仅当 key 存在时设置值

但是呢，这个方案还是可能存在问题：**「锁被别的线程误删」**。假设线程 a 执行完后，去释放锁。但是它不知道当前的锁可能是线程 b 持有的（线程 a 去释放锁时，有可能过期时间已经到了，此时线程 b 进来占有了锁）。那线程 a 就把线程 b 的锁释放掉了，但是线程 b 临界区业务代码可能都还没执行完呢。

**5.SET EX PX NX + 校验唯一随机值**  
既然锁可能被别的线程误删，那我们给 value 值设置一个标记当前线程唯一的随机数，在删除的时候，校验一下，不就 OK 了嘛。

参考链接地址：[Redis 实现分布式锁的 7 种方案，及正确使用姿势！](https://www.cnblogs.com/wangyingshuo/p/14510524.html)

### 8.3 Redis 的基本数据类型及底层数据结构

**1.String**  
字符串对象的值底层都是由**简单动态字符串**实现的

```
get <key>							查询对应键值
set <key> <value>			添加键值对
append <key> <value>	将给定的<value>追加到原值的末尾
strlen <key>					获取值的长度
senx <key> <value>		只有在key 不存在时设置key的值
incr <key>						将key中存储的数字值增1, 只能对数字值操作，如果为空，新增值为1
decr <key>						将key中存储的数字值减1, 只能对数字之操作，如果为空,新增值为-1
incrby/decrby <key> 	将key中存储的数字值增减，自定义步长
mset <key1> <value1> <key2> <value2>		同时设置一个或多个key-value对
mget <key1> <key2> <key3>								同时获取一个或多个value
msetnx <key1> <value1> <key2> <value2>	同时设置一个或多个key-value对，当且仅当所有给定的key都不存在
getrange <key> <起始位置> <结束位置>			 获得值的范围,类似java中的substring
setrange <key> <起始位置> <value>		用<value>覆盖<key>所存储的字符串值，从<起始位置>开始
setex <key> <过期时间> <value>			设置键值的同时，设置过去时间，单位秒
getset <key> <value>					 以新换旧,设置了新值的同时获取旧值
```

**2.list**  
底层数据结构是**双向链表**

```
常用操作命令
lpush/rpush <key> <value1> <value2>  	从左边/右边插入一个或多个值。
lpop/rpop <key>							从左边/右边吐出一个值。值在键在，值光键亡。
rpoplpush <key1> <key2>  				从<key1>列表右边吐出一个值，插到<key2>列表左边
lrange <key> <start> <stop>				按照索引下标获得元素(从左到右)
lindex <key> <index>					按照索引下标获得元素(从左到右)
llen <key>								获得列表长度
linsert <key> before <value> <newvalue>		在<value>的后面插入<newvalue> 插入值
lrem <key> <n> <value>								从左边删除n个value(从左到右)
```

**3.set**  
底层数据结构是 **hash + 整数数组**

**4.zset**  
底层数据结构是 **ziplist + 跳表**

**5.hash**  
底层数据结构是 **ziplist+hash**

### 8.4 Redis 如何与数据库保持双写一致性

先更新数据库再删除缓存，若有错误需要重试

### 8.5 Redis 的持久化策略

1.  **RDB**：在**指定的时间间隔内**，**将内存中的数据集的快照写入磁盘**，文件名 dump.rdb 适合大规模的数据恢复，对数据库的完整性和一致性要求不是很高，**如果数据库意外 down 掉，就会失去最后一次快照的所有修改**。
2.  **AOF**：**以日志的形式记录每个写操作，只允许追加文件，不允许改写文件**，redis 启动时会读取这个文件，并从头到尾执行一遍，以此来恢复数据，文件名 appendonly.aof。完整性较高，但是会对磁盘持续的进行 IO，代价太大。

### 8.6 说说缓存穿透、击穿、雪崩以及如何避免

**缓存穿透**：**指大量请求访问一个本身不存在的数据**，使得请求直达存储层，导致负载过大。  
_处理手段_：使用过滤器进行拦截，若请求的数据不存在则直接返回空值。

**缓存击穿**：**指一份热点数据缓存失效，突然涌入大量的访问请求**，使得请求直达存储层，导致负载过大。  
_处理手段_：1. **永不过期**：对热点数据不设置过期时间 2. **加互斥锁**，当一个线程访问该数据时，另一个线程只能等待，这个线程访问之后，缓存中的数据将被重建，届时其他线程就可以从缓存中取值

**缓存雪崩**：**大量数据同时过期，缓存层无法提供服务**，使得请求直达存储层，导致负载过大。  
_处理手段_：1. **永不过期**：对热点数据不设置过期时间 2. **避免数据同时过期**，设置随机过期时间

### 8.7 redis 是单线程还是多线程，为什么？

对于**键值对读写是单线程的**，而对于**持久化、异步删除是依赖其他线程来执行的**。事实上他底层并不是单线程的

1.  采用单线程则避免了线程间的切换和加锁过程，减小了消耗。
2.  redis 采用 [IO 多路复用机制](https://editor.csdn.net/md?articleId=126193367#88_IO_789)，使其能够处理并发请求。

### 8.8 什么是 IO 多路复用机制？

**select / poll / epoll** 这是三个多路复用接口

1.  **select/poll**  
    select 实现多路复用的方式与 poll 的方式类似：将已连接的 Socket 都放到一个 **FD（文件描述符）集合**，然后调用 select 函数**将文件描述符集合拷贝到内核里**，让内核来检查是否有网络事件产生，通过**遍历**文件描述符集合的方式，当检查到有事件产生后，将此 Socket 进行**标记**， 接着再把**整个文件描述符集合拷贝回用户态里**，然后用户态还需要**再通过遍历**的方法找到可读或可写的 Socket，然后再对其处理。
    
2.  **epoll**  
    epoll 在内核里使用**红黑树**来跟踪进程所有待检测的文件描述符，**减少了内核和用户空间大量的数据拷**，提高了效率。  
    epoll 内核里维护了一个**链表来记录就绪事件**，当某个 socket 有事件发生时，通过回调函数内核会将其加入到这个就绪事件列表中
    

9.MQ
----

### 9.1 为什么要使用 MQ

**1. 实现异步处理**  
有时候我们会遇到这样的场景, 用户在客户端提交了一个请求, 后端处理这个请求的业务相对比较复杂, 如果这个请求使用的是同步调用, 客户端就会出现发送请求后过了很久才相应的情况, 这对用户体验来说是十分致命的. 如果说用户并不关心请求是否处理, 对于一些耗时的非事务性的业务处理, 我们可以使用 mq 异步请求的方式, 将处理信息放入队列, 由后端监听队列自行处理, 在将消息存入队列后直接返回客户端相应, 加快响应速度.

**2. 实现分布式系统之间的应用解耦**  
在分布式系统中, 经常会出现一个服务会有多个消费端调用, 而且可能每个消费方需要接入的逻辑不一致问题。将消息写入消息队列，需要消息的系统自己从消息队列中订阅，实现解耦。

**3. 流量削峰**  
例如秒杀活动, 可能在短时间内会有很大请求同时到后端, 如果后端对每个请求都执行业务操作, 例如查询数据库和写数据库, 会造成服务器压力过大, 同时, 在同一时间进行大量数据库操作, 可能会出现数据异常, 我们可以使用 mq 实现缓冲, 将所有请求先放入消息队列中, 服务端每次处理业务先从消息队列获取.

### 9.2 如何解决 MQ 消息丢失问题？

1.  开启生产者消息手动确认机制
2.  开启消息持久化和队列持久化
3.  开启消费者消息手动确认机制

10.Dubbo
--------

11. 计算机网络
---------

### 11.1 TCP 和 UDP 的区别

1.  TCP 是**面向连接**的，UDP 是**无连接**的。
2.  TCP 是**可靠传输**的，UDP 是**不可靠传输**的。
3.  TCP 是是面向**字节流**传输的，UDP 是面向**报文**传输的。

### 11.2 TCP 三次握手和四次挥手过程

**通道的建立 ------- 三次握手：**  
（1）在建立通道时，客户端首先要向服务端**发送一个 SYN 同步信号**。  
（2）服务端在接收到这个信号之后会向客户端**发出 SYN 同步信号**和 **ACK 确认信号**。  
（3）当服务端的 ACK 和 SYN 到达客户端后，客户端与服务端之间的这个 “通道” 就会被建立起来。

**通道的关闭——四次挥手：**  
（1）在数据传输完毕之后，客户端会向服务端**发出一个 FIN 终止信号**。  
（2）服务端在收到这个信号之后会向客户端**发出一个 ACK 确认信号**。  
（3）如果**服务端此后也没有数据发给客户端时**服务端会向客户端发送一个 **FIN 终止信号**。  
（4）**客户端在收到这个信号之后会回复一个确认信号**，在服务端接收到这个信号之后，服务端与客户端的通道也就关闭

### 11.3 七层网络协议

### ![](https://img-blog.csdnimg.cn/bfa51de4756e4b0c8cdc7edebe522c77.png)

### 11.3 Http 和 Https 详解

[Http 和 Https 详解](https://blog.csdn.net/lingxu6/article/details/124738027)

### 11.4 Http 状态码

1.  200：成功
2.  301：永久性重定向，表示资源已被分配了新的 URL
3.  302：临时性重定向，表示资源临时被分配了新的 URL
4.  404：服务器无法根据客户端的请求找到资源
5.  500：服务器内部错误

### 11.5 TCP 粘包

粘包是指发送方发送的若干包数据到接收方接收时粘成一包

**原因**：

1.  当连续发送数据时，为了提高效率，tcp 协议会将**较小的内容拼接成大的内容**，**一次性发送到服务器端**，因此造成粘包
2.  当发送内容较大时，由于服务器端方法中的 **buffer_size 较小**，不能一次性完全接收全部内容，因此在下一次请求到达时，接收的内容依然是上一次没有完全接收完的内容，因此造成粘包现象。

**解决**：  
在每次使用 tcp 协议发送数据流时, 在**开头标记一个长度信息**, 并**固定该报文长度**，当服务端接收数据，判断**客户端发送数据流长度**, **并只接收该长度字节数据**, 就可以实现拆包, 完美解决 tcp 粘包问题.

12.Linux
--------

### 12.1 linux 常用命令

1.  打包指令：tar[主选项 + 辅选项] 文件或目录
2.  vim
3.  cd
4.  pwd: 显示用户当前所在的目录
5.  ls: 对于目录，该命令列出该目录下的所有子目录与文件
6.  grep: 用于查找文件里符合条件的字符串
7.  ps: 用来列出系统中当前正在运行的那些进程
8.  ping : 检测是否与主机连通

13.JWT
------

![](https://img-blog.csdnimg.cn/ed0106d3a91d475b8ec2e4d5414f3a5a.png)

1.  前端通过 Web 表单将自己的用户名和密码发送到后端的接口
2.  后端核对用户名和密码成功后，将用户信息作为 JWT Payload (负载)，将其与 Header（头部）分别进行编码拼接后，进行签名形成一个 JWT(Token) 返回给前端。
3.  以 token 为 key，用户信息为 value，存入到 redis 中。
4.  前端收到 后端返回的 token 后，将其存储在 HTTP 请求的头信息 Authorization 字段里面