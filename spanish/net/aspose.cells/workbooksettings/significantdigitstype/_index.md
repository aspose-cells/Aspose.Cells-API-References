---
title: "WorkbookSettings.SignificantDigitsType"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad WorkbookSettings. Obtiene y establece el tipo de dígitos significativos para la salida de valores numéricos en este libro de trabajo. El valor predeterminado es SignificantDigitsType"
type: docs
url: /es/net/aspose.cells/workbooksettings/significantdigitstype/
---
## WorkbookSettings.SignificantDigitsType property

Obtiene y establece el tipo de dígitos significativos para la salida de valores numéricos en este libro de trabajo. El valor predeterminado es [`SignificantDigitsType`](../../cellshelper/significantdigitstype/).

```csharp
public SignificantDigitsType SignificantDigitsType { get; set; }
```

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class WorkbookSettingsPropertySignificantDigitsTypeDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();

            // Acceder a WorkbookSettings
            WorkbookSettings settings = workbook.Settings;

            // Mostrar el valor actual de SignificantDigitsType
            Console.WriteLine("Current SignificantDigitsType: " + settings.SignificantDigitsType);

            // Demuestre la configuración de diferentes valores de SignificantDigitsType
            settings.SignificantDigitsType = SignificantDigitsType.Digits15;
            Console.WriteLine("After setting to Digits15: " + settings.SignificantDigitsType);

            settings.SignificantDigitsType = SignificantDigitsType.G17;
            Console.WriteLine("After setting to G17: " + settings.SignificantDigitsType);

            settings.SignificantDigitsType = SignificantDigitsType.Rounding17;
            Console.WriteLine("After setting to Rounding17: " + settings.SignificantDigitsType);

            // Agregue algunos datos numéricos para demostrar el efecto
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue(123.4567890123456789);
            worksheet.Cells["A2"].PutValue(9876543210.123456789);

            // Guarda el libro de trabajo
            workbook.Save("SignificantDigitsTypeDemo.xlsx");
            Console.WriteLine("Workbook saved with SignificantDigitsType settings.");
        }
    }
}
```

### Ver también

* enum [SignificantDigitsType](../../significantdigitstype/)
* class [WorkbookSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


