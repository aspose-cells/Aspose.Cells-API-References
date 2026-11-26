---
title: "XmlSaveOptions.SheetIndexes"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad XmlSaveOptions. Representa los índices de las hojas exportadas"
type: docs
url: /es/net/aspose.cells/xmlsaveoptions/sheetindexes/
---
## XmlSaveOptions.SheetIndexes property

Representa los índices de las hojas exportadas.

```csharp
public int[] SheetIndexes { get; set; }
```

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class XmlSaveOptionsPropertySheetIndexesDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo con varias hojas
            Workbook workbook = new Workbook();
            workbook.Worksheets.Add("Sheet2");
            workbook.Worksheets.Add("Sheet3");

            // Poblar algunos datos en todas las hojas
            for (int i = 0; i < workbook.Worksheets.Count; i++)
            {
                Worksheet sheet = workbook.Worksheets[i];
                sheet.Cells["A1"].PutValue("Data in " + sheet.Name);
            }

            // Crear instancia de XmlSaveOptions
            XmlSaveOptions options = new XmlSaveOptions();

            // Inicialmente exportar todas las hojas (SheetIndexes es nulo)
            Console.WriteLine("Initial SheetIndexes value: " + (options.SheetIndexes == null ? "null (all sheets)" : string.Join(",", options.SheetIndexes)));

            // Configurar para exportar solo la primera y la tercera hoja (índices 0 y 2)
            options.SheetIndexes = new int[] { 0, 2 };

            // Guardar solo con las hojas seleccionadas
            workbook.Save("XmlExportSelectedSheets.xml", options);

            // Cambiar para exportar solo la segunda hoja (índice 1)
            options.SheetIndexes = new int[] { 1 };

            // Guardar con una selección de hojas diferente
            workbook.Save("XmlExportSingleSheet.xml", options);

            // Establecer SheetIndexes a nulo para exportar todas las hojas
            options.SheetIndexes = null;
            workbook.Save("XmlExportAllSheets.xml", options);
        }
    }
}
```

### Ver también

* class [XmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


