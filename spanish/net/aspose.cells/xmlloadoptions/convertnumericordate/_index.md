---
title: "XmlLoadOptions.ConvertNumericOrDate"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad XmlLoadOptions. Indica si se convierte el valor en el archivo xml a numérico o fecha"
type: docs
url: /es/net/aspose.cells/xmlloadoptions/convertnumericordate/
---
## XmlLoadOptions.ConvertNumericOrDate property

Indica si se convierte el valor del archivo XML a numérico o fecha.

```csharp
public bool ConvertNumericOrDate { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class XmlLoadOptionsPropertyConvertNumericOrDateDemo
    {
        public static void Run()
        {
            // Crear opciones de carga XML
            XmlLoadOptions options = new XmlLoadOptions();
            
            // Establecer ConvertNumericOrDate a true (por defecto)
            options.ConvertNumericOrDate = true;
            Workbook wb1 = new Workbook("input.xml", options);
            Cell cell1 = wb1.Worksheets[0].Cells["A1"];
            Console.WriteLine("With conversion (true): " + cell1.Value + " is type: " + cell1.Type);
            
            // Establecer ConvertNumericOrDate a false
            options.ConvertNumericOrDate = false;
            Workbook wb2 = new Workbook("input.xml", options);
            Cell cell2 = wb2.Worksheets[0].Cells["A1"];
            Console.WriteLine("Without conversion (false): " + cell2.Value + " is type: " + cell2.Type);
            
            // Guardar resultados
            wb1.Save("output_with_conversion.xlsx");
            wb2.Save("output_without_conversion.xlsx");
        }
    }
}
```

### Ver también

* class [XmlLoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


