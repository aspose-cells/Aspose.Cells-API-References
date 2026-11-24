---
title: "VbaModule.BinaryCodes"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "VbaModule-Eigenschaft. Gibt die Binärcodes des Moduls zurück und legt sie fest"
type: docs
url: /de/net/aspose.cells.vba/vbamodule/binarycodes/
---
## VbaModule.BinaryCodes property

Liest und schreibt die Binärcodes des Moduls.

```csharp
public byte[] BinaryCodes { get; }
```

### Beispiele

```csharp
using System;
using System.Text;
using Aspose.Cells;
using Aspose.Cells.Vba;

namespace AsposeCellsExamples
{
    public class VbaModulePropertyBinaryCodesDemo
    {
        public static void Run()
        {
            // Laden Sie die Arbeitsmappe mit VBA-Projekt
            Workbook workbook = new Workbook("example.xlsm");
            
            // Zugriff auf das VBA-Projekt
            VbaProject vbaProject = workbook.VbaProject;
            
            // Rufen Sie die Binärcodes des ersten Moduls ab
            byte[] binaryCodes = vbaProject.Modules[0].BinaryCodes;
            
            // In Zeichenfolge konvertieren mit chinesischer Kodierung (936)
            string codeContent = Encoding.GetEncoding(936).GetString(binaryCodes);
            
            // Geben Sie den Inhalt aus, der chinesische Zeichen enthält
            Console.WriteLine("VBA Module Content:");
            Console.WriteLine(codeContent);
        }
    }
}
```

### Siehe auch

* class [VbaModule](../)
* namespace [Aspose.Cells.Vba](../../../aspose.cells.vba/)
* assembly [Aspose.Cells](../../../)


