---
title: "Workbook.RibbonXml"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad Workbook. Obtiene y establece el archivo XML que define la interfaz de usuario de la cinta"
type: docs
url: /es/net/aspose.cells/workbook/ribbonxml/
---
## Workbook.RibbonXml property

Obtiene y establece el archivo XML que define la interfaz Ribbon UI.

```csharp
public string RibbonXml { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookPropertyRibbonXmlDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();

            // Ejemplo de XML de cinta para personalizar la cinta
            string ribbonXml = 
                "<customUI xmlns=\"http://schemas.microsoft.com/office/2006/01/customui\">" +
                "  <ribbon>" +
                "    <tabs>" +
                "      <tab id=\"customTab\" label=\"My Tab\">" +
                "        <group id=\"customGroup\" label=\"My Group\">" +
                "          <button id=\"customButton\" label=\"My Button\" size=\"large\" />" +
                "        </group>" +
                "      </tab>" +
                "    </tabs>" +
                "  </ribbon>" +
                "</customUI>";

            // Establecer la propiedad RibbonXml
            workbook.RibbonXml = ribbonXml;

            // Guarda el libro de trabajo
            workbook.Save("output.xlsm");

            // Verificar la propiedad RibbonXml
            Console.WriteLine("RibbonXml is set: " + (workbook.RibbonXml != null));
        }
    }
}
```

### Ver también

* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


