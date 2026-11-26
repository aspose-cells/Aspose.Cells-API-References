---
title: "WorkbookSettings.RemovePersonalInformation"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad WorkbookSettings. Verdadero si la información personal puede ser eliminada del libro de trabajo especificado"
type: docs
url: /es/net/aspose.cells/workbooksettings/removepersonalinformation/
---
## WorkbookSettings.RemovePersonalInformation property

Verdadero si la información personal puede eliminarse del workbook especificado.

```csharp
public bool RemovePersonalInformation { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookSettingsPropertyRemovePersonalInformationDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            
            // Establecer RemovePersonalInformation a verdadero
            workbook.Settings.RemovePersonalInformation = true;
            
            // Agregar algunos datos de ejemplo
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Name");
            worksheet.Cells["B1"].PutValue("Email");
            worksheet.Cells["A2"].PutValue("John Doe");
            worksheet.Cells["B2"].PutValue("john@example.com");
            
            // Guarda el libro de trabajo
            string outputPath = "output_with_personal_info_removed.xlsx";
            workbook.Save(outputPath);
            
            // Cargar el libro guardado para verificar la configuración
            Workbook loadedWorkbook = new Workbook(outputPath);
            Console.WriteLine("RemovePersonalInformation setting: " + 
                loadedWorkbook.Settings.RemovePersonalInformation);
        }
    }
}
```

### Ver también

* class [WorkbookSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


