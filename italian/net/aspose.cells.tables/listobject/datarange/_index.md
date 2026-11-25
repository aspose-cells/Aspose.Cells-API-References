---
title: "ListObject.DataRange"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà ListObject. Ottiene l'intervallo di dati della tabella"
type: docs
url: /it/net/aspose.cells.tables/listobject/datarange/
---
## ListObject.DataRange property

Ottiene l'intervallo di dati della Tabella.

```csharp
public Range DataRange { get; }
```

### Esempi

```csharp
using System;
using System.Text;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ListObjectPropertyDataRangeDemo
    {
        public static void Run()
        {
            Encoding.RegisterProvider(CodePagesEncodingProvider.Instance);
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi dati di esempio
            worksheet.Cells["A1"].PutValue("ID");
            worksheet.Cells["B1"].PutValue("Name");
            worksheet.Cells["A2"].PutValue(1);
            worksheet.Cells["B2"].PutValue("John");
            worksheet.Cells["A3"].PutValue(2);
            worksheet.Cells["B3"].PutValue("Mary");

            // Crea un ListObject (Tabella)
            int tableIndex = worksheet.ListObjects.Add(0, 0, 2, 1, true);
            Aspose.Cells.Tables.ListObject table = worksheet.ListObjects[tableIndex];
            table.DisplayName = "EmployeeTable";

            // Ottieni l'intervallo di dati della tabella
            Aspose.Cells.Range dataRange = table.DataRange;

            // Dimostra l'uso di DataRange
            Console.WriteLine("Table Data Range: " + dataRange.Address);
            Console.WriteLine("Row Count: " + dataRange.RowCount);
            Console.WriteLine("Column Count: " + dataRange.ColumnCount);

            // Aggiungi una formula all'ultima colonna usando DataRange
            string formula = "=CONCATENATE(\"ID-\", [ID])";
            int lastColIndex = dataRange.ColumnCount - 1;
            dataRange[0, lastColIndex].PutValue("FormattedID");
            for (int i = 1; i < dataRange.RowCount; i++)
            {
                dataRange[i, lastColIndex].Formula = formula;
            }

            // Salva la cartella di lavoro
            workbook.Save("ListObjectDataRangeDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [Range](../../../aspose.cells/range/)
* class [ListObject](../)
* namespace [Aspose.Cells.Tables](../../../aspose.cells.tables/)
* assembly [Aspose.Cells](../../../)


