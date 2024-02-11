/**
 * You can edit, run, and share this code.
 * play.kotlinlang.org
 */
fun main() {
//     student_count = 5000;
    
//     println("Hello, world!!!")
    val myListOfNames = listOf("Class A","Class B","Class C","Class  D")
    
    val myMutableList = mutableListOf(12,34,45,123)
    myMutableList.add(214)
    println(myMutableList)
    println("Number of elements ${myMutableList.size}")
    println("Number of elements ${myMutableList[1]}")
    println("Index of element \"two\" ${myMutableList.indexOf(45)}")
    
    val myNewList = mutableListOf<String>()
    myNewList.add("Student A")
    myNewList.add("Student B")
    myNewList.add("Student C")
    myNewList.add("Student D")
    myNewList.add("Student E")
    
    for (i in 1..10){
        myNewList.add(i,"Hey $i")
    }
    
    println(myNewList)
    
    
    
    
    
    val mySet = setOf("Course A","Course B","Course C")
    val myMutableSet = mutableSetOf(1,3,4,5)
    myMutableSet.add(123)
    println ("mySet ${mySet}")
    
    
    val secretMap = mapOf("Up" to 1, "Down" to 2, "Left" to 3, "Right" to 4)
    val myMutableSecretMap = mutableMapOf("One" to 1, "Two" to 2, "Three" to 3)
	myMutableSecretMap["Fourt"]=4	
    
    if("Up" in secretMap) println ("Yes is in!")
    if(4 in secretMap.values) println ("Yes is in!")
    
    
    
    myListOfNames.forEach{
        print(" Mahidol: $it | ")
    }
    
//     for (item in myListOfNames){
//         print(" Mahidol: $item | ")
//     }


//     ge100(40,10000,60)
}

// func getEnglevel(score_eng:Int){
//     val level = 0
//     if(score_eng>100){
//         level =2
//     }else (score_eng>200){
//         level =2
//     }else (score_eng>300){
//         level =3
//     }else (score_eng>400){
//         level =4
//     }
//     return level
// }

fun ge100(total_count:Int, total_course: Int, multipleOf:Int){
    
//     val eng_level = getEnglevel(300)
    
    for (i in total_count..total_course){
        if (i%multipleOf == 0){
           	
            println("$i SEC $i is multiple of $multipleOf")
        }
    }
}

fun sayHello(){
    print("this is function")
    
    for (i in 1..100){
       
        if (i%3 ==0){
            print("$i is mulit 2")
        }
    }
}

