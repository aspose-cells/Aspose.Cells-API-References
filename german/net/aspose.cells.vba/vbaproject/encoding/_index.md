---
title: "VbaProject.Encoding"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "VbaProject-Eigenschaft. Gibt die Kodierung des VBA-Projekts zurück und legt sie fest"
type: docs
url: /de/net/aspose.cells.vba/vbaproject/encoding/
---
## VbaProject.Encoding property

Liest und setzt die Kodierung des VBA-Projekts.

```csharp
public Encoding Encoding { get; set; }
```

### Beispiele

```csharp
using System;
using System.Text;
using Aspose.Cells;
using Aspose.Cells.Vba;
using System.Security.Cryptography.X509Certificates;

namespace AsposeCellsExamples
{
    public class VbaProjectPropertyEncodingDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();

            // VBA-Projekt initialisieren
            VbaProject vbaProject = workbook.VbaProject;

            // Setze VBA-Projekteigenschaften einschließlich Kodierung
            vbaProject.Name = "TestVbaProject";
            vbaProject.Encoding = Encoding.UTF8;

            // Fügen Sie ein Modul zum VBA-Projekt hinzu
            vbaProject.Modules.Add(VbaModuleType.Class, "TestModule");

            // Speichere die Arbeitsmappe mit VBA-Projekt
            workbook.Save("VbaProjectEncodingDemo.xlsm");
        }
    }
}
```

### Siehe auch

* class [VbaProject](../)
* namespace [Aspose.Cells.Vba](../../../aspose.cells.vba/)
* assembly [Aspose.Cells](../../../)


