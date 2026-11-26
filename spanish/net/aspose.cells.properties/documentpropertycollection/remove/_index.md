---
title: "DocumentPropertyCollection.Remove"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método DocumentPropertyCollection. Elimina una propiedad con el nombre especificado de la colección"
type: docs
url: /es/net/aspose.cells.properties/documentpropertycollection/remove/
---
## DocumentPropertyCollection.Remove method

Elimina una propiedad con el nombre especificado de la colección.

```csharp
public void Remove(string name)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| name | String | El nombre de la propiedad sin distinción de mayúsculas. |

### Ejemplos

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

### Ver también

* class [DocumentPropertyCollection](../)
* namespace [Aspose.Cells.Properties](../../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../../)


