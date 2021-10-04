public static Connection connect()
{
try {
        Class.forName("com.mysql.cj.jdbc.Driver");
        //System.out.println("Loaded driver");
        Connection con = DriverManager.getConnection("jdbc:mysql://localhost/mysql?user=root&password=edureka");
        //System.out.println("Connected to MySQL");
        return con;
 } 
 catch (Exception ex) {
        ex.printStackTrace();
 }
return null;
}