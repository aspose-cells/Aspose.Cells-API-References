---
title: "CustomFilterCollection.And"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "CustomFilterCollection‑Eigenschaft. Gibt an, ob die beiden Kriterien eine UND‑Beziehung haben"
type: docs
url: /de/net/aspose.cells/customfiltercollection/and/
---
## CustomFilterCollection.And property

Gibt an, ob die beiden Kriterien eine \"und\"-Beziehung haben.

```csharp
public bool And { get; set; }
```

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CustomFilterCollectionPropertyAndDemo
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
                // Erstellen Sie eine neue CustomFilterCollection
                CustomFilterCollection filters = new CustomFilterCollection();

                // Zeige den Standardwert der And‑Eigenschaft an
                Console.WriteLine($"Default And property value: {filters.And}");

                // Setze die And‑Eigenschaft auf true
                filters.And = true;
                Console.WriteLine($"After setting to true, And property value: {filters.And}");

                // Setze die And‑Eigenschaft auf false
                filters.And = false;
                Console.WriteLine($"After setting to false, And property value: {filters.And}");

                // Speichere die Arbeitsmappe
                workbook.Save("CustomFilterCollectionAndDemo.xlsx");
                Console.WriteLine("CustomFilterCollection And property demonstrated successfully");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error demonstrating And property: {ex.Message}");
            }
        }
    }
}
```

### Siehe auch

* class [CustomFilterCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


