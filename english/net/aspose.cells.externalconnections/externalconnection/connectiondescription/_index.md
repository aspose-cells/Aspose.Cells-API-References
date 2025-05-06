---
title: ExternalConnection.ConnectionDescription
second_title: Aspose.Cells for .NET API Reference
description: ExternalConnection property. Specifies the user description for this connection
type: docs
url: /net/aspose.cells.externalconnections/externalconnection/connectiondescription/
---
## ExternalConnection.ConnectionDescription property

Specifies the user description for this connection

```csharp
public string ConnectionDescription { get; set; }
```

### Examples

```csharp
// Called: Console.WriteLine(&amp;quot;Description info: &amp;quot; + workbook.DataConnections[i].ConnectionDescription);
[Test]
        public void Property_ConnectionDescription()
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

* class [ExternalConnection](../)
* namespace [Aspose.Cells.ExternalConnections](../../../aspose.cells.externalconnections/)
* assembly [Aspose.Cells](../../../)


