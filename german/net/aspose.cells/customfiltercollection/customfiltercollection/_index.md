---
title: "CustomFilterCollection.CustomFilterCollection"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "CustomFilterCollection‑Konstruktor. Erstellt eine neue Instanz"
type: docs
url: /de/net/aspose.cells/customfiltercollection/customfiltercollection/
---
## CustomFilterCollection constructor

Erstellt eine neue Instanz.

```csharp
[Obsolete("Use FilterColumn.CustomFilters, instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public CustomFilterCollection()
```

### Hinweise

HINWEIS: Dieses Mitglied ist jetzt veraltet. Stattdessen setzen Sie bitte FilterColumn.FilterType auf FilterType.CustomFilters und rufen dann FilterColumn.CustomFilters ab. Diese Eigenschaft wird 12 Monate später, seit Juni 2026, entfernt. Aspose entschuldigt sich für etwaige Unannehmlichkeiten, die Sie möglicherweise erfahren haben.

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CustomFilterCollectionMethodSharpctorDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Fügen Sie Beispieldaten hinzu
            worksheet.Cells["A1"].Value = "Numbers";
            worksheet.Cells["A2"].Value = 10;
            worksheet.Cells["A3"].Value = 20;
            worksheet.Cells["A4"].Value = 30;
            worksheet.Cells["A5"].Value = 40;
            worksheet.Cells["A6"].Value = 50;

            try
            {
                // Erstellen Sie eine neue CustomFilterCollection mithilfe des Konstruktors
                CustomFilterCollection filters = new CustomFilterCollection();

                // Zeige den Standardwert der And‑Eigenschaft an
                Console.WriteLine($"Default And property value: {filters.And}");

                // Der Konstruktor erstellt eine leere Sammlung
                Console.WriteLine($"Number of filters in collection: {filters.Count}");

                // Speichere die Arbeitsmappe
                workbook.Save("CustomFilterCollectionDemo.xlsx");
                Console.WriteLine("CustomFilterCollection created successfully");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error creating CustomFilterCollection: {ex.Message}");
            }
        }
    }
}
```

### Siehe auch

* class [CustomFilterCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


