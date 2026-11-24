---
title: "WorksheetCollection.Insert"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "WorksheetCollection-Methode. Ein Arbeitsblatt einfügen."
type: docs
url: /de/net/aspose.cells/worksheetcollection/insert/
---
## Insert(int, SheetType) {#insert}

Fügt ein Arbeitsblatt ein.

```csharp
public Worksheet Insert(int index, SheetType sheetType)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Index | Int32 | Der Blattindex |
| sheetType | SheetType | Der Blatttyp. |

### Rückgabewert

Gibt ein eingefügtes Arbeitsblatt zurück.

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetCollectionMethodInsertWithInt32SheetTypeDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets.Insert(1, SheetType.Worksheet);
            worksheet.Name = "InsertedSheet";
            workbook.Worksheets[0].Cells["A1"].Value = "Referencing inserted sheet:";
            workbook.Worksheets[0].Cells["A2"].Formula = "='InsertedSheet'!A1";
        }
    }
}
```

### Siehe auch

* class [Worksheet](../../worksheet/)
* enum [SheetType](../../sheettype/)
* class [WorksheetCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## Insert(int, SheetType, string) {#insert_1}

Fügt ein Arbeitsblatt ein.

```csharp
public Worksheet Insert(int index, SheetType sheetType, string sheetName)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Index | Int32 | Der Blattindex |
| sheetType | SheetType | Der Blatttyp. |
| sheetName | String | Der Blattname. |

### Rückgabewert

Gibt ein eingefügtes Arbeitsblatt zurück.

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetCollectionMethodInsertWithInt32SheetTypeStringDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            
            // Füge ein neues Arbeitsblatt bei Index 0 mit dem Namen "InsertedSheet" ein.
            workbook.Worksheets.Insert(0, SheetType.Worksheet, "InsertedSheet");
            
            // Greife auf das eingefügte Arbeitsblatt zu.
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Füge einige Daten in Zelle A1 des eingefügten Blatts ein.
            worksheet.Cells["A1"].PutValue("This sheet was inserted using Insert method");
            
            // Speichere die Arbeitsmappe
            workbook.Save("WorksheetInsertDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [Worksheet](../../worksheet/)
* enum [SheetType](../../sheettype/)
* class [WorksheetCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


