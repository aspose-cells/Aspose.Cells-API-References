---
title: "OleObject.ObjectSourceFullName"
second_title: "Aspose.Cells för .NET API‑referens"
description: "OleObject-egenskap. Returnerar det fullständiga källnamnet för källfilen för det länkade OLE-objektet"
type: docs
url: /sv/net/aspose.cells.drawing/oleobject/objectsourcefullname/
---
## OleObject.ObjectSourceFullName property

Returnerar det fullständiga källnamnet för källfilen för det länkade OLE-objektet.

```csharp
public string ObjectSourceFullName { get; set; }
```

### Anmärkningar

Stöder endast att ange det fullständiga källnamnet när filtypen är OleFileType.Unknown. Till exempel wav-fil, avi-fil osv..

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class OleObjectPropertyObjectSourceFullNameDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till ett OLE-objekt (använder fildata som byte array)
            byte[] fileData = System.IO.File.ReadAllBytes("test.docx");
            int oleObjectIndex = worksheet.OleObjects.Add(10, 10, 200, 200, fileData);
            Aspose.Cells.Drawing.OleObject oleObject = worksheet.OleObjects[oleObjectIndex];

            // Ange och hämta ObjectSourceFullName
            oleObject.ObjectSourceFullName = "C:\\Temp\\source.docx";
            Console.WriteLine("OLE Object Source Full Name: " + oleObject.ObjectSourceFullName);

            // Spara arbetsboken
            workbook.Save("OleObjectDemo.xlsx");
        }
    }
}
```

### Se även

* class [OleObject](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


