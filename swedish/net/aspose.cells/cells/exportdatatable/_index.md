---
title: "Cells.ExportDataTable"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Cells‑metod. Exporterar data i Cells‑samlingen till ett DataTable‑objekt"
type: docs
url: /sv/net/aspose.cells/cells/exportdatatable/
---
## ExportDataTable(int, int, int, int) {#exportdatatable}

Exporterar data i [`Cells`](../)‑samlingen till ett DataTable‑objekt.

```csharp
public DataTable ExportDataTable(int firstRow, int firstColumn, int totalRows, int totalColumns)
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

Om du använder den här metoden för att exportera ett datablock, se till att data i en kolumn har samma datatyp. Använd annars metoden [`ExportDataTableAsString`](../exportdatatableasstring/) istället.

### Exempel

```csharp
using System;
using System.Data;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodExportDataTableWithInt32Int32Int32Int32Demo
    {
        public static void Run()
        {
            // Skapa en arbetsbok med exempeldata
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Lägg till exempeldata i celler
            worksheet.Cells["A1"].PutValue("Name");
            worksheet.Cells["B1"].PutValue("Age");
            worksheet.Cells["C1"].PutValue("City");
            
            for (int i = 1; i <= 5; i++)
            {
                worksheet.Cells[i, 0].PutValue($"Person {i}");
                worksheet.Cells[i, 1].PutValue(20 + i);
                worksheet.Cells[i, 2].PutValue($"City {i}");
            }

            // Exportera data till DataTable (börjar från rad 0, kolumn 0, med 5 rader och 3 kolumner)
            DataTable dataTable = worksheet.Cells.ExportDataTable(0, 0, 5, 3);

            // Visa den exporterade datan
            Console.WriteLine("Exported DataTable:");
            foreach (DataRow row in dataTable.Rows)
            {
                Console.WriteLine($"{row[0]}, {row[1]}, {row[2]}");
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

## ExportDataTable(int, int, int, int, bool) {#exportdatatable_2}

Exporterar data i [`Cells`](../)‑samlingen till ett DataTable‑objekt.

```csharp
public DataTable ExportDataTable(int firstRow, int firstColumn, int totalRows, int totalColumns, 
    bool exportColumnName)
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

### Exempel

```csharp
using System;
using System.Data;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodExportDataTableWithInt32Int32Int32Int32BooleanDemo
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

            // Exportera data till DataTable (första raden innehåller rubriker)
            DataTable dt = worksheet.Cells.ExportDataTable(0, 0, 3, 2, true);

            // Visa den exporterade datan
            Console.WriteLine("Exported DataTable:");
            foreach (DataRow row in dt.Rows)
            {
                Console.WriteLine($"{row["Name"]}, {row["Age"]}");
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

## ExportDataTable(int, int, int, int, ExportTableOptions) {#exportdatatable_1}

Exporterar data i [`Cells`](../)‑samlingen till ett DataTable‑objekt.

```csharp
public DataTable ExportDataTable(int firstRow, int firstColumn, int totalRows, int totalColumns, 
    ExportTableOptions options)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| firstRow | Int32 | Radnumret för den första cellen som ska exporteras. |
| firstColumn | Int32 | Kolumnnumret för den första cellen som ska exporteras. |
| totalRows | Int32 | Antal rader att importera. |
| totalColumns | Int32 | Antal kolumner att importera. |
| alternativ | ExportTableOptions | Alla exporttabellalternativ |

### Returvärde

Exporterad DataTable‑objekt.

### Exempel

```csharp
using System;
using System.Data;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodExportDataTableWithInt32Int32Int32Int32ExportTablDemo
    {
        public static void Run()
        {
            // Skapa en arbetsbok
            Workbook workbook = new Workbook();
            Cells cells = workbook.Worksheets[0].Cells;

            // Ange värde och format för cell A1
            cells["A1"].PutValue(1.23356);
            Style style = cells["A1"].GetStyle();
            style.Custom = "0.00";
            cells["A1"].SetStyle(style);

            // Skapa exportalternativ
            ExportTableOptions etOpt = new ExportTableOptions();
            etOpt.ExportColumnName = false;
            etOpt.ExportAsString = true;

            // Exportera med CellStyle-formatstrategi
            etOpt.FormatStrategy = CellValueFormatStrategy.CellStyle;
            DataTable dt1 = cells.ExportDataTable(0, 0, 1, 1, etOpt);
            Console.WriteLine("CellStyle format: " + dt1.Rows[0][0].ToString());

            // Exportera med ingen formatstrategi
            etOpt.FormatStrategy = CellValueFormatStrategy.None;
            DataTable dt2 = cells.ExportDataTable(0, 0, 1, 1, etOpt);
            Console.WriteLine("None format: " + dt2.Rows[0][0].ToString());

            // Exportera med DisplayStyle-formatstrategi
            etOpt.FormatStrategy = CellValueFormatStrategy.DisplayStyle;
            DataTable dt3 = cells.ExportDataTable(0, 0, 1, 1, etOpt);
            Console.WriteLine("DisplayStyle format: " + dt3.Rows[0][0].ToString());
        }
    }
}
```

### Se även

* class [ExportTableOptions](../../exporttableoptions/)
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


