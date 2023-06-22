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



Eğer sınıfa ait metotlardan bir yada birden fazlasının önüne "static" deyimi yazılırsa, o metotlar sınıf metodu olurlar. Sınıf metotlarının en önemli özelliği, ilgili sınıfa ait nesne oluşturmadan sınıf metodu çağırılabilir. Bir sınıf değişkeninin, henüz nesne oluşturulmasa da bellekte fiziksel olarak yer kapladığını söylemiştik. Bir sınıf metodunun ise nesne oluşturulmadan, sınıf adı üzerinden çağrılabildiğini belirttik. Bu durumda, nesne var olmadan çağrılabilecek olan sınıf metotları, nesne var olmadan bellekte var olamayan olgu değişkenlerine erişmesi olanaklı değildir. Benzer şekilde, nesne var olmadan bellekte var olan sınıf değişkenleri üzerinde işlem yapan yöntemlerin, nesne var olmadan çağrılabilmeleri gerekir.



public class Course {     String name;
    String code;
    String prefix;
int note; 
public Course(String name, String code, String prefix) { this.name = name; this.code = code; this.prefix = prefix; this.note = 0;     }

public static void courseList() { String[] courseList = {"fizik", "kimya", "matematik"}; for (String courseName : courseList) {             System.out.println(courseName);
        }
    }

public static void main(String[] args) { Course c1 = new Course("Mat-101" , "MAT" , "MAT");         Course.courseList();
    }
}
