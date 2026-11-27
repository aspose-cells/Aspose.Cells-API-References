---
title: "VbaProjectReference.Name"
second_title: "Aspose.Cells för .NET API‑referens"
description: "VbaProjectReference-egenskap. Hämtar och anger namnet på referensen"
type: docs
url: /sv/net/aspose.cells.vba/vbaprojectreference/name/
---
## VbaProjectReference.Name property

Hämtar och anger namnet på referensen.

```csharp
public string Name { get; set; }
```

### Exempel

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
            // Skapa en arbetsbok (VBA-projekt skapas automatiskt för .xlsm-filer)
            Workbook workbook = new Workbook(FileFormatType.Xlsm);
            
            // Lägg till en referens till VBA-projektet
            string referenceName = "MyReference";
            string referencePath = @"C:\Temp\MyLibrary.dll";
            workbook.VbaProject.References.AddRegisteredReference(referenceName, referencePath);

            // Kom åt och verifiera referensen via Name-egenskapen
            VbaProjectReferenceCollection references = workbook.VbaProject.References;
            for (int i = 0; i < references.Count; i++)
            {
                if (references[i].Name.Equals(referenceName))
                {
                    Console.WriteLine($"Found reference: {references[i].Name}");
                    break;
                }
            }

            // Spara arbetsboken
            workbook.Save("VbaProjectReferenceDemo.xlsm");
        }
    }
}
```

### Se även

* class [VbaProjectReference](../)
* namespace [Aspose.Cells.Vba](../../../aspose.cells.vba/)
* assembly [Aspose.Cells](../../../)


