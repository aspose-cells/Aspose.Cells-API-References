---
title: "LoadOptions.MemorySetting"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad LoadOptions. Obtiene o establece el modo de memoria para el libro de trabajo cargado"
type: docs
url: /es/net/aspose.cells/loadoptions/memorysetting/
---
## LoadOptions.MemorySetting property

Obtiene o establece el modo de memoria para el libro de trabajo cargado.

```csharp
public MemorySetting MemorySetting { get; set; }
```

### Observaciones

Para obtener más detalles sobre el modo de memoria, consulte [`MemorySetting`](../../cells/memorysetting/).

### Ejemplos

```csharp
using System;
using System.IO;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class LoadOptionsPropertyMemorySettingDemo
    {
        public static void Run()
        {
            // Crear opciones de carga con la configuración de preferencia de memoria
            LoadOptions loadOptions = new LoadOptions(LoadFormat.Auto);
            loadOptions.MemorySetting = MemorySetting.MemoryPreference;

            // Cargar libro de trabajo con configuraciones optimizadas de memoria
            Workbook workbook = new Workbook(new MemoryStream(), loadOptions);
            
            // Acceder a la hoja de cálculo y agregar algunos datos de muestra
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Memory Setting Demo");
            worksheet.Cells["A2"].PutValue(DateTime.Now.ToString());
            
            // Guarda el libro de trabajo
            workbook.Save("MemorySettingDemo.xlsx", SaveFormat.Xlsx);
            
            Console.WriteLine("Workbook saved with MemoryPreference setting.");
        }
    }
}
```

### Ver también

* enum [MemorySetting](../../memorysetting/)
* class [LoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


