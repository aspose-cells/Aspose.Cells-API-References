---
title: "DocumentPropertyCollection.Remove"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo DocumentPropertyCollection. Rimuove una proprietà con il nome specificato dalla collezione"
type: docs
url: /it/net/aspose.cells.properties/documentpropertycollection/remove/
---
## DocumentPropertyCollection.Remove method

Rimuove una proprietà con il nome specificato dalla raccolta.

```csharp
public void Remove(string name)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| name | String | Il nome della proprietà, senza distinzione tra maiuscole e minuscole. |

### Esempi

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

### Vedi anche

* class [DocumentPropertyCollection](../)
* namespace [Aspose.Cells.Properties](../../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../../)


