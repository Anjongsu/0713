# 0713
## ㅁ
###### ㅁ

- 1
- 2

<hr/>
<pre><code>
## DB Connection
package DBPKG;

import java.sql.Connection;
import java.sql.DriverManager;
import java.sql.SQLException;

public class dbconnection {

	//DB연결
public static Connection getConnection() throws ClassNotFoundException, SQLException {
Class.forName("oracle.jdbc.driver.OracleDriver");
Connection dbcon = null;
		
dbcon = DriverManager.getConnection("jdbc:oracle:thin:@localhost:1521:system", "hrd", "1234");
return dbcon;


}
	
	//쿼리문실행

}
</code></pre>
