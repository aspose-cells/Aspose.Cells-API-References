---
title: "TableStyleCollection.DefaultPivotStyleName"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà TableStyleCollection. Ottiene e imposta il nome dello stile predefinito della tabella pivot"
type: docs
url: /it/net/aspose.cells.tables/tablestylecollection/defaultpivotstylename/
---
## TableStyleCollection.DefaultPivotStyleName property

Ottiene e imposta il nome dello stile predefinito della tabella pivot.

```csharp
public string DefaultPivotStyleName { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Tables;

namespace AsposeCellsExamples
{
    public class TableStyleCollectionPropertyDefaultPivotStyleNameDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            
            // Accedi alla raccolta degli stili di tabella
            TableStyleCollection tableStyles = workbook.Worksheets.TableStyles;
            
            // Visualizza il nome dello stile pivot predefinito
            Console.WriteLine("Default Pivot Style: " + tableStyles.DefaultPivotStyleName);
            
            // Modifica lo stile pivot predefinito
            tableStyles.DefaultPivotStyleName = "PivotStyleDark2";
            
            // Verifica la modifica
            Console.WriteLine("Updated Default Pivot Style: " + tableStyles.DefaultPivotStyleName);
            
            // Salva la cartella di lavoro
            workbook.Save("output.xlsx");
        }
    }
}
```

### Vedi anche

* class [TableStyleCollection](../)
* namespace [Aspose.Cells.Tables](../../../aspose.cells.tables/)
* assembly [Aspose.Cells](../../../)


