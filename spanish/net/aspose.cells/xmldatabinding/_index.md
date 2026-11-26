---
title: "Clase XmlDataBinding"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Clase Aspose.Cells.XmlDataBinding. Representa información de enlace de datos Xml"
type: docs
url: /es/net/aspose.cells/xmldatabinding/
---
## XmlDataBinding class

Representa la información de enlace de datos Xml.

```csharp
public class XmlDataBinding
```

## Propiedades

| Nombre | Descripción |
| --- | --- |
| [Url](../../aspose.cells/xmldatabinding/url/) { get; } | Obtiene la URL de origen de este enlace de datos. |

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Tables;
    using System;

    public class CellsClassXmlDataBindingDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Crear un objeto de lista que utilizará el enlace de datos XML
            ListObject listObject = worksheet.ListObjects[worksheet.ListObjects.Add(0, 0, 5, 4, true)];

            // Obtener la información del enlace de datos XML (normalmente se establecería al importar datos XML)
            XmlDataBinding xmlDataBinding = listObject.XmlMap.DataBinding;

            // Mostrar la URL de la fuente de datos XML (propiedad de solo lectura)
            Console.WriteLine("XML Data Binding Source URL: " + xmlDataBinding.Url);

            // Nota: En un escenario real, la Url se establecería al importar datos XML
            // Con fines de demostración, mostramos cómo acceder a la propiedad

            // Guarda el libro de trabajo
            workbook.Save("XmlDataBindingDemo.xlsx");
        }
    }
}
```

### Ver también

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


