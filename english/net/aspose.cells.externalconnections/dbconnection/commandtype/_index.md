---
title: DBConnection.CommandType
second_title: Aspose.Cells for .NET API Reference
description: DBConnection property. Specifies the OLE DB command type. 1. Query specifies a cube name 2. Query specifies a SQL statement 3. Query specifies a table name 4. Query specifies that default information has been given and it is up to the provider how to interpret. 5. Query is against a web based List Data Provider
type: docs
url: /net/aspose.cells.externalconnections/dbconnection/commandtype/
---
## DBConnection.CommandType property

Specifies the OLE DB command type. 1. Query specifies a cube name 2. Query specifies a SQL statement 3. Query specifies a table name 4. Query specifies that default information has been given, and it is up to the provider how to interpret. 5. Query is against a web based List Data Provider.

```csharp
public override OLEDBCommandType CommandType { get; set; }
```

### Examples

```csharp
// Called: Console.WriteLine(&amp;quot;Command type: &amp;quot; + dbConn.CommandType);
[Test]
        public void Property_CommandType()
        {
            string filePath = Constants.PivotTableSourcePath + @&quot;NET52065_&quot;;

            Workbook workbook = new Workbook(filePath + &quot;RRI_Template_DataSQL.xlsb&quot;);
            int dbCount = 0;
            int dataModelCount = 0;
            for (int i = 0; i &lt; workbook.DataConnections.Count; i++)
            {
                Aspose.Cells.ExternalConnections.ExternalConnection externalConnection = workbook.DataConnections[i];
                if (externalConnection is DBConnection)
                {
                    DBConnection dbConn = externalConnection as DBConnection;
                    Console.WriteLine(&quot;Connection Name: &quot; + dbConn.Name);
                    Console.WriteLine(&quot;Info: &quot; + dbConn.ConnectionInfo);
                    Console.WriteLine(&quot;Command type: &quot; + dbConn.CommandType);
                    Console.WriteLine(&quot;Command: &quot; + dbConn.Command);
                    Console.WriteLine(&quot;Description: &quot; + dbConn.ConnectionDescription);
                    Console.WriteLine(&quot;Id: &quot; + dbConn.Id);
                    Console.WriteLine(&quot;Credentials: &quot; + dbConn.CredentialsMethodType);
                    Console.WriteLine(&quot;Type: &quot; + dbConn.SourceType);
                    Console.WriteLine(&quot;########################&quot;);
                    dbCount++;
                }
                else if (externalConnection is DataModelConnection)
                {
                    DataModelConnection dataModelConnection = externalConnection as DataModelConnection;
                    Console.WriteLine(&quot;Connection Name: &quot; + dataModelConnection.Name);
                    Console.WriteLine(&quot;Description info: &quot; + dataModelConnection.ConnectionDescription);
                    Console.WriteLine(&quot;Connection ID: &quot; + dataModelConnection.Id);
                    Console.WriteLine(&quot;Credentials: &quot; + dataModelConnection.CredentialsMethodType);
                    Console.WriteLine(&quot;Type: &quot; + dataModelConnection.SourceType);
                    Console.WriteLine(&quot;########################&quot;);
                    dataModelCount++;

                }
                else
                {

                    Console.WriteLine(&quot;Connection Name: &quot; + workbook.DataConnections[i].Name);
                    Console.WriteLine(&quot;Description info: &quot; + workbook.DataConnections[i].ConnectionDescription);
                    Console.WriteLine(&quot;Connection ID: &quot; + workbook.DataConnections[i].Id);
                    Console.WriteLine(&quot;Credentials: &quot; + workbook.DataConnections[i].CredentialsMethodType);
                    Console.WriteLine(&quot;Type: &quot; + workbook.DataConnections[i].SourceType);
                    Console.WriteLine(&quot;########################&quot;);
                }
            }

            Assert.AreEqual(dbCount, 1);
            Assert.AreEqual(dataModelCount, 3);
        }
```

### See Also

* enum [OLEDBCommandType](../../oledbcommandtype/)
* class [DBConnection](../)
* namespace [Aspose.Cells.ExternalConnections](../../../aspose.cells.externalconnections/)
* assembly [Aspose.Cells](../../../)


