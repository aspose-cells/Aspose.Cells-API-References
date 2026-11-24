---
title: "ListObject.PutCellFormula"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "ListObject‑Methode. Setzt die Formel in die Zelle der Tabelle"
type: docs
url: /de/net/aspose.cells.tables/listobject/putcellformula/
---
## PutCellFormula(int, int, string) {#putcellformula}

Setzt die Formel in die Zelle der Tabelle.

```csharp
public void PutCellFormula(int rowOffset, int columnOffset, string formula)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| rowOffset | Int32 | Der Zeilenversatz in der Tabelle. |
| columnOffset | Int32 | Der Spaltenversatz in der Tabelle. |
| Formel | String | Die Formel der Zelle. |

### Beispiele

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
            // Erstelle ein neues Arbeitsbuch
            Workbook wb = new Workbook();
            Worksheet sheet = wb.Worksheets[0];
            
            // Füge Beispieldaten hinzu, um eine Tabelle zu erstellen
            sheet.Cells["A1"].PutValue("ID");
            sheet.Cells["B1"].PutValue("Value");
            sheet.Cells["C1"].PutValue("Formula");
            sheet.Cells["A2"].PutValue(1);
            sheet.Cells["B2"].PutValue(10);
            sheet.Cells["A3"].PutValue(2);
            sheet.Cells["B3"].PutValue(20);

            // Erstelle ein Listenobjekt (Tabelle)
            int index = sheet.ListObjects.Add("A1", "C3", true);
            ListObject table = sheet.ListObjects[index];

            // Eine neue Zeile hinzufügen und Werte/Formel setzen
            table.PutCellValue(4, 0, 3); // Row 4, Column 0 (ID)
            table.PutCellValue(4, 1, 30); // Row 4, Column 1 (Value)
            table.PutCellFormula(4, 2, "=B3*2"); // Row 4, Column 2 (Formula)

            // Speichere die Arbeitsmappe
            wb.Save("output.xlsx");
        }
    }
}
```

### Siehe auch

* class [ListObject](../)
* namespace [Aspose.Cells.Tables](../../../aspose.cells.tables/)
* assembly [Aspose.Cells](../../../)

---

## PutCellFormula(int, int, string, bool) {#putcellformula_1}

Setzt die Formel in die Zelle der Tabelle.

```csharp
public void PutCellFormula(int rowOffset, int columnOffset, string formula, bool isTotalsRowFormula)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| rowOffset | Int32 | Der Zeilenversatz in der Tabelle. |
| columnOffset | Int32 | Der Spaltenversatz in der Tabelle. |
| Formel | String | Die Formel der Zelle. |
| isTotalsRowFormula | Boolean |  |

### Beispiele

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
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            
            // Zugriff auf das erste Arbeitsblatt
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Beispieldaten hinzufügen, um ein List-Objekt zu erstellen.
            worksheet.Cells["A1"].PutValue("Column1");
            worksheet.Cells["A2"].PutValue(10);
            worksheet.Cells["A3"].PutValue(20);
            
            // List-Objekt erstellen
            int index = worksheet.ListObjects.Add(0, 0, 2, 0, true);
            ListObject listObject = worksheet.ListObjects[index];
            
            // PutCellFormula demonstrieren
            listObject.PutCellFormula(3, 0, "=SUM(A2:A3)", true);
            
            // Speichere die Arbeitsmappe
            workbook.Save("output.xlsx");
        }
    }
}
```

### Siehe auch

* class [ListObject](../)
* namespace [Aspose.Cells.Tables](../../../aspose.cells.tables/)
* assembly [Aspose.Cells](../../../)


