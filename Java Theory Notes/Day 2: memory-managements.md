# Memory Management
- Memory: The term Memory can be defined as a collection of data in a specific format. It is used to store instructions and process data. The memory comprises a large array or group of words or bytes, each with its own location.
 
 In java memory allocation happens in two types:
 - Stack Memory
 - Heap Memory


![Screenshot from 2022-11-20 11-30-07](https://user-images.githubusercontent.com/66300439/202888294-bfa3f882-c985-4bdf-92ba-a6c54cac3391.png)


 Now for example we have: 
 a = 10
 This a is known as reference variable and 10 is known as the object.
 Variables or fuction calls are stored in the stack and the object(means the value of the object) is stored in the heap memory.
 a is going to be pointing towards 10. a will be pointing to the address of the object. Every object has its own address in the ram.
 
 ## What actually is reference variable?
 - Reference variable is just like a variable which is used to point to the object/value. 
 
 Now lets see a real life exapmle of it. 
 
 Suppose "Soumali" which is an object of this world (i.e the earth). And his name is Rohan, that means name = "Soumali". Now Soumali is a actual object of the class human. Now this object is in the heap memory, and we want to call this object how shall we do it? by its name, which is the reference variable. 
 Now my mom doesn't call me soumali she calls me by the name "sonu". Now soumali and sonu are the same person (the same object). Now if soumali is giving a party which means sonu is also giving a party. 
 
Which means:
 <strong>
 - More than one reference variable can point towards the same object.
 - If any one of the reference variable change the object, the original object is going to change. And its going to be changed for all.
 </strong>
 
 In future we will see about some concepts like pass by reference value. 
 Now see if a = [1,3,5,9] and b = a, interanlly it will be 
 
 ![WhatsApp Image 2022-11-20 at 11 53 54 AM](https://user-images.githubusercontent.com/66300439/202888959-16b7ee54-eef0-4e58-abaa-fc732b3bad9a.jpeg)

now if we change a[0] = 99 so now a is also modified which means b will also be modified. Hence the object is modified. 

## Garbage Collection
- Garbage collection in Java is the process by which Java programs perform automatic memory management. 
- The main objective of Garbage Collector is to free heap memory by destroying unreachable objects.

### How it works:
Suppose Soumali has a boyfriend and he calls her baby. So baby and Soumali are the same person. Now a new girl comes named "Tanya" and Soumali's bf break up and is now with Tanya and also calles her baby. So now the baby is ponting towards tanya. All the changes made by baby will be modified to the object Tanya. Now Soumali gets upset that she's not the baby anymore and she went to forest and gives up her name. So now there is no soumali. This human is living alone with no name. Now this person is an object with no reference variable. This object (person) will be removed from the memory when 
garbage collection hits. In java we have something called garbage collection, ie, all the object which doesn't have the reference variable will be removed from the memory automatically. 

![WhatsApp Image 2022-11-20 at 12 18 36 PM](https://user-images.githubusercontent.com/66300439/202889684-06a4a55d-6cb0-4a99-8e25-d775c86dab36.jpeg)


For example:
a = 10
a points towards 10 now

a = 30
so now a points towards 30

No one is pointing towards 10 so garbage collection will come and remove it.

### Advantages of Garbage Collection in Java

1. It makes java memory-efficient because the garbage collector removes the unreferenced objects from heap memory.
2. It is automatically done by the garbage collector(a part of JVM), so we don’t need extra effort.
