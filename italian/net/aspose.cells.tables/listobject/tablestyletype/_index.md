---
title: "ListObject.TableStyleType"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà ListObject. Ottiene lo stile di tabella incorporato"
type: docs
url: /it/net/aspose.cells.tables/listobject/tablestyletype/
---
## ListObject.TableStyleType property

Ottiene e lo stile di tabella incorporato.

```csharp
public TableStyleType TableStyleType { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Tables;

namespace AsposeCellsExamples
{
    public class ListObjectPropertyTableStyleTypeDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            
            // Accedi al primo foglio di lavoro
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Aggiungi dati di esempio alle celle
            for (int i = 0; i < 10; i++)
            {
                for (int j = 0; j < 5; j++)
                {
                    worksheet.Cells[i, j].PutValue($"Data {i+1}-{j+1}");
                }
            }
            
            // Ottieni la raccolta di oggetti elenco
            ListObjectCollection tables = worksheet.ListObjects;
            
            // Aggiungi una tabella
            int index = tables.Add(0, 0, 9, 4, true);
            ListObject table = tables[0];
            
            // Imposta lo stile della tabella
            table.TableStyleType = TableStyleType.TableStyleDark2;
            
            // Salva la cartella di lavoro
            workbook.Save("TableStyleDemo.xlsx");
        }
    }
}
```

### Vedi anche

* enum [TableStyleType](../../tablestyletype/)
* class [ListObject](../)
* namespace [Aspose.Cells.Tables](../../../aspose.cells.tables/)
* assembly [Aspose.Cells](../../../)


