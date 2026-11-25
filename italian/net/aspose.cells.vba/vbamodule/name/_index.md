---
title: "VbaModule.Name"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà VbaModule. Ottiene e imposta il nome del modulo"
type: docs
url: /it/net/aspose.cells.vba/vbamodule/name/
---
## VbaModule.Name property

Ottiene e imposta il nome del modulo.

```csharp
public string Name { get; set; }
```

### Esempi

```csharp
using System;
using System.IO;
using Aspose.Cells;
using Aspose.Cells.Vba;

namespace AsposeCellsExamples
{
    public class VbaModulePropertyNameDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook wb = new Workbook();

            // Aggiungi un foglio di lavoro e ottieni il suo modulo VBA
            Worksheet sheet = wb.Worksheets[0];
            int moduleIndex = wb.VbaProject.Modules.Add(sheet);
            VbaModule module = wb.VbaProject.Modules[moduleIndex];

            // Imposta il nome del modulo
            module.Name = "Sheet1";

            // Aggiungi codice VBA semplice al modulo
            string vbaCode = "Private Sub Worksheet_SelectionChange(ByVal Target As Range)\r\n" +
                             "    MsgBox \"Sheet name: \" & Me.Name\r\n" +
                             "End Sub\r\n";
            module.Codes = vbaCode;

            // Salva in uno stream di memoria (per dimostrazione)
            using (MemoryStream ms = new MemoryStream())
            {
                wb.Save(ms, SaveFormat.Xlsm);
            }
        }
    }
}
```

### Vedi anche

* class [VbaModule](../)
* namespace [Aspose.Cells.Vba](../../../aspose.cells.vba/)
* assembly [Aspose.Cells](../../../)


