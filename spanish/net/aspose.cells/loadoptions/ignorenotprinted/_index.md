---
title: "LoadOptions.IgnoreNotPrinted"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad LoadOptions. Ignora los datos que no se imprimen al imprimir el archivo directamente"
type: docs
url: /es/net/aspose.cells/loadoptions/ignorenotprinted/
---
## LoadOptions.IgnoreNotPrinted property

Ignora los datos que no se imprimen al imprimir directamente el archivo

```csharp
public bool IgnoreNotPrinted { get; set; }
```

### Observaciones

Solo para archivo xlsx.

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class LoadOptionsPropertyIgnoreNotPrintedDemo
    {
        public static void Run()
        {
            // Crear opciones de carga HTML y establecer IgnoreNotPrinted
            HtmlLoadOptions loadOptions = new HtmlLoadOptions(LoadFormat.Html);
            loadOptions.IgnoreNotPrinted = true;
            loadOptions.AutoFitColsAndRows = true;

            // Cargar archivo HTML con las opciones especificadas
            Workbook workbook = new Workbook("example.html", loadOptions);
            Worksheet worksheet = workbook.Worksheets[0];

            // Demostrar el efecto de IgnoreNotPrinted comprobando los estilos de celda
            Console.WriteLine("B3 Cell Color: " + worksheet.Cells["B3"].GetStyle().ForegroundColor);
            Console.WriteLine("B4 Cell Color: " + worksheet.Cells["B4"].GetStyle().ForegroundColor);
            Console.WriteLine("B5 Cell Color: " + worksheet.Cells["B5"].GetStyle().ForegroundColor);

            // Guarda el libro de trabajo
            workbook.Save("output.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### Ver también

* class [LoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


