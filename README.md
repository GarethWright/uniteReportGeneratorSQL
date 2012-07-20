Enable 3rd Party developments to retrieve raw sql from Capita's Unit-e Report Generator.

Add as a reference and import com.garethwright.UniteReportsMSSQL

You now have access to the function getReportSQL which takes two parameters.

getReportSQL(byVal ReportReference as String, byVal ConnectionString as string) as string

e.g Dim connString as string = "Data Source=unitesql\live;Initial Catalog=LIVE;Persist Security Info=True;User ID=user;Password=password;"

Dim SelectCommand as string = getReportSQL("gw.TotalEnrolments1112", connString)

Enjoy!