---
title: "VbaProjectReference.Name"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "VbaProjectReference-Eigenschaft. Liest und schreibt den Namen der Referenz"
type: docs
url: /de/net/aspose.cells.vba/vbaprojectreference/name/
---
## VbaProjectReference.Name property

Ermittelt und setzt den Namen der Referenz.

```csharp
public string Name { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Vba;

namespace AsposeCellsExamples
{
    public class VbaProjectReferencePropertyNameDemo
    {
        public static void Run()
        {
            // Erstelle eine Arbeitsmappe (VBA-Projekt wird für .xlsm-Dateien automatisch erstellt)
            Workbook workbook = new Workbook(FileFormatType.Xlsm);
            
            // Füge eine Referenz zum VBA-Projekt hinzu
            string referenceName = "MyReference";
            string referencePath = @"C:\Temp\MyLibrary.dll";
            workbook.VbaProject.References.AddRegisteredReference(referenceName, referencePath);

            // Greife auf die Referenz zu und verifiziere sie über die Name-Eigenschaft
            VbaProjectReferenceCollection references = workbook.VbaProject.References;
            for (int i = 0; i < references.Count; i++)
            {
                if (references[i].Name.Equals(referenceName))
                {
                    Console.WriteLine($"Found reference: {references[i].Name}");
                    break;
                }
            }

            // Speichere die Arbeitsmappe
            workbook.Save("VbaProjectReferenceDemo.xlsm");
        }
    }
}
```

### Siehe auch

* class [VbaProjectReference](../)
* namespace [Aspose.Cells.Vba](../../../aspose.cells.vba/)
* assembly [Aspose.Cells](../../../)


