![Java programming language](https://img.shields.io/badge/Java-programming%20language-brightgreen)
# JHelper-Library-Java
-----------------------
This library is  built with Java programming language by  dev. Mohamed Hossam (Mohamed Kandeel) to help developer to make swing easier.
this contain some method to help accessing database and change UI of JFrame this is free library so you can use it by download it and add it to your project.
to add library to your project follow these instructions:-
***********************************
* open your project on Netbeans<br>
* make sure you added JDBC to your project<br>
* right click on Libraries<br>
* choose Add JAR/Folder<br>
* select the library<br>
* add these imports to your code:<br>
    - import com.mkandeel.JHelper.Tools;<br>
	- import com.mkandeel.ui.*;<br>
	- import com.mkandeel.db.database;<br>
* use the library in your project<br>
**********************************
1- To Connect with database you should make port for MySQL 3308 and to connect to DB use the following code for example:
```
public static void main(String[] args) {
        database.setDbname("DBName");
	...
    }
```
2- if you make a JFrame and you want to open it you can use this code:
```
public class MyClass {    
    public static void main(String[] args) {
        ...
        Frame frm = new Frame();
        frm.setTitle("my frame");
        Tools.open(frm, MyClass.class, "icon.png", 255,255,255);
    }
}
```
open method takes six parameters:-<br>
* your JFrame object
* your working class
* path of JFrame icon and its extension
* next three parameter is the RGB code for your form background color<br>

3- if you want to insert, update, delete from database you can use this example of code:-
```
String sql = "write your sql query (insert, update, delete)";
database.RunNonQuery(sql);
```
do not forget that this library is designed and built to help all developer so if you faced any problem or you have any suggestions to improve it or adding more functions please contact with developer via this gmail:-
mohamed.kandeel7799@gmail.com
Thank you.
