---
title: "OleObject.SetEmbeddedObject"
second_title: "Aspose.Cells för .NET API‑referens"
description: "OleObject-metod. Ställer in inbäddad objektdata"
type: docs
url: /sv/net/aspose.cells.drawing/oleobject/setembeddedobject/
---
## SetEmbeddedObject(bool, byte[], string, bool, string) {#setembeddedobject}

Anger inbäddad objektdata.

```csharp
public void SetEmbeddedObject(bool linkToFile, byte[] objectData, string sourceFileName, 
    bool displayAsIcon, string label)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| linkToFile | Boolean | Anger om objektet länkar till filen. Om true ignoreras parametern objectData. |
| objectData | Byte[] | Den inbäddade objektdata. |
| sourceFileName | String | Filnamnet. |
| displayAsIcon | Boolean | Anger om objektet visas som en ikon. Om true kommer den ursprungliga bilddata att täckas av ikonen. |
| label | String | Ikonetiketten. Fungerar endast när displayAsIcon är true. |

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;
    using System.IO;

    public class OleObjectMethodSetEmbeddedObjectWithBooleanByteArrayStringBooleanStringDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till ett OleObject i kalkylbladet
            int oleObjectIndex = worksheet.OleObjects.Add(10, 10, 200, 200, new byte[0]);
            OleObject oleObject = worksheet.OleObjects[oleObjectIndex];

            try
            {
                // Förbered parametrar för SetEmbeddedObject
                bool linkToFile = false;
                byte[] objectData = File.ReadAllBytes("sample.xlsx");
                string sourceFileName = "sample.xlsx";
                bool displayAsIcon = false;
                string label = "Excel Document";

                // Anropa SetEmbeddedObject med de angivna parametrarna
                oleObject.SetEmbeddedObject(linkToFile, objectData, sourceFileName, displayAsIcon, label);

                Console.WriteLine("SetEmbeddedObject executed successfully with parameters (Boolean, Byte[], String, Boolean, String)");
                
                // Visa några egenskaper för att visa effekten
                Console.WriteLine($"OleObject label: {oleObject.Label}");
                Console.WriteLine($"Display as icon: {oleObject.DisplayAsIcon}");
                Console.WriteLine($"Is linked to file: {oleObject.IsLink}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing SetEmbeddedObject method: {ex.Message}");
            }

            // Spara arbetsboken
            workbook.Save("OleObjectMethodSetEmbeddedObjectDemo.xlsx");
        }
    }
}
```

### Se även

* class [OleObject](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)

---

## SetEmbeddedObject(bool, byte[], string, bool, string, bool) {#setembeddedobject_1}

Anger inbäddad objektdata.

```csharp
public void SetEmbeddedObject(bool linkToFile, byte[] objectData, string sourceFileName, 
    bool displayAsIcon, string label, bool updateIcon)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| linkToFile | Boolean | Anger om objektet länkar till filen. Om true ignoreras parametern objectData. |
| objectData | Byte[] | Den inbäddade objektdata. |
| sourceFileName | String | Filnamnet. |
| displayAsIcon | Boolean | Anger om objektet visas som en ikon. Om true kommer den ursprungliga bilddata att täckas av ikonen. |
| label | String | Ikonetiketten. Fungerar endast när displayAsIcon är true. |
| updateIcon | Boolean | Anger om ikonen uppdateras automatiskt. |

### Anmärkningar

Eftersom Aspose kan uppdatera alla inbäddade filikoner, är det bättre att du kan lägga till rätt ikon med *updateIcon* satt till false.

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;
    using System.IO;

    public class OleObjectMethodSetEmbeddedObjectWithBooleanByteArrayStringBooleanStringBooleanDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till ett OleObject i kalkylbladet
            int oleObjectIndex = worksheet.OleObjects.Add(10, 10, 200, 200, new byte[0]);
            OleObject oleObject = worksheet.OleObjects[oleObjectIndex];

            try
            {
                // Förbered parametrar för SetEmbeddedObject
                bool linkToFile = false;
                byte[] objectData = File.ReadAllBytes("sample.docx");
                string sourceFileName = "sample.docx";
                bool displayAsIcon = true;
                string label = "Word Document";
                bool updateIcon = true;

                // Anropa SetEmbeddedObject med de angivna parametrarna
                oleObject.SetEmbeddedObject(linkToFile, objectData, sourceFileName, displayAsIcon, label, updateIcon);

                Console.WriteLine("SetEmbeddedObject executed successfully with parameters (Boolean, Byte[], String, Boolean, String, Boolean)");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing SetEmbeddedObject method: {ex.Message}");
            }

            // Spara arbetsboken
            workbook.Save("OleObjectMethodSetEmbeddedObjectDemo.xlsx");
        }
    }
}
```

### Se även

* class [OleObject](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


