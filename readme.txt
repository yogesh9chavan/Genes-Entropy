-To open the code and run the application, follow the below steps:

1. Open Eclipse
2. Click on File menu and then Open file menu option
3. Open entropy.java file
4. Run the program


-To run the application directly double click on entropyCRsfs.exe

-Sample results are in sampleResults.txt

-Notes and snapshots are in notes.doc



fun accumulate f a [] = a 

 
   | accumulate f a (x::xs) = accumulate f (f(x,a)) xs;
    
   

 
fun reverse lis = accumulate (fn (x,a) => x + (a * 10)) 0 lis;


	
 reverse [1,2,3,4];




fun accumulate f a [] = a 


    | accumulate f a (x::xs) = accumulate f (f(x,a)) xs;
    
   

 
fun reverse lis = accumulate (fn (x,a) => x::a) [] lis;



reverse [1,2,3,4];


fun accumulate f a [] = a 

 
   | accumulate f a (x::xs) = accumulate f (f(x,a)) xs;
    


    
fun all p lis = accumulate (fn (x,a) => if p x andalso a = true then   true    else  false ) true lis;



all (fn x => (x=4)) [4,4,9,4];


fun accumulate f a [] = a 

  
  | accumulate f a (x::xs) = accumulate f (f(x,a)) xs;
    

    

fun xx lis = accumulate (fn (x,a) => 1) 1 lis;

xx ["ss", "dd"];
