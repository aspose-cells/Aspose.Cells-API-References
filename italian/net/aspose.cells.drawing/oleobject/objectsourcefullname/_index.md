---
title: "OleObject.ObjectSourceFullName"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà OleObject. Restituisce il nome completo della sorgente del file per l'oggetto OLE collegato"
type: docs
url: /it/net/aspose.cells.drawing/oleobject/objectsourcefullname/
---
## OleObject.ObjectSourceFullName property

Restituisce il nome completo della sorgente del file di origine per l'oggetto OLE collegato.

```csharp
public string ObjectSourceFullName { get; set; }
```

### Osservazioni

Supporta solo l'impostazione del nome completo della sorgente quando il tipo di file è OleFileType.Unknown. Come file wav, file avi, ecc..

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class OleObjectPropertyObjectSourceFullNameDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi un oggetto OLE (usando i dati del file come array di byte)
            byte[] fileData = System.IO.File.ReadAllBytes("test.docx");
            int oleObjectIndex = worksheet.OleObjects.Add(10, 10, 200, 200, fileData);
            Aspose.Cells.Drawing.OleObject oleObject = worksheet.OleObjects[oleObjectIndex];

            // Imposta e ottieni ObjectSourceFullName
            oleObject.ObjectSourceFullName = "C:\\Temp\\source.docx";
            Console.WriteLine("OLE Object Source Full Name: " + oleObject.ObjectSourceFullName);

            // Salva la cartella di lavoro
            workbook.Save("OleObjectDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [OleObject](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


