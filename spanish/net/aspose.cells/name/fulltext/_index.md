---
title: "Name.FullText"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad Name. Obtiene el texto completo del nombre del objeto con la configuración de alcance"
type: docs
url: /es/net/aspose.cells/name/fulltext/
---
## Name.FullText property

Obtiene el texto completo del nombre del objeto con la configuración de alcance.

```csharp
public string FullText { get; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class NamePropertyFullTextDemo
    {
        public static void Run()
        {
            // Crear un libro de trabajo
            Workbook workbook = new Workbook();
            
            // Acceder a la primera hoja de cálculo
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Crear algunos rangos con nombre
            worksheet.Cells["A1"].PutValue("Test Value");
            worksheet.Cells.CreateRange("A1", "B5").Name = "TestRange1";
            worksheet.Cells.CreateRange("C1", "D5").Name = "TestRange2";
            
            // Obtener la colección de nombres
            NameCollection names = workbook.Worksheets.Names;
            
            // Buscar un nombre por su FullText
            string reference = "=Sheet1!$A$1:$B$5";
            Name foundName = FindNameByFullText(names, reference);
            
            // Mostrar resultados
            if (foundName != null)
            {
                Console.WriteLine("Found name: " + foundName.Text);
                Console.WriteLine("FullText: " + foundName.FullText);
            }
            else
            {
                Console.WriteLine("Name not found");
            }
        }
        
        public static Name FindNameByFullText(NameCollection names, string reference)
        {
            if (reference.IndexOf('=') == 0)
            {
                reference = reference.Substring(1);
            }
            foreach (Name nm in names)
            {
                if (nm.FullText.Equals(reference))
                {
                    return nm;
                }
            }
            return null;
        }
    }
}
```

### Ver también

* class [Name](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


