---
title: "LoadOptions.LoadFilter"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad LoadOptions. El filtro que indica cómo cargar los datos"
type: docs
url: /es/net/aspose.cells/loadoptions/loadfilter/
---
## LoadOptions.LoadFilter property

El filtro que indica cómo cargar los datos.

```csharp
public LoadFilter LoadFilter { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CustomLoadFilter : LoadFilter
    {
        public override void StartSheet(Worksheet sheet)
        {
            // Cargue los datos solo si la hoja es visible
            if (sheet.IsVisible)
            {
                base.StartSheet(sheet);
            }
        }
    }

    public class LoadOptionsPropertyLoadFilterDemo
    {
        public static void Run()
        {
            // Cree un libro de trabajo de prueba
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];
            sheet.Name = "HiddenSheet";
            sheet.IsVisible = false;
            sheet.Cells["A1"].PutValue("This should not load");
            
            // Agregue una hoja visible
            Worksheet visibleSheet = workbook.Worksheets.Add("VisibleSheet");
            visibleSheet.Cells["A1"].PutValue("This will load");
            
            // Guarde el archivo de prueba
            string filePath = "LoadFilterTest.xlsx";
            workbook.Save(filePath);
            workbook.Dispose();

            // Cargue con filtro personalizado
            LoadOptions options = new LoadOptions();
            options.LoadFilter = new CustomLoadFilter();
            
            Workbook loadedWorkbook = new Workbook(filePath, options);
            
            // Verificar que solo se cargó la hoja visible
            Console.WriteLine("Loaded Sheets:");
            foreach (Worksheet ws in loadedWorkbook.Worksheets)
            {
                Console.WriteLine($"- {ws.Name}: Visible={ws.IsVisible}");
                if (ws.IsVisible)
                {
                    Console.WriteLine($"  A1 Value: {ws.Cells["A1"].StringValue}");
                }
            }
            
            loadedWorkbook.Dispose();
        }
    }
}
```

### Ver también

* class [LoadFilter](../../loadfilter/)
* class [LoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


