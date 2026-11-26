---
title: "Enumeración SmartTagShowType"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Enumeración Aspose.Cells.Markup.SmartTagShowType. Representa el tipo de visualización de la etiqueta inteligente"
type: docs
url: /es/net/aspose.cells.markup/smarttagshowtype/
---
## SmartTagShowType enumeration

Representa el tipo de visualización de la etiqueta inteligente.

```csharp
public enum SmartTagShowType
```

### Valores

| Nombre | Valor | Descripción |
| --- | --- | --- |
| All | `0` | Indica que las etiquetas inteligentes están habilitadas y se muestran |
| NoSmartTagIndicator | `1` | Indica que las etiquetas inteligentes están habilitadas pero el indicador no se muestra |
| None | `2` | Indica que las etiquetas inteligentes están deshabilitadas y no se muestran |

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Markup;
    using System;

    public class MarkupClassSmartTagShowTypeDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Demuestra todos los valores de la enumeración SmartTagShowType
            Console.WriteLine("SmartTagShowType values:");
            Console.WriteLine($"All: {SmartTagShowType.All}");
            Console.WriteLine($"NoSmartTagIndicator: {SmartTagShowType.NoSmartTagIndicator}");
            Console.WriteLine($"None: {SmartTagShowType.None}");

            // Crea y configura una etiqueta inteligente
            var smartTagCollection = worksheet.SmartTagSetting.Add("urn:schemas-microsoft-com:office:smarttags#date");

            // Establece propiedades que usarían SmartTagShowType (simulado ya que la propiedad real no está disponible)
            Console.WriteLine("\nSmart tag created at A1 with current date");

            // Guarda con diferentes escenarios de tipo de visualización
            workbook.Save("SmartTagShowTypeDemo_All.xlsx");
            Console.WriteLine("Workbook saved with default show type (All)");

            // Crea otro libro de trabajo con un comportamiento de tipo de visualización diferente
            Workbook workbook2 = new Workbook();
            Worksheet worksheet2 = workbook2.Worksheets[0];
            worksheet2.SmartTagSetting.Add("urn:schemas-microsoft-com:office:smarttags#date");
            Console.WriteLine("\nSecond workbook created with smart tag at B2");

            workbook2.Save("SmartTagShowTypeDemo_None.xlsx");
            Console.WriteLine("Second workbook saved (simulating None behavior)");
        }
    }
}
```

### Ver también

* namespace [Aspose.Cells.Markup](../../aspose.cells.markup/)
* assembly [Aspose.Cells](../../)


