---
title: "Workbook.CustomXmlParts"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad Workbook. Representa una Custom XML Data Storage Part de datos XML personalizados dentro de un paquete"
type: docs
url: /es/net/aspose.cells/workbook/customxmlparts/
---
## Workbook.CustomXmlParts property

Representa una parte de almacenamiento de datos XML personalizada (datos XML personalizados dentro de un paquete).

```csharp
public CustomXmlPartCollection CustomXmlParts { get; }
```

### Ejemplos

```csharp
using System;
using System.Text;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookPropertyCustomXmlPartsDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook wb = new Workbook();
            
            // Definir datos XML y esquema
            string xmlData = "<MyXmlData1 xmlns=\"http://my.namespace.com\"/>";
            string xmlSchema = "<?xml version=\"1.0\" encoding=\"UTF-8\" standalone=\"no\"?>" +
                "<ds:datastoreItem ds:itemID=\"{1D3CF2F4-9155-40AE-99F6-33298D217F89}\" xmlns:ds=\"http://schemas.openxmlformats.org/officeDocument/2006/customXml\">" +
                    "<ds:schemaRefs>" +
                        "<ds:schemaRef ds:uri=\"http://my.namespace.com\"/>" +
                    "</ds:schemaRefs>" +
                "</ds:datastoreItem>";

            // Agregar una parte XML personalizada al libro de trabajo
            wb.CustomXmlParts.Add(Encoding.UTF8.GetBytes(xmlData), Encoding.UTF8.GetBytes(xmlSchema));

            // Guardar y volver a cargar el libro de trabajo
            string outputPath = "output.xlsx";
            wb.Save(outputPath);
            
            Workbook loadedWb = new Workbook(outputPath);
            
            // Mostrar el recuento de partes XML personalizadas
            Console.WriteLine($"Number of custom XML parts: {loadedWb.CustomXmlParts.Count}");
        }
    }
}
```

### Ver también

* class [CustomXmlPartCollection](../../../aspose.cells.markup/customxmlpartcollection/)
* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


