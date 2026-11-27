---
title: "Klass OdsCellField"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.Ods.OdsCellField klass. Representerar cellfältet för ods"
type: docs
url: /sv/net/aspose.cells.ods/odscellfield/
---
## OdsCellField class

Representerar cellfältet för ods.

```csharp
public class OdsCellField
```

## Egenskaper

| Namn | Beskrivning |
| --- | --- |
| [Column](../../aspose.cells.ods/odscellfield/column/) { get; set; } | Hämtar och anger kolumnindexet för cellen. |
| [CustomFormat](../../aspose.cells.ods/odscellfield/customformat/) { get; set; } | Representerar det anpassade formatet för fältets värde. |
| [FieldType](../../aspose.cells.ods/odscellfield/fieldtype/) { get; set; } | Hämtar och anger typen för fältet. |
| [Row](../../aspose.cells.ods/odscellfield/row/) { get; set; } | Hämtar och anger radindexet för cellen. |

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using System;
    using Aspose.Cells;
    using Aspose.Cells.Ods;

    public class OdsClassOdsCellFieldDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok och hämta det första kalkylbladet
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            try
            {
                // -----------------------------------------------------------------
                // 1. Skapa ett OdsCellField via samlingen (ingen parameterlös konstruktor)
                // -----------------------------------------------------------------
                OdsCellFieldCollection odsFields = sheet.Cells.OdsCellFields;
                odsFields.Add(2, 1, OdsCellFieldType.Title, "Demo Title");

                // Hämta fältet vi just lade till
                OdsCellField manualField = odsFields[odsFields.Count - 1];

                // Skriv något till cellen som identifieras av OdsCellField
                sheet.Cells[manualField.Row, manualField.Column].PutValue("Manual Field");

                // --------------------------------------------------------------
                // 2. Lägg till samma fält igen för att demonstrera samlingsanvändning (valfritt)
                // --------------------------------------------------------------
                odsFields.Add(manualField.Row, manualField.Column, manualField.FieldType, manualField.CustomFormat);

                // Uppdatera alla ODS-fält så att de återspeglas i den sparade filen
                odsFields.UpdateFieldsValue();

                // Visa egenskapsvärdena i konsolen
                Console.WriteLine($"Created OdsCellField -> Row: {manualField.Row}, Column: {manualField.Column}, " +
                                  $"Type: {manualField.FieldType}, Format: {manualField.CustomFormat}");

                // Spara arbetsboken som en ODS-fil
                workbook.Save("OdsClassOdsCellFieldDemo.ods");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error while working with OdsCellField: {ex.Message}");
            }
        }
    }
}
```

### Se även

* namespace [Aspose.Cells.Ods](../../aspose.cells.ods/)
* assembly [Aspose.Cells](../../)


