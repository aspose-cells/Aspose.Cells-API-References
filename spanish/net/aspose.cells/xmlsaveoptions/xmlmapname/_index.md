---
title: "XmlSaveOptions.XmlMapName"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad XmlSaveOptions. Indica si se exporta el mapa xml en el archivo"
type: docs
url: /es/net/aspose.cells/xmlsaveoptions/xmlmapname/
---
## XmlSaveOptions.XmlMapName property

Indica si se exporta el mapa XML en el archivo.

```csharp
public string XmlMapName { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class XmlSaveOptionsPropertyXmlMapNameDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Llena algunos datos en la hoja de cálculo
            worksheet.Cells["A1"].PutValue("Product");
            worksheet.Cells["B1"].PutValue("Price");
            worksheet.Cells["A2"].PutValue("Laptop");
            worksheet.Cells["B2"].PutValue(999.99);

            // Crear mapa XML y agregarlo al libro de trabajo
            int mapIndex = workbook.Worksheets.XmlMaps.Add("<Schema><Element><Product/><Price/></Element></Schema>");
            XmlMap xmlMap = workbook.Worksheets.XmlMaps[mapIndex];
            xmlMap.Name = "ProductDataMap";

            // Crear XmlSaveOptions y establecer XmlMapName
            XmlSaveOptions saveOptions = new XmlSaveOptions();
            saveOptions.XmlMapName = "ProductDataMap";

            // Guardar el libro de trabajo con mapeo XML
            workbook.Save("XmlWithMapping.xml", saveOptions);
        }
    }
}
```

### Ver también

* class [XmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


