---
title: "OleObject.IsAutoSize"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà OleObject. True indica che la dimensione dell'oggetto ole verrà modificata automaticamente in base alla dimensione dell'istantanea del contenuto incorporato quando l'oggetto ole è attivato"
type: docs
url: /it/net/aspose.cells.drawing/oleobject/isautosize/
---
## OleObject.IsAutoSize property

True indica che la dimensione dell'oggetto ole verrà modificata automaticamente in base alla dimensione dell'istantanea del contenuto incorporato quando l'oggetto ole è attivato.

```csharp
public bool IsAutoSize { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class OleObjectPropertyIsAutoSizeDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi un oggetto OLE (usando i dati del file come array di byte)
            byte[] oleData = System.IO.File.ReadAllBytes(@"C:\example\test.docx");
            int oleIndex = worksheet.OleObjects.Add(10, 10, 200, 200, oleData);
            Aspose.Cells.Drawing.OleObject oleObject = worksheet.OleObjects[oleIndex];

            // Imposta e dimostra la proprietà IsAutoSize
            oleObject.IsAutoSize = true;
            Console.WriteLine("OLE Object AutoSize initially: " + oleObject.IsAutoSize);

            // Modifica la proprietà
            oleObject.IsAutoSize = false;
            Console.WriteLine("OLE Object AutoSize after change: " + oleObject.IsAutoSize);

            // Salva la cartella di lavoro
            workbook.Save("OleObjectIsAutoSizeDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [OleObject](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


