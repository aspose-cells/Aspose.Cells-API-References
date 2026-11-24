---
title: "DocumentPropertyCollection.Remove"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "DocumentPropertyCollection-Methode. Entfernt eine Eigenschaft mit dem angegebenen Namen aus der Sammlung"
type: docs
url: /de/net/aspose.cells.properties/documentpropertycollection/remove/
---
## DocumentPropertyCollection.Remove method

Entfernt eine Eigenschaft mit dem angegebenen Namen aus der Sammlung.

```csharp
public void Remove(string name)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Name | String | Der Groß-/Kleinschreibung‑unabhängige Name der Eigenschaft. |

### Beispiele

```csharp
using System;
using System.IO;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class DocumentPropertyCollectionMethodRemoveWithStringDemo
    {
        public static void Run()
        {
            string inputPath = "example.xlsx";
            string outputPath = "output.xlsm";

            using (FileStream stream = new FileStream(inputPath, FileMode.Open))
            {
                Workbook workbook = new Workbook(stream);
                
                if (workbook.Worksheets.CustomDocumentProperties.Contains("_PID_HLINKS"))
                {
                    workbook.Worksheets.CustomDocumentProperties.Remove("_PID_HLINKS");
                }

                workbook.Save(outputPath, SaveFormat.Xlsm);
            }
        }
    }
}
```

### Siehe auch

* class [DocumentPropertyCollection](../)
* namespace [Aspose.Cells.Properties](../../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../../)


