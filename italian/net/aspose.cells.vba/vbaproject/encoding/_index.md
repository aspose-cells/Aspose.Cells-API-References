---
title: "VbaProject.Encoding"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà VbaProject. Ottiene e imposta la codifica del progetto VBA"
type: docs
url: /it/net/aspose.cells.vba/vbaproject/encoding/
---
## VbaProject.Encoding property

Ottiene e imposta la codifica del progetto VBA.

```csharp
public Encoding Encoding { get; set; }
```

### Esempi

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
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();

            // Inizializza il progetto VBA
            VbaProject vbaProject = workbook.VbaProject;

            // Imposta le proprietà del progetto VBA includendo Encoding
            vbaProject.Name = "TestVbaProject";
            vbaProject.Encoding = Encoding.UTF8;

            // Aggiungi un modulo al progetto VBA
            vbaProject.Modules.Add(VbaModuleType.Class, "TestModule");

            // Salva la cartella di lavoro con il progetto VBA
            workbook.Save("VbaProjectEncodingDemo.xlsm");
        }
    }
}
```

### Vedi anche

* class [VbaProject](../)
* namespace [Aspose.Cells.Vba](../../../aspose.cells.vba/)
* assembly [Aspose.Cells](../../../)


