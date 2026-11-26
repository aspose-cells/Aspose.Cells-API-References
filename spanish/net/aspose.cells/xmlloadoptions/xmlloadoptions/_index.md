---
title: "XmlLoadOptions.XmlLoadOptions"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Constructor de XmlLoadOptions. Representa las opciones de carga del archivo xml"
type: docs
url: /es/net/aspose.cells/xmlloadoptions/xmlloadoptions/
---
## XmlLoadOptions() {#constructor}

Representa las opciones de carga del archivo XML.

```csharp
public XmlLoadOptions()
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class XmlLoadOptionsMethodCtorDemo
    {
        public static void Run()
        {
            // Crear nuevas opciones de carga XML
            XmlLoadOptions options = new XmlLoadOptions();
            
            // Establecer para convertir valores numéricos o de fecha
            options.ConvertNumericOrDate = true;
            
            // Cargar libro de trabajo con opciones
            Workbook workbook = new Workbook("input.xml", options);
            
            // Acceder a los datos de la celda
            Cell cell = workbook.Worksheets[0].Cells["A1"];
            Console.WriteLine("Cell Value: " + cell.Value);
            Console.WriteLine("Cell Type: " + cell.Type);
            
            // Guardar el libro de trabajo
            workbook.Save("output.xlsx");
        }
    }
}
```

### Ver también

* class [XmlLoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## XmlLoadOptions(LoadFormat) {#constructor_1}

Representa las opciones de carga del archivo XML.

```csharp
public XmlLoadOptions(LoadFormat type)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| type | LoadFormat | El tipo de formato de carga. |

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class XmlLoadOptionsMethodCtorWithLoadFormatDemo
    {
        public static void Run()
        {
            try
            {
                // Crear una instancia de XmlLoadOptions con el parámetro LoadFormat
                LoadFormat loadFormat = LoadFormat.Xml;
                XmlLoadOptions xmlLoadOptions = new XmlLoadOptions(loadFormat);

                // Establecer algunas propiedades de XmlLoadOptions
                xmlLoadOptions.StartCell = "A1";
                xmlLoadOptions.IsXmlMap = true;
                xmlLoadOptions.ConvertNumericOrDate = true;

                // Cree un libro de trabajo usando las opciones de carga
                Workbook workbook = new Workbook("sample.xml", xmlLoadOptions);

                // Acceder a la primera hoja de cálculo
                Worksheet worksheet = workbook.Worksheets[0];

                // Mostrar alguna información
                Console.WriteLine("XML file loaded successfully with LoadFormat.Xml");
                Console.WriteLine($"First cell value: {worksheet.Cells["A1"].Value}");

                // Guarda el libro de trabajo
                workbook.Save("XmlLoadOptionsCtorDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing XmlLoadOptions constructor: {ex.Message}");
            }
        }
    }
}
```

### Ver también

* enum [LoadFormat](../../loadformat/)
* class [XmlLoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


