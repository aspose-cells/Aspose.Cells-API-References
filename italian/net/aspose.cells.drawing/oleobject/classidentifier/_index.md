---
title: "OleObject.ClassIdentifier"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà OleObject. Ottiene e imposta l'identificatore di classe dell'oggetto incorporato. Significa quale applicazione apre il file incorporato"
type: docs
url: /it/net/aspose.cells.drawing/oleobject/classidentifier/
---
## OleObject.ClassIdentifier property

Ottiene e imposta l'identificatore di classe dell'oggetto incorporato. Indica quale applicazione apre il file incorporato.

```csharp
public byte[] ClassIdentifier { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class OleObjectPropertyClassIdentifierDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Esempio di array di byte per ClassIdentifier (normalmente sarebbe un vero ID di classe)
            byte[] classId = new byte[] { 0x01, 0x02, 0x03, 0x04, 0x05, 0x06, 0x07, 0x08, 
                                         0x09, 0x0A, 0x0B, 0x0C, 0x0D, 0x0E, 0x0F, 0x10 };

            // Aggiungi un oggetto OLE con dati di esempio
            int oleIndex = sheet.OleObjects.Add(10, 10, 200, 100, new byte[100]);
            OleObject oleObject = sheet.OleObjects[oleIndex];
            
            // Imposta la proprietà ClassIdentifier
            oleObject.ClassIdentifier = classId;
            oleObject.ProgID = "Excel.Sheet.12";
            oleObject.DisplayAsIcon = true;

            // Salva la cartella di lavoro
            workbook.Save("OleObjectDemo.xlsx");

            // Carica la cartella di lavoro salvata per verificare il ClassIdentifier
            Workbook loadedWorkbook = new Workbook("OleObjectDemo.xlsx");
            OleObject loadedOle = loadedWorkbook.Worksheets[0].OleObjects[0];
            
            // Verifica che il ClassIdentifier sia stato conservato
            Console.WriteLine("ClassIdentifier length: " + loadedOle.ClassIdentifier.Length);
        }
    }
}
```

### Vedi anche

* class [OleObject](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


