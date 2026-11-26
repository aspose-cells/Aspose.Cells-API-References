---
title: "WorkbookSettings.SignificantDigits"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad WorkbookSettings. Obtiene y establece el número de dígitos significativos. El valor predeterminado es SignificantDigits"
type: docs
url: /es/net/aspose.cells/workbooksettings/significantdigits/
---
## WorkbookSettings.SignificantDigits property

Obtiene y establece el número de dígitos significativos. El valor predeterminado es [`SignificantDigits`](../../cellshelper/significantdigits/).

```csharp
[Obsolete("Use SignificantDigitsType property instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public int SignificantDigits { get; set; }
```

### Observaciones

Solo puede ser 15 o 17 ahora. NOTA: Este miembro está ahora obsoleto. En su lugar, por favor use [`SignificantDigitsType`](../significantdigitstype/). Esta propiedad será eliminada 12 meses después a partir de junio de 2025. Aspose se disculpa por cualquier inconveniente que haya experimentado.

### Ejemplos

```csharp
using System;
using System.Globalization;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookSettingsPropertySignificantDigitsDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Agregar datos numéricos de muestra para demostrar los dígitos significativos
            sheet.Cells["A1"].PutValue(123.4567890123456789);
            sheet.Cells["A2"].PutValue(0.000000000123456789);

            // Acceder a la configuración del libro de trabajo
            WorkbookSettings settings = workbook.Settings;

            // Establecer los dígitos significativos a 15 (precisión máxima para double)
            settings.SignificantDigits = 15;

            // Guardar el libro de trabajo para mostrar el efecto de los dígitos significativos
            workbook.Save("SignificantDigitsDemo.xlsx");

            Console.WriteLine("Workbook saved with SignificantDigits set to 15.");
        }
    }
}
```

### Ver también

* class [WorkbookSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


