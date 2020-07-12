# 0713
## ㅁ
###### ㅁ

- 1
- 2

<hr/>

## DB Connection

<pre><code>
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


<hr/>

## joinForm

<pre><code>

<%@ page language="java" contentType="text/html; charset=UTF-8"
	pageEncoding="UTF-8"%>

<head>
<meta http-equiv="Content-Type" content="text/html; charset=UTF-8">
<title>회원가입</title>
</head>
<h1>회원가입</h1>
<form method="get" action="joinAction.jsp" >
<table border=1>

<tr><th>아이디</th><td><input name="id"></td></tr>
<tr><th>패스워드</th><td><input name="pass"></td></tr>
<tr><th>성명</th><td><input name="name"></td></tr>
<tr><th>나이</th><td><input name="age"></td></tr>
<tr><th>이메일</th><td><input name="email"></td></tr>
<tr><th>전화번호</th><td><input name="phone"></td></tr>
<tr><th>주소</th><td><input name="address"></td></tr>
<tr><td colspan=2><input type="submit" value="가입"></td></tr>

</table>
</form>
</code></pre>
