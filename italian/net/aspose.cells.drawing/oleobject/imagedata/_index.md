---
title: "OleObject.ImageData"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà OleObject. Rappresenta l'immagine dell'oggetto ole come array di byte"
type: docs
url: /it/net/aspose.cells.drawing/oleobject/imagedata/
---
## OleObject.ImageData property

Rappresenta l'immagine dell'oggetto ole come array di byte.

```csharp
public byte[] ImageData { get; set; }
```

### Esempi

```csharp
using System;
using System.IO;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class OleObjectPropertyImageDataDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            
            // Leggi il file immagine in un array di byte
            byte[] imageBytes = File.ReadAllBytes("image1.png");
            
            // Aggiungi un oggetto OLE con i dati dell'immagine
            int oleIndex = workbook.Worksheets[0].OleObjects.Add(0, 0, 60, 60, imageBytes);
            OleObject oleObject = workbook.Worksheets[0].OleObjects[oleIndex];
            
            // Imposta le proprietà dell'oggetto incorporato
            oleObject.SetEmbeddedObject(false, imageBytes, "image1.png", true, "Sample Image", false);
            
            // Dimostra l'uso della proprietà ImageData
            Console.WriteLine($"Image data length: {oleObject.ImageData.Length}");
            Console.WriteLine($"First byte: {oleObject.ImageData[0]}");
            Console.WriteLine($"Middle byte: {oleObject.ImageData[oleObject.ImageData.Length/2]}");
            Console.WriteLine($"Last byte: {oleObject.ImageData[oleObject.ImageData.Length-1]}");
            
            // Salva la cartella di lavoro
            workbook.Save("OleObjectWithImage.xlsx");
        }
    }
}
```

### Vedi anche

* class [OleObject](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


