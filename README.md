# static
public class Player { static int onlinePlayers; 
    Player() {
        onlinePlayers++;
    }

public static void main(String[] args) { 
Player p1 = new Player();
Player p2 = new Player();
Player p3 = new Player(); 
System.out.println("Online oyuncular : " + Player.onlinePlayers);    
  }
}

public class Course {    
String name;
    String code;
    String prefix;
int note; 
public Course(String name, String code, String prefix) 
 { 
this.name = name; 
this.code = code; 
this.prefix = prefix; 
this.note = 0;     }

public static void courseList() { 
String[] courseList = {"fizik", "kimya", "matematik"}; 
for (String courseName : courseList) 
 {            
System.out.println(courseName);
        }
    }

public static void main(String[] args) { Course c1 = new Course("Mat-101" , "MAT" , "MAT");         Course.courseList();
    }
}
