---
title: "OleObject.SetEmbeddedObject"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "OleObject-Methode. Setzt die Daten des eingebetteten Objekts."
type: docs
url: /de/net/aspose.cells.drawing/oleobject/setembeddedobject/
---
## SetEmbeddedObject(bool, byte[], string, bool, string) {#setembeddedobject}

Setzt die Daten des eingebetteten Objekts.

```csharp
public void SetEmbeddedObject(bool linkToFile, byte[] objectData, string sourceFileName, 
    bool displayAsIcon, string label)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| linkToFile | Boolean | Gibt an, ob das Objekt mit der Datei verknüpft ist. Wenn true, wird der Parameter objectData ignoriert. |
| objectData | Byte[] | Die Daten des eingebetteten Objekts. |
| sourceFileName | String | Der Dateiname. |
| displayAsIcon | Boolean | Gibt an, ob das Objekt als Symbol angezeigt wird. Wenn true, werden die ursprünglichen Bilddaten durch das Symbol überdeckt. |
| Bezeichnung | String | Die Symbolbeschriftung. Funktioniert nur, wenn displayAsIcon true ist. |

### Beispiele

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
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ein OleObject zum Arbeitsblatt hinzufügen
            int oleObjectIndex = worksheet.OleObjects.Add(10, 10, 200, 200, new byte[0]);
            OleObject oleObject = worksheet.OleObjects[oleObjectIndex];

            try
            {
                // Parameter für SetEmbeddedObject vorbereiten
                bool linkToFile = false;
                byte[] objectData = File.ReadAllBytes("sample.xlsx");
                string sourceFileName = "sample.xlsx";
                bool displayAsIcon = false;
                string label = "Excel Document";

                // Rufen Sie SetEmbeddedObject mit den angegebenen Parametern auf
                oleObject.SetEmbeddedObject(linkToFile, objectData, sourceFileName, displayAsIcon, label);

                Console.WriteLine("SetEmbeddedObject executed successfully with parameters (Boolean, Byte[], String, Boolean, String)");
                
                // Einige Eigenschaften anzeigen, um den Effekt zu zeigen
                Console.WriteLine($"OleObject label: {oleObject.Label}");
                Console.WriteLine($"Display as icon: {oleObject.DisplayAsIcon}");
                Console.WriteLine($"Is linked to file: {oleObject.IsLink}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing SetEmbeddedObject method: {ex.Message}");
            }

            // Speichere die Arbeitsmappe
            workbook.Save("OleObjectMethodSetEmbeddedObjectDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [OleObject](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)

---

## SetEmbeddedObject(bool, byte[], string, bool, string, bool) {#setembeddedobject_1}

Setzt die Daten des eingebetteten Objekts.

```csharp
public void SetEmbeddedObject(bool linkToFile, byte[] objectData, string sourceFileName, 
    bool displayAsIcon, string label, bool updateIcon)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| linkToFile | Boolean | Gibt an, ob das Objekt mit der Datei verknüpft ist. Wenn true, wird der Parameter objectData ignoriert. |
| objectData | Byte[] | Die Daten des eingebetteten Objekts. |
| sourceFileName | String | Der Dateiname. |
| displayAsIcon | Boolean | Gibt an, ob das Objekt als Symbol angezeigt wird. Wenn true, werden die ursprünglichen Bilddaten durch das Symbol überdeckt. |
| Bezeichnung | String | Die Symbolbeschriftung. Funktioniert nur, wenn displayAsIcon true ist. |
| updateIcon | Boolean | Gibt an, ob das Symbol automatisch aktualisiert wird. |

### Hinweise

Da Aspose alle Dateisymbole aktualisieren kann, ist es besser, wenn Sie das korrekte Symbol mit *updateIcon* auf false setzen.

### Beispiele

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
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ein OleObject zum Arbeitsblatt hinzufügen
            int oleObjectIndex = worksheet.OleObjects.Add(10, 10, 200, 200, new byte[0]);
            OleObject oleObject = worksheet.OleObjects[oleObjectIndex];

            try
            {
                // Parameter für SetEmbeddedObject vorbereiten
                bool linkToFile = false;
                byte[] objectData = File.ReadAllBytes("sample.docx");
                string sourceFileName = "sample.docx";
                bool displayAsIcon = true;
                string label = "Word Document";
                bool updateIcon = true;

                // Rufen Sie SetEmbeddedObject mit den angegebenen Parametern auf
                oleObject.SetEmbeddedObject(linkToFile, objectData, sourceFileName, displayAsIcon, label, updateIcon);

                Console.WriteLine("SetEmbeddedObject executed successfully with parameters (Boolean, Byte[], String, Boolean, String, Boolean)");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing SetEmbeddedObject method: {ex.Message}");
            }

            // Speichere die Arbeitsmappe
            workbook.Save("OleObjectMethodSetEmbeddedObjectDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [OleObject](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


