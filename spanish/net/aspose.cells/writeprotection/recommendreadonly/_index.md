---
title: "WriteProtection.RecommendReadOnly"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad WriteProtection. Indica si la opción \"Read Only Recommended\" está seleccionada"
type: docs
url: /es/net/aspose.cells/writeprotection/recommendreadonly/
---
## WriteProtection.RecommendReadOnly property

Indica si la opción Leer solo recomendado está seleccionada.

```csharp
public bool RecommendReadOnly { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WriteProtectionPropertyRecommendReadOnlyDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            
            // Acceder a la hoja de cálculo y agregar algunos datos de muestra
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Sample Data");

            // Establecer RecommendReadOnly a true
            workbook.Settings.WriteProtection.RecommendReadOnly = true;
            
            // Verificar que la propiedad está establecida
            Console.WriteLine("RecommendReadOnly: " + workbook.Settings.WriteProtection.RecommendReadOnly);
            Console.WriteLine("IsWriteProtected: " + workbook.Settings.WriteProtection.IsWriteProtected);

            // Guarda el libro de trabajo
            workbook.Save("output_recommend_readonly.xlsx");

            // Cargar el libro de trabajo guardado para verificar que la configuración persista
            Workbook loadedWorkbook = new Workbook("output_recommend_readonly.xlsx");
            Console.WriteLine("After loading - RecommendReadOnly: " + loadedWorkbook.Settings.WriteProtection.RecommendReadOnly);
            Console.WriteLine("After loading - IsWriteProtected: " + loadedWorkbook.Settings.WriteProtection.IsWriteProtected);
        }
    }
}
```

### Ver también

* class [WriteProtection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


