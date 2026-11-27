---
title: "ListObject.PutCellFormula"
second_title: "Aspose.Cells för .NET API‑referens"
description: "ListObject metod. Placera formeln i cellen i tabellen"
type: docs
url: /sv/net/aspose.cells.tables/listobject/putcellformula/
---
## PutCellFormula(int, int, string) {#putcellformula}

Placera formeln i cellen i tabellen.

```csharp
public void PutCellFormula(int rowOffset, int columnOffset, string formula)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| rowOffset | Int32 | Radoffseten i tabellen. |
| columnOffset | Int32 | Kolumnoffseten i tabellen. |
| formel | String | Formeln i cellen. |

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Tables;

namespace AsposeCellsExamples
{
    public class ListObjectMethodPutCellFormulaWithInt32Int32StringDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook wb = new Workbook();
            Worksheet sheet = wb.Worksheets[0];
            
            // Lägg till exempeldata för att skapa en tabell
            sheet.Cells["A1"].PutValue("ID");
            sheet.Cells["B1"].PutValue("Value");
            sheet.Cells["C1"].PutValue("Formula");
            sheet.Cells["A2"].PutValue(1);
            sheet.Cells["B2"].PutValue(10);
            sheet.Cells["A3"].PutValue(2);
            sheet.Cells["B3"].PutValue(20);

            // Skapa ett listobjekt (tabell)
            int index = sheet.ListObjects.Add("A1", "C3", true);
            ListObject table = sheet.ListObjects[index];

            // Lägg till en ny rad och sätt värden/formel
            table.PutCellValue(4, 0, 3); // Row 4, Column 0 (ID)
            table.PutCellValue(4, 1, 30); // Row 4, Column 1 (Value)
            table.PutCellFormula(4, 2, "=B3*2"); // Row 4, Column 2 (Formula)

            // Spara arbetsboken
            wb.Save("output.xlsx");
        }
    }
}
```

### Se även

* class [ListObject](../)
* namespace [Aspose.Cells.Tables](../../../aspose.cells.tables/)
* assembly [Aspose.Cells](../../../)

---

## PutCellFormula(int, int, string, bool) {#putcellformula_1}

Placera formeln i cellen i tabellen.

```csharp
public void PutCellFormula(int rowOffset, int columnOffset, string formula, bool isTotalsRowFormula)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| rowOffset | Int32 | Radoffseten i tabellen. |
| columnOffset | Int32 | Kolumnoffseten i tabellen. |
| formel | String | Formeln i cellen. |
| isTotalsRowFormula | Boolean |  |

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Tables;

namespace AsposeCellsExamples
{
    public class ListObjectMethodPutCellFormulaWithInt32Int32StringBooleanDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            
            // Kom åt första arbetsbladet
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Lägg till exempeldata för att skapa ett listobjekt
            worksheet.Cells["A1"].PutValue("Column1");
            worksheet.Cells["A2"].PutValue(10);
            worksheet.Cells["A3"].PutValue(20);
            
            // Skapa listobjekt
            int index = worksheet.ListObjects.Add(0, 0, 2, 0, true);
            ListObject listObject = worksheet.ListObjects[index];
            
            // Demonstrera PutCellFormula
            listObject.PutCellFormula(3, 0, "=SUM(A2:A3)", true);
            
            // Spara arbetsboken
            workbook.Save("output.xlsx");
        }
    }
}
```

### Se även

* class [ListObject](../)
* namespace [Aspose.Cells.Tables](../../../aspose.cells.tables/)
* assembly [Aspose.Cells](../../../)


