# Week 3 Homework- Raneem Safi

## *The Difference between _Task_ and _Thread_ in C#*
-  The **_Thread_** class is used for **creating** and **manipulating** a thread in Windows. And represent an actual thread in operating system, and it’s not used frequently
-  A **_Task_** is a higher level, it uses **Threadpool**, represents some **_asynchronous_** operation and in **_parallel_**, it is part of the [Task Parallel Library](http://msdn.microsoft.com/en-us/library/dd460717%28v=vs.110%29.aspx), a set of APIs for running tasks asynchronously and in parallel.
1.  A **_Task_** will by default use the **_Threadpool_**, which saves resources as creating threads can be expensive. A **_Threadpool_** is.. a pool of threads, which are ready to carry out instructions (if they are no occupied of course).
2.  The **_Task_** can return a result. There is no direct mechanism to return the result from a **_Thread._**
4.	**_Task_** supports cancellation through the use of cancellation tokens. But **_Thread_** doesn't.
5.	A **_Task_** can have multiple processes happening at the same time. **_Thread_**s can only have one task running at a time.
6.	We can easily implement Asynchronous using ’async’ and ‘await’ keywords with **_Task_**
7.	A new Thread()is not dealing with **_Thread_** pool thread, whereas **_Task_** does use thread pool.
 <br />Figures always describe what words cannot, please have a look
### <br /> **Task:** 
 ![Task](https://github.com/raneem87/test/blob/master/task.gif)
 ### <br />  **Thread:** 
![Thread](https://github.com/raneem87/test/blob/master/thread.gif) 
<br /><br />

## *What is Extention Package*
- An **_Extension Pack_** is a set of extensions that can be installed together. 
- Extension Packs enable you to easily share your favorite extensions with other users or bundle a set of extensions together for a particular scenario.
### **.NET Core Extension Pack**
- This extension pack packages some of the most popular .NET Core related extensions.
- It includes: 
  - C# Productivity
  - Testing Tools
  - NuGet & Build Tools
  - ASP.NET Core Productivity
  - Misc
  - Some other extensions you may need (Optional)
  - Other manual setup (Optional)
  
<br /> In addition to the Extention Pachage, while i'm searching for it, I found it interesting to mention the Extention method as well.
- A C# **_Extension_** method allows developers to extend functionality of an existing type without  creating a new derived type, recompiling, or otherwise modifying the original type.
- C# **_Extension_** method is a special kind of static method that is called as if it was an instance methods on the extended type.
- C# **_Extension_** method is a static method of a static class, where the "this" modifier is applied to the first parameter. 
- The type of the first parameter will be the type that is extended.
- **_Extension_** methods are only in scope when you explicitly import the namespace into your source code with a using directive.

```
1.	using System;  
2.	using System.Text;  
3.	  
4.	namespace ClassLibExtMethod  
5.	{  
6.	    public class Class1  
7.	    {  
8.	        public string Display()  
9.	        {  
10.	            return ("I m in Display");  
11.	        }  
12.	  
13.	        public string Print()  
14.	        {  
15.	            return ("I m in Print");  
16.	        }  
17.	    }  
18.	} 
```
### <br /> Extention
![Extention](https://github.com/raneem87/test/blob/master/extenstion.gif)
