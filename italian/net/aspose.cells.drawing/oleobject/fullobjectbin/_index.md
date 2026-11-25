---
title: "OleObject.FullObjectBin"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà OleObject. Ottiene i dati binari completi dell'oggetto ole incorporato nel file modello"
type: docs
url: /it/net/aspose.cells.drawing/oleobject/fullobjectbin/
---
## OleObject.FullObjectBin property

Ottiene i dati binari completi dell'oggetto ole incorporato nel file modello.

```csharp
public byte[] FullObjectBin { get; }
```

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;
    using System.IO;

    public class OleObjectPropertyFullObjectBinDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi un oggetto OLE al foglio di lavoro
            byte[] objectData = File.ReadAllBytes("example.docx");
            int oleObjectIndex = worksheet.OleObjects.Add(10, 10, 200, 200, objectData, "docx");
            OleObject oleObject = worksheet.OleObjects[oleObjectIndex];

            // Imposta alcune proprietà per l'oggetto OLE
            oleObject.FileFormatType = FileFormatType.Docx;
            oleObject.ObjectData = objectData;
            oleObject.IsAutoSize = true;

            // Ottieni i dati FullObjectBin (proprietà di sola lettura)
            byte[] fullObjectBinData = oleObject.FullObjectBin;
            Console.WriteLine("FullObjectBin data length: " + (fullObjectBinData != null ? fullObjectBinData.Length.ToString() : "null"));

            // Dimostra l'uso di FullObjectBin salvandolo in un file
            if (fullObjectBinData != null && fullObjectBinData.Length > 0)
            {
                File.WriteAllBytes("FullObjectBinData.bin", fullObjectBinData);
                Console.WriteLine("Saved FullObjectBin data to file.");
            }

            // Crea un altro workbook per dimostrare la lettura dell'oggetto OLE
            Workbook workbook2 = new Workbook();
            Worksheet worksheet2 = workbook2.Worksheets[0];

            // Aggiungi l'oggetto OLE dai dati FullObjectBin
            if (fullObjectBinData != null)
            {
                int newOleObjectIndex = worksheet2.OleObjects.Add(10, 10, 200, 200, fullObjectBinData, "docx");
                Console.WriteLine("Added new OLE object using FullObjectBin data.");
            }

            // Salva i workbook
            workbook.Save("OleObjectWithFullObjectBin.xlsx");
            workbook2.Save("OleObjectFromFullObjectBin.xlsx");
        }
    }
}
```

### Vedi anche

* class [OleObject](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


