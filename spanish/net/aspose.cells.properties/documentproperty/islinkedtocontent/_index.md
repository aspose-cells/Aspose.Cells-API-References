---
title: "DocumentProperty.IsLinkedToContent"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "DocumentProperty property. Indica si esta propiedad está vinculada al contenido"
type: docs
url: /es/net/aspose.cells.properties/documentproperty/islinkedtocontent/
---
## DocumentProperty.IsLinkedToContent property

Indica si esta propiedad está vinculada al contenido

```csharp
public bool IsLinkedToContent { get; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Properties;

namespace AsposeCellsExamples
{
    public class DocumentPropertyPropertyIsLinkedToContentDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            
            // Agregar datos de muestra a las celdas
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].Value = "Company Name";
            worksheet.Cells["B1"].Value = "Company Address";

            // Crea propiedades de documento personalizadas vinculadas
            workbook.CustomDocumentProperties.AddLinkToContent("Company", "A1");
            workbook.CustomDocumentProperties.AddLinkToContent("Address", "B1");

            // Obtén y verifica la propiedad IsLinkedToContent
            DocumentProperty companyProp = workbook.CustomDocumentProperties["Company"];
            Console.WriteLine($"Is 'Company' property linked to content: {companyProp.IsLinkedToContent}");
            Console.WriteLine($"Linked source: {companyProp.Source}");
            Console.WriteLine($"Current value: {companyProp.Value}");

            // Actualiza el valor de la celda y actualiza las propiedades vinculadas
            worksheet.Cells["A1"].Value = "Updated Company Name";
            workbook.CustomDocumentProperties.UpdateLinkedPropertyValue();

            // Verifique que la propiedad se haya actualizado
            Console.WriteLine($"Updated value: {companyProp.Value}");

            // Guarda el libro de trabajo
            workbook.Save("LinkedPropertiesDemo.xlsx");
        }
    }
}
```

### Ver también

* class [DocumentProperty](../)
* namespace [Aspose.Cells.Properties](../../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../../)


