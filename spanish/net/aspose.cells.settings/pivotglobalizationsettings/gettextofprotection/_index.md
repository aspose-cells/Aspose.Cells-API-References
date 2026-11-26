---
title: "PivotGlobalizationSettings.GetTextOfProtection"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método PivotGlobalizationSettings. Obtiene el nombre de protección en la PivotTable"
type: docs
url: /es/net/aspose.cells.settings/pivotglobalizationsettings/gettextofprotection/
---
## PivotGlobalizationSettings.GetTextOfProtection method

Obtiene el nombre de protección en la tabla dinámica.

```csharp
[Obsolete("Use PivotGlobalizationSettings.GetTextOfProtectedName(string) method instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public virtual string GetTextOfProtection()
```

### Valor de retorno

El nombre de protección de la tabla dinámica

### Observaciones

NOTA: Este miembro está ahora obsoleto. En su lugar, por favor use el método PivotGlobalizationSettings.GetTextOfProtectedName(string). Esta propiedad será eliminada 12 meses después desde marzo de 2023. Aspose se disculpa por cualquier inconveniente que pueda haber experimentado.

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;
using Aspose.Cells.Settings;

namespace AsposeCellsExamples
{
    public class PivotGlobalizationSettingsMethodGetTextOfProtectionDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar datos de ejemplo
            worksheet.Cells["A1"].PutValue("Product");
            worksheet.Cells["B1"].PutValue("Sales");
            worksheet.Cells["A2"].PutValue("Apple");
            worksheet.Cells["B2"].PutValue(1000);
            worksheet.Cells["A3"].PutValue("Banana");
            worksheet.Cells["B3"].PutValue(2000);

            // Crear tabla dinámica
            int pivotIndex = worksheet.PivotTables.Add("A1:B3", "D1", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
            pivotTable.AddFieldToArea(PivotFieldType.Data, 1);

            // Cree la configuración de globalización y demuestre GetTextOfProtection
            PivotGlobalizationSettings globalizationSettings = new PivotGlobalizationSettings();
            Console.WriteLine("Protection Text: " + globalizationSettings.GetTextOfProtection());

            // Guarda el libro de trabajo
            workbook.Save("PivotGlobalizationDemo.xlsx");
        }
    }
}
```

### Ver también

* class [PivotGlobalizationSettings](../)
* namespace [Aspose.Cells.Settings](../../../aspose.cells.settings/)
* assembly [Aspose.Cells](../../../)


