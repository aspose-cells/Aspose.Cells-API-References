---
title: "WorkbookDesigner.SetJsonDataSource"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo WorkbookDesigner. Imposta il valore della stringa json come fonte di dati dei marcatori intelligenti"
type: docs
url: /it/net/aspose.cells/workbookdesigner/setjsondatasource/
---
## WorkbookDesigner.SetJsonDataSource method

Imposta il valore della stringa JSON come origine dati degli smart marker.

```csharp
public void SetJsonDataSource(string name, string json)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| name | String | Il nome della tabella. Se il valore di JSON rappresenta un oggetto, potrebbe essere null. |
| json | String | Il valore della stringa Json. |

### Esempi

```csharp
using System;
using System.IO;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookDesignerMethodSetJsonDataSourceWithStringStringDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            
            // Accedi al primo foglio di lavoro
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Aggiungi un marcatore di esempio nella cella A1
            worksheet.Cells["A1"].PutValue("&=$DataSource.Name");
            
            // Crea il designer di cartella di lavoro
            WorkbookDesigner designer = new WorkbookDesigner();
            designer.Workbook = workbook;
            
            // Dati JSON di esempio
            string jsonData = "{\"Name\":\"John Doe\",\"Age\":30,\"City\":\"New York\"}";
            
            // Imposta la fonte di dati JSON
            designer.SetJsonDataSource("DataSource", jsonData);
            
            // Elabora i marcatori
            designer.Process();
            
            // Salva la cartella di lavoro
            workbook.Save("output.xlsx");
        }
    }
}
```

### Vedi anche

* class [WorkbookDesigner](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


