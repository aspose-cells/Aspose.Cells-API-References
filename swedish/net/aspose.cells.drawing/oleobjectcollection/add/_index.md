---
title: "OleObjectCollection.Add"
second_title: "Aspose.Cells för .NET API‑referens"
description: "OleObjectCollection-metod. Lägger till ett OleObject i samlingen"
type: docs
url: /sv/net/aspose.cells.drawing/oleobjectcollection/add/
---
## Add(int, int, int, int, byte[]) {#add}

Lägger till ett OleObject i samlingen.

```csharp
public int Add(int topRow, int leftColumn, int height, int width, byte[] imageData)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| topRow | Int32 | Övre vänstra radindex. |
| leftColumn | Int32 | Övre vänstra kolumnindex. |
| höjd | Int32 | Höjd för oleObject, i enheten pixel. |
| bredd | Int32 | Bredd för oleObject, i enheten pixel. |
| imageData | Byte[] | Bild av ole-objekt som byte-array. |

### Returvärde

[`OleObject`](../../oleobject/) object index.

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;
    using System.IO;

    public class OleObjectCollectionMethodAddWithInt32Int32Int32Int32ByteDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Förbered OLE-objektsdata (exempelfil i Excel som byte-array)
            byte[] oleData;
            try
            {
                string sampleFilePath = "sample.xlsx";
                oleData = File.ReadAllBytes(sampleFilePath);
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error reading sample file: {ex.Message}");
                return;
            }

            try
            {
                // Anropa Add-metoden med parametrarna: (upperLeftRow, upperLeftColumn, height, width, imageData)
                int oleIndex = worksheet.OleObjects.Add(5, 2, 200, 300, oleData);

                Console.WriteLine($"OLE object added successfully at index: {oleIndex}");
                Console.WriteLine($"Position: Row 5, Column 2");
                Console.WriteLine($"Size: 200px height, 300px width");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing Add method: {ex.Message}");
            }

            // Spara resultatet
            workbook.Save("OleObjectAddDemo.xlsx");
        }
    }
}
```

### Se även

* class [OleObjectCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)

---

## Add(int, int, int, int, byte[], string) {#add_1}

Lägger till ett länkat OleObject i samlingen.

```csharp
public int Add(int topRow, int leftColumn, int height, int width, byte[] imageData, 
    string linkedFile)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| topRow | Int32 | Övre vänstra radindex. |
| leftColumn | Int32 | Övre vänstra kolumnindex. |
| höjd | Int32 | Höjd för oleObject, i enheten pixel. |
| bredd | Int32 | Bredd för oleObject, i enheten pixel. |
| imageData | Byte[] | Bild av ole-objekt som byte-array. |
| linkedFile | String |  |

### Returvärde

[`OleObject`](../../oleobject/) object index.

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.IO;

    public class OleObjectCollectionMethodAddWithInt32Int32Int32Int32ByteStringDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Förbered OLE-objektsdata
            int upperLeftRow = 1;
            int upperLeftColumn = 1;
            int height = 200;
            int width = 200;
            byte[] imageData = File.ReadAllBytes("sample.ole");
            string linkedFile = "sample.xlsx";

            try
            {
                // Anropa Add-metoden med de specifika parametertyperna
                int index = worksheet.OleObjects.Add(upperLeftRow, upperLeftColumn, height, width, imageData, linkedFile);
                
                Console.WriteLine($"OLE object added at index: {index}");
                Console.WriteLine($"Total OLE objects in worksheet: {worksheet.OleObjects.Count}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing Add method: {ex.Message}");
            }
            
            // Spara resultatet
            workbook.Save("OleObjectAddDemo.xlsx");
        }
    }
}
```

### Se även

* class [OleObjectCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


