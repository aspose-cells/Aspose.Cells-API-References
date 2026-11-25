---
title: "ListObject.Resize"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo ListObject. Ridimensiona l'intervallo dell'oggetto elenco"
type: docs
url: /it/net/aspose.cells.tables/listobject/resize/
---
## ListObject.Resize method

Ridimensiona l'intervallo dell'oggetto elenco.

```csharp
public void Resize(int startRow, int startColumn, int endRow, int endColumn, bool hasHeaders)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| startRow | Int32 | L'indice della riga iniziale del nuovo intervallo. |
| startColumn | Int32 | L'indice della colonna iniziale del nuovo intervallo. |
| endRow | Int32 | L'indice della riga finale del nuovo intervallo. |
| endColumn | Int32 | L'indice della colonna finale del nuovo intervallo. |
| hasHeaders | Booleano | Indica se questa tabella ha intestazioni. |

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Tables;

namespace AsposeCellsExamples
{
    public class ListObjectMethodResizeWithInt32Int32Int32Int32BooleanDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Aggiungi dati di esempio
            for (int i = 0; i < 10; i++)
            {
                worksheet.Cells[i, 0].PutValue("Item " + (i + 1));
                worksheet.Cells[i, 1].PutValue(i * 10);
            }

            // Crea un oggetto elenco
            int index = worksheet.ListObjects.Add(0, 0, 5, 1, true);
            ListObject listObj = worksheet.ListObjects[index];
            listObj.TableStyleType = TableStyleType.TableStyleLight2;

            // Ridimensiona l'oggetto elenco
            listObj.Resize(0, 0, 9, 1, true);

            // Salva la cartella di lavoro
            workbook.Save("ResizedListObject.xlsx");
        }
    }
}
```

### Vedi anche

* class [ListObject](../)
* namespace [Aspose.Cells.Tables](../../../aspose.cells.tables/)
* assembly [Aspose.Cells](../../../)


