---
title: "CustomFilterCollection.And"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà CustomFilterCollection. Indica se i due criteri hanno una relazione AND"
type: docs
url: /it/net/aspose.cells/customfiltercollection/and/
---
## CustomFilterCollection.And property

Indica se i due criteri hanno una relazione "and".

```csharp
public bool And { get; set; }
```

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CustomFilterCollectionPropertyAndDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi dati di esempio
            worksheet.Cells["A1"].Value = "Numbers";
            worksheet.Cells["A2"].Value = 10;
            worksheet.Cells["A3"].Value = 20;
            worksheet.Cells["A4"].Value = 30;
            worksheet.Cells["A5"].Value = 40;
            worksheet.Cells["A6"].Value = 50;

            try
            {
                // Crea una nuova CustomFilterCollection
                CustomFilterCollection filters = new CustomFilterCollection();

                // Visualizza il valore predefinito della proprietà And
                Console.WriteLine($"Default And property value: {filters.And}");

                // Imposta la proprietà And su true
                filters.And = true;
                Console.WriteLine($"After setting to true, And property value: {filters.And}");

                // Imposta la proprietà And su false
                filters.And = false;
                Console.WriteLine($"After setting to false, And property value: {filters.And}");

                // Salva la cartella di lavoro
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

### Vedi anche

* class [CustomFilterCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


