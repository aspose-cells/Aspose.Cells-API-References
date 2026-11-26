---
title: "TxtLoadOptions.TextQualifier"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad TxtLoadOptions. Especifica el calificador de texto para los valores de celda. El calificador predeterminado es"
type: docs
url: /es/net/aspose.cells/txtloadoptions/textqualifier/
---
## TxtLoadOptions.TextQualifier property

Especifica el calificador de texto para los valores de celda. El calificador predeterminado es '\"'.

```csharp
public char TextQualifier { get; set; }
```

### Observaciones

Al establecer esta propiedad, [`HasTextQualifier`](../hastextqualifier/) se volverá true automáticamente.

### Ejemplos

```csharp
using System;
using System.Text;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class TxtLoadOptionsPropertyTextQualifierDemo
    {
        public static void Run()
        {
            // Crea una instancia de TxtLoadOptions para CSV
            TxtLoadOptions loadOptions = new TxtLoadOptions(LoadFormat.Csv)
            {
                Separator = ',',
                HasTextQualifier = true,
                TextQualifier = '\"'
            };

            // Crea datos CSV de ejemplo con calificadores de texto
            string csvData = "Name,Age,City\n\"John Doe\",30,\"New York\"\n\"Jane Smith\",25,\"San Francisco\"";
            
            // Guarda los datos de ejemplo en un archivo temporal
            string tempFile = "temp.csv";
            System.IO.File.WriteAllText(tempFile, csvData);

            // Carga el archivo CSV con las opciones especificadas
            Workbook workbook = new Workbook(tempFile, loadOptions);

            // Guarda el libro de trabajo en un archivo Excel
            workbook.Save("TextQualifierDemo.xlsx");

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


