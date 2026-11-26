---
title: "XmlLoadOptions.StartCell"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad XmlLoadOptions. Obtiene y establece la celda de inicio"
type: docs
url: /es/net/aspose.cells/xmlloadoptions/startcell/
---
## XmlLoadOptions.StartCell property

Obtiene y establece la celda inicial.

```csharp
public string StartCell { get; set; }
```

### Observaciones

Solo funciona cuando el archivo no es speadsheetML o mapea xml a Excel.

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class XmlLoadOptionsPropertyStartCellDemo
    {
        public static void Run()
        {
            // Crea una instancia de XmlLoadOptions
            XmlLoadOptions options = new XmlLoadOptions();

            // Establecer la celda de inicio para la importación de datos XML
            options.StartCell = "B2";

            // Carga un archivo XML en un Workbook usando las opciones especificadas
            Workbook workbook = new Workbook("input.xml", options);

            // Acceder a la primera hoja de cálculo
            Worksheet worksheet = workbook.Worksheets[0];

            // Muestra el valor de la celda inicial para demostrar la propiedad
            Console.WriteLine("Value at start cell (B2): " + worksheet.Cells["B2"].Value);

            // Guarda el libro de trabajo
            workbook.Save("output.xlsx");
        }
    }
}
```

### Ver también

* class [XmlLoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


