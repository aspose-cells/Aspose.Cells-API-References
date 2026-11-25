---
title: "OleObject.FileFormatType"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà OleObject. Ottiene e imposta il tipo di file dei dati dell'oggetto ole incorporato"
type: docs
url: /it/net/aspose.cells.drawing/oleobject/fileformattype/
---
## OleObject.FileFormatType property

Ottiene e imposta il tipo di file dei dati dell'oggetto ole incorporato

```csharp
public FileFormatType FileFormatType { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class OleObjectPropertyFileFormatTypeDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            
            // Accedi al primo foglio di lavoro
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Aggiungi un oggetto OLE al foglio di lavoro (senza dati del file)
            int oleIndex = worksheet.OleObjects.Add(10, 10, 200, 200, null);
            
            // Ottieni l'oggetto OLE aggiunto
            OleObject oleObject = worksheet.OleObjects[oleIndex];
            
            // Imposta e visualizza il tipo di formato file
            oleObject.FileFormatType = FileFormatType.Docm;
            Console.WriteLine("OLE Object File Format Type: " + oleObject.FileFormatType);
            
            // Salva la cartella di lavoro
            workbook.Save("OleObjectFileFormatTypeDemo.xlsx");
        }
    }
}
```

### Vedi anche

* enum [FileFormatType](../../../aspose.cells/fileformattype/)
* class [OleObject](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


