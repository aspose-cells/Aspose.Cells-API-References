---
title: "OleObject.SetNativeSourceFullName"
second_title: "Aspose.Cells för .NET API‑referens"
description: "OleObject-metod. Ställer in den inhemska källfilens fullständiga namn med sökväg"
type: docs
url: /sv/net/aspose.cells.drawing/oleobject/setnativesourcefullname/
---
## OleObject.SetNativeSourceFullName method

Anger det inhemska ole-källfilens fullständiga namn med sökväg.

```csharp
public void SetNativeSourceFullName(string sourceFullName)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| sourceFullName | String | den inhemska källfilens fullständiga namn |

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class OleObjectMethodSetNativeSourceFullNameWithStringDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till ett OleObject i kalkylbladet
            int oleObjectIndex = worksheet.OleObjects.Add(10, 10, 200, 200, new byte[0]); // Changed to empty byte array
            OleObject oleObject = worksheet.OleObjects[oleObjectIndex];

            try
            {
                // Anropa SetNativeSourceFullName-metoden med en strängparameter
                oleObject.SetNativeSourceFullName(@"C:\temp\updated_test.xlsx");
                
                Console.WriteLine("SetNativeSourceFullName method executed successfully with parameter: C:\\temp\\updated_test.xlsx");
                
                // Visa effekten genom att kontrollera egenskapen ObjectSourceFullName
                Console.WriteLine($"OleObject's source is now: {oleObject.ObjectSourceFullName}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing SetNativeSourceFullName method: {ex.Message}");
            }
            
            // Spara arbetsboken
            workbook.Save("OleObjectMethodSetNativeSourceFullNameDemo.xlsx");
        }
    }
}
```

### Se även

* class [OleObject](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


