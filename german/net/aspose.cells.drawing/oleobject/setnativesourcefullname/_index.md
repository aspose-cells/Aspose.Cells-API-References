---
title: "OleObject.SetNativeSourceFullName"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "OleObject-Methode. Legt den vollständigen Dateinamen der nativen OLE-Quelle mit Pfad fest"
type: docs
url: /de/net/aspose.cells.drawing/oleobject/setnativesourcefullname/
---
## OleObject.SetNativeSourceFullName method

Setzt den vollständigen Dateinamen der nativen Ole-Quelle mit Pfad.

```csharp
public void SetNativeSourceFullName(string sourceFullName)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| sourceFullName | String | der vollständige Dateiname der nativen OLE-Quelle |

### Beispiele

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
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ein OleObject zum Arbeitsblatt hinzufügen
            int oleObjectIndex = worksheet.OleObjects.Add(10, 10, 200, 200, new byte[0]); // Changed to empty byte array
            OleObject oleObject = worksheet.OleObjects[oleObjectIndex];

            try
            {
                // Rufe die SetNativeSourceFullName-Methode mit einem String-Parameter auf
                oleObject.SetNativeSourceFullName(@"C:\temp\updated_test.xlsx");
                
                Console.WriteLine("SetNativeSourceFullName method executed successfully with parameter: C:\\temp\\updated_test.xlsx");
                
                // Zeige die Wirkung an, indem du die ObjectSourceFullName-Eigenschaft prüfst
                Console.WriteLine($"OleObject's source is now: {oleObject.ObjectSourceFullName}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing SetNativeSourceFullName method: {ex.Message}");
            }
            
            // Speichere die Arbeitsmappe
            workbook.Save("OleObjectMethodSetNativeSourceFullNameDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [OleObject](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


