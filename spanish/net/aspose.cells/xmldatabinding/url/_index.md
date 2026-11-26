---
title: "XmlDataBinding.Url"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad XmlDataBinding. Obtiene la URL de origen de este enlace de datos"
type: docs
url: /es/net/aspose.cells/xmldatabinding/url/
---
## XmlDataBinding.Url property

Obtiene la URL de origen de este enlace de datos.

```csharp
public string Url { get; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Tables;

namespace AsposeCellsExamples
{
    public class XmlDataBindingPropertyUrlDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            
            // Agregar dos hojas de cálculo
            workbook.Worksheets.Add("Sheet1");
            workbook.Worksheets.Add("Sheet2");

            // Agregar objetos de lista y mapas XML
            ListObject list1 = workbook.Worksheets[0].ListObjects[0];
            ListObject list2 = workbook.Worksheets[1].ListObjects[0];
            
            // Obtener URLs de enlace de datos XML (Url es de solo lectura)
            string url1 = list1.XmlMap.DataBinding.Url;
            string url2 = list2.XmlMap.DataBinding.Url;

            // Mostrar las URLs
            Console.WriteLine("Sheet1 ListObject XML URL: " + url1);
            Console.WriteLine("Sheet2 ListObject XML URL: " + url2);

            // Guarda el libro de trabajo
            workbook.Save("XmlDataBindingDemo.xlsx");
        }
    }
}
```

### Ver también

* class [XmlDataBinding](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


