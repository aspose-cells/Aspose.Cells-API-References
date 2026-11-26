---
title: "ExternalLinkCollection.GetEnumerator"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método ExternalLinkCollection. Obtiene un enumerador que recorre esta colección"
type: docs
url: /es/net/aspose.cells/externallinkcollection/getenumerator/
---
## ExternalLinkCollection.GetEnumerator method

Obtener un enumerador que recorra esta colección.

```csharp
public IEnumerator GetEnumerator()
```

### Ejemplos

```csharp
using System;
using System.Collections;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ExternalLinkCollectionMethodGetEnumeratorDemo
    {
        public static void Run()
        {
            // Crear un libro de trabajo
            Workbook workbook = new Workbook();
            
            // Agregue algunos enlaces externos usando la firma correcta del método Add
            workbook.Worksheets.ExternalLinks.Add("externallink1.xlam", new string[] { "Sheet1!A1" });
            workbook.Worksheets.ExternalLinks.Add("externallink2.xlam", new string[] { "Sheet1!A1" });
            workbook.Worksheets.ExternalLinks.Add("externallink3.xlam", new string[] { "Sheet1!A1" });
            workbook.Worksheets.ExternalLinks.Add("externallink4.xlam", new string[] { "Sheet1!A1" });

            // Obtenga la ExternalLinkCollection
            ExternalLinkCollection externalLinks = workbook.Worksheets.ExternalLinks;
            
            // Demostrar el uso de GetEnumerator
            Console.WriteLine("Enumerating external links:");
            IEnumerator enumerator = externalLinks.GetEnumerator();
            int count = 0;
            while (enumerator.MoveNext())
            {
                ExternalLink link = (ExternalLink)enumerator.Current;
                Console.WriteLine($"{++count}. {link.DataSource}");
            }

            // Agregar fórmulas que referencian estos enlaces externos
            Worksheet worksheet = workbook.Worksheets[0];
            for (int i = 0; i < 4; i++)
            {
                worksheet.Cells[i, 0].Formula = $"=externallink{i+1}.xlam!customfunc()";
            }

            Console.WriteLine("\nFormulas referencing external links:");
            for (int i = 0; i < 4; i++)
            {
                Console.WriteLine($"Cell A{i+1}: {worksheet.Cells[i, 0].Formula}");
            }
        }
    }
}
```

### Ver también

* class [ExternalLinkCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


