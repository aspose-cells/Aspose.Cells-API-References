---
title: "OleObject.ObjectData"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà OleObject. Rappresenta i dati dell'oggetto ole incorporato come array di byte"
type: docs
url: /it/net/aspose.cells.drawing/oleobject/objectdata/
---
## OleObject.ObjectData property

Rappresenta i dati dell'oggetto ole incorporato come array di byte.

```csharp
public byte[] ObjectData { get; set; }
```

### Esempi

```csharp
using System;
using System.IO;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class OleObjectPropertyObjectDataDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            var workbook = new Workbook();
            
            // Accedi al primo foglio di lavoro
            var worksheet = workbook.Worksheets[0];
            
            // Percorsi di file di esempio (sostituiscili con percorsi reali nel tuo ambiente)
            string imagePath = "logo.jpg";
            string oleDataPath = "test.xls";

            // Aggiungi oggetto OLE con dati immagine iniziali
            int oleIndex = worksheet.OleObjects.Add(10, 10, 300, 200, File.ReadAllBytes(imagePath));
            
            // Modifica i dati dell'oggetto OLE
            worksheet.OleObjects[oleIndex].ObjectData = File.ReadAllBytes(oleDataPath);
            
            // Salva la cartella di lavoro
            workbook.Save("OleObjectDemo.xlsx", SaveFormat.Xlsx);
            
            Console.WriteLine("OLE object demo created successfully.");
        }
    }
}
```

### Vedi anche

* class [OleObject](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


