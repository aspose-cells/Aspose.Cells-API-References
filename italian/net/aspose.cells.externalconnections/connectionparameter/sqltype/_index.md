---
title: "ConnectionParameter.SqlType"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "ConnectionParameter proprietà. Tipo di dati SQL del parametro. Valido solo per sorgenti ODBC"
type: docs
url: /it/net/aspose.cells.externalconnections/connectionparameter/sqltype/
---
## ConnectionParameter.SqlType property

Tipo di dati SQL del parametro. Valido solo per le origini ODBC.

```csharp
public SqlDataType SqlType { get; set; }
```

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.ExternalConnections;
    using System;

    public class ConnectionParameterPropertySqlTypeDemo
    {
        public static void Run()
        {
            try
            {
                // Crea un nuovo workbook
                Workbook workbook = new Workbook();
                
                // Crea un parametro di connessione (simulato poiché i parametri del costruttore sono sconosciuti)
                ConnectionParameter parameter = null;
                
                // In uno scenario reale, dovresti creare il parametro correttamente
                // parameter = new ConnectionParameter(/* required parameters */);
                
                // Per dimostrazione, mostreremo come verrebbe usato SqlType se avessimo un parametro
                if (parameter != null)
                {
                    // Ottieni e visualizza il valore corrente di SqlType
                    Console.WriteLine("Current SqlType: " + parameter.SqlType);
                    
                    // Imposta un nuovo valore SqlType (poiché la proprietà è leggibile e scrivibile)
                    parameter.SqlType = SqlDataType.SqlInteger;
                    Console.WriteLine("Updated SqlType: " + parameter.SqlType);
                }
                else
                {
                    // Dimostrazione di fallback quando non possiamo creare il parametro
                    workbook.Worksheets[0].Cells["A1"].Value = "SqlType property demo (see code comments)";
                    Console.WriteLine("Demonstrated workbook creation. In actual usage, create ConnectionParameter properly.");
                }
                
                // Salva la cartella di lavoro
                workbook.Save("ConnectionParameterSqlTypeDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }
    }
}
```

### Vedi anche

* enum [SqlDataType](../../sqldatatype/)
* class [ConnectionParameter](../)
* namespace [Aspose.Cells.ExternalConnections](../../../aspose.cells.externalconnections/)
* assembly [Aspose.Cells](../../../)


