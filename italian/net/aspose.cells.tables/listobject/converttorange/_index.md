---
title: "ListObject.ConvertToRange"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo ListObject. Converte la tabella in intervallo"
type: docs
url: /it/net/aspose.cells.tables/listobject/converttorange/
---
## ConvertToRange() {#converttorange}

Converti la tabella in intervallo.

```csharp
public void ConvertToRange()
```

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Tables;

namespace AsposeCellsExamples
{
    public class ListObjectMethodConvertToRangeDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            
            // Accedi al primo foglio di lavoro
            Worksheet sheet = workbook.Worksheets[0];
            
            // Aggiungi dati di esempio
            sheet.Cells["A1"].PutValue("ID");
            sheet.Cells["B1"].PutValue("Name");
            sheet.Cells["A2"].PutValue(1);
            sheet.Cells["B2"].PutValue("John");
            sheet.Cells["A3"].PutValue(2);
            sheet.Cells["B3"].PutValue("Mary");
            
            // Crea un oggetto elenco
            int index = sheet.ListObjects.Add("A1", "B3", true);
            ListObject listObject = sheet.ListObjects[index];
            
            Console.WriteLine("Before conversion - ListObject exists: " + (listObject != null));
            
            // Converti l'oggetto elenco in intervallo
            listObject.ConvertToRange();
            
            Console.WriteLine("After conversion - ListObjects count: " + sheet.ListObjects.Count);
            
            // Salva la cartella di lavoro
            workbook.Save("ListObjectConversion.xlsx");
        }
    }
}
```

### Vedi anche

* class [ListObject](../)
* namespace [Aspose.Cells.Tables](../../../aspose.cells.tables/)
* assembly [Aspose.Cells](../../../)

---

## ConvertToRange(TableToRangeOptions) {#converttorange_1}

Converti la tabella in intervallo.

```csharp
public void ConvertToRange(TableToRangeOptions options)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| opzioni | TableToRangeOptions | le opzioni quando si converte una tabella in intervallo. |

### Esempi

```csharp
using Aspose.Cells;
using Aspose.Cells.Tables;

namespace AsposeCellsExamples
{
    public class ListObjectMethodConvertToRangeWithTableToRangeOptionsDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Crea dati di esempio
            for (int i = 0; i < 5; i++)
            {
                worksheet.Cells[0, i].PutValue($"Column {i + 1}");
                for (int row = 1; row < 5; row++)
                {
                    worksheet.Cells[row, i].PutValue(row * (i + 1));
                }
            }

            // Crea tabella
            int tableIndex = worksheet.ListObjects.Add(0, 0, 4, 4, true);
            ListObject table = worksheet.ListObjects[tableIndex];
            table.ShowTotals = true;
            table.ListColumns[0].TotalsCalculation = Aspose.Cells.Tables.TotalsCalculation.Sum;

            // Converti la tabella in intervallo con opzioni
            TableToRangeOptions options = new TableToRangeOptions();
            options.LastRow = 4;
            table.ConvertToRange(options);

            workbook.Save("TableToRangeWithOptions.xlsx");
        }
    }
}
```

### Vedi anche

* class [TableToRangeOptions](../../tabletorangeoptions/)
* class [ListObject](../)
* namespace [Aspose.Cells.Tables](../../../aspose.cells.tables/)
* assembly [Aspose.Cells](../../../)


