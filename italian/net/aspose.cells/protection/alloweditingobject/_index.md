---
title: "Protection.AllowEditingObject"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà Protection. Rappresenta se l'utente è autorizzato a manipolare gli oggetti di disegno su un foglio di lavoro protetto"
type: docs
url: /it/net/aspose.cells/protection/alloweditingobject/
---
## Protection.AllowEditingObject property

Rappresenta se all'utente è consentito manipolare gli oggetti di disegno su un foglio di lavoro protetto.

```csharp
public bool AllowEditingObject { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ProtectionPropertyAllowEditingObjectDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Imposta le impostazioni di protezione con AllowEditingObject abilitato
            Protection protection = worksheet.Protection;
            protection.AllowEditingObject = true;
            protection.AllowEditingContent = false; // Contrast with AllowEditingObject
            worksheet.Protect(ProtectionType.All);

            // Verifica i flag di protezione
            Console.WriteLine("Protection Settings:");
            Console.WriteLine($"AllowEditingObject: {protection.AllowEditingObject}");
            Console.WriteLine($"AllowEditingContent: {protection.AllowEditingContent}");

            // Crea una casella di testo (oggetto) per testare la modifica
            worksheet.Shapes.AddTextBox(0, 0, 100, 100, 200, 200);
            
            // Salva la cartella di lavoro
            workbook.Save("ProtectionDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [Protection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


