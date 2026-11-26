---
title: "TxtLoadOptions.HasTextQualifier"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad TxtLoadOptions. Indica si hay calificador de texto para el valor de la celda. El valor predeterminado es true"
type: docs
url: /es/net/aspose.cells/txtloadoptions/hastextqualifier/
---
## TxtLoadOptions.HasTextQualifier property

Indica si hay calificador de texto para el valor de la celda. El valor predeterminado es verdadero.

```csharp
public bool HasTextQualifier { get; set; }
```

### Ejemplos

```csharp
using System;
using System.Text;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class TxtLoadOptionsPropertyHasTextQualifierDemo
    {
        public static void Run()
        {
            // Cree contenido CSV con calificadores de texto
            string csvContent = "\"Name\",\"Age\",\"City\"\n\"John\",30,\"New York\"\n\"Alice\",25,\"London\"";
            
            // Guarde el contenido CSV en un archivo temporal
            string tempFile = "temp.csv";
            System.IO.File.WriteAllText(tempFile, csvContent, Encoding.UTF8);

            // Cree TxtLoadOptions con HasTextQualifier establecido en true
            TxtLoadOptions loadOptions = new TxtLoadOptions(LoadFormat.Csv)
            {
                Separator = ',',
                HasTextQualifier = true,
                TextQualifier = '\"'
            };

            // Cargue el archivo CSV con calificadores de texto
            Workbook workbook = new Workbook(tempFile, loadOptions);

            // Guarde el libro de trabajo para demostrar una carga exitosa
            workbook.Save("Output.xlsx");

            // Limpia el archivo temporal
            System.IO.File.Delete(tempFile);
        }
    }
}
```

### Ver también

* class [TxtLoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


