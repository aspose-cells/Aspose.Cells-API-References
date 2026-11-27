---
title: "Cells.ExportDataTableAsString"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Cells‑metod. Exporterar data i Cells‑samlingen till ett DataTable‑objekt"
type: docs
url: /sv/net/aspose.cells/cells/exportdatatableasstring/
---
## ExportDataTableAsString(int, int, int, int) {#exportdatatableasstring}

Exporterar data i [`Cells`](../)‑samlingen till ett DataTable‑objekt.

```csharp
public DataTable ExportDataTableAsString(int firstRow, int firstColumn, int totalRows, 
    int totalColumns)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| firstRow | Int32 | Radnumret för den första cellen som ska exporteras. |
| firstColumn | Int32 | Kolumnnumret för den första cellen som ska exporteras. |
| totalRows | Int32 | Antal rader att importera. |
| totalColumns | Int32 | Antal kolumner att importera. |

### Returvärde

Exporterad DataTable‑objekt.

### Anmärkningar

All data i [`Cells`](../)-samlingen konverteras till strängar.

### Exempel

```csharp
using System;
using System.Data;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodExportDataTableAsStringWithInt32Int32Int32Int32Demo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            
            // Åtkomst till det första kalkylbladet
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Lägg till exempeldata i celler
            cells["A1"].PutValue("Column1");
            cells["B1"].PutValue("Column2");
            cells["A2"].PutValue("Value1");
            cells["B2"].PutValue("Value2");

            // Exportera data till DataTable som strängar
            DataTable dataTable = cells.ExportDataTableAsString(0, 0, 2, 2);

            // Visa den exporterade datan
            Console.WriteLine("Exported DataTable:");
            foreach (DataColumn column in dataTable.Columns)
            {
                Console.Write(column.ColumnName + "\t");
            }
            Console.WriteLine();
            
            foreach (DataRow row in dataTable.Rows)
            {
                foreach (var item in row.ItemArray)
                {
                    Console.Write(item.ToString() + "\t");
                }
                Console.WriteLine();
            }
        }
    }
}
```

### Se även

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## ExportDataTableAsString(int, int, int, int, bool) {#exportdatatableasstring_1}

Exporterar data i [`Cells`](../)‑samlingen till ett DataTable‑objekt.

```csharp
public DataTable ExportDataTableAsString(int firstRow, int firstColumn, int totalRows, 
    int totalColumns, bool exportColumnName)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| firstRow | Int32 | Radnumret för den första cellen som ska exporteras. |
| firstColumn | Int32 | Kolumnnumret för den första cellen som ska exporteras. |
| totalRows | Int32 | Antal rader att importera. |
| totalColumns | Int32 | Antal kolumner att importera. |
| exportColumnName | Boolean | Anger om data i den första raden exporteras till kolumnnamnet i DataTable. |

### Returvärde

Exporterad DataTable‑objekt.

### Anmärkningar

All data i [`Cells`](../)-samlingen konverteras till strängar.

### Exempel

```csharp
using System;
using System.Data;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodExportDataTableAsStringWithInt32Int32Int32Int32BooleanDemo
    {
        public static void Run()
        {
            // Skapa en arbetsbok med exempeldata
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Lägg till exempeldata i celler
            worksheet.Cells["A1"].PutValue("Name");
            worksheet.Cells["B1"].PutValue("Age");
            worksheet.Cells["A2"].PutValue("John");
            worksheet.Cells["B2"].PutValue(30);
            worksheet.Cells["A3"].PutValue("Alice");
            worksheet.Cells["B3"].PutValue(25);

            // Exportera data till DataTable
            int maxRow = worksheet.Cells.MaxDataRow + 1;
            int maxCol = worksheet.Cells.MaxDataColumn + 1;
            DataTable dataTable = worksheet.Cells.ExportDataTableAsString(0, 0, maxRow, maxCol, true);

            // Visa den exporterade datan
            foreach (DataRow row in dataTable.Rows)
            {
                foreach (DataColumn col in dataTable.Columns)
                {
                    Console.Write(row[col] + "\t");
                }
                Console.WriteLine();
            }
        }
    }
}
```

### Se även

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


