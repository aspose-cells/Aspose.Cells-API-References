---
title: "TableStyleCollection.GetBuiltinTableStyle"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "TableStyleCollection-Methode. Ruft den integrierten Tabellenstil ab"
type: docs
url: /de/net/aspose.cells.tables/tablestylecollection/getbuiltintablestyle/
---
## TableStyleCollection.GetBuiltinTableStyle method

Liest den integrierten Tabellenstil

```csharp
public TableStyle GetBuiltinTableStyle(TableStyleType type)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Typ | TableStyleType | Der integrierte Tabellenstiltyp. |

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Tables;
    using System;

    public class TableStyleCollectionMethodGetBuiltinTableStyleWithTableStyleTypeDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Füge Beispieldaten hinzu, um eine Tabelle zu erstellen
            worksheet.Cells["A1"].PutValue("Name");
            worksheet.Cells["B1"].PutValue("Age");
            worksheet.Cells["A2"].PutValue("John");
            worksheet.Cells["B2"].PutValue(30);
            worksheet.Cells["A3"].PutValue("Alice");
            worksheet.Cells["B3"].PutValue(25);

            // Eine Tabelle erstellen
            int tableIndex = worksheet.ListObjects.Add(0, 0, 2, 1, true);
            Aspose.Cells.Tables.ListObject table = worksheet.ListObjects[tableIndex];

            try
            {
                // Die Tabellenstil-Sammlung abrufen
                TableStyleCollection tableStyles = workbook.Worksheets.TableStyles;

                // Rufe GetBuiltinTableStyle mit dem TableStyleType-Parameter auf
                TableStyle builtinStyle = tableStyles.GetBuiltinTableStyle(TableStyleType.TableStyleMedium2);

                // Wende den integrierten Stil auf unsere Tabelle an
                table.TableStyleName = builtinStyle.Name;

                Console.WriteLine($"Applied built-in table style: {builtinStyle.Name}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetBuiltinTableStyle method: {ex.Message}");
            }

            // Speichere die Arbeitsmappe
            workbook.Save("TableStyleCollectionMethodGetBuiltinTableStyleDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [TableStyle](../../tablestyle/)
* enum [TableStyleType](../../tablestyletype/)
* class [TableStyleCollection](../)
* namespace [Aspose.Cells.Tables](../../../aspose.cells.tables/)
* assembly [Aspose.Cells](../../../)


