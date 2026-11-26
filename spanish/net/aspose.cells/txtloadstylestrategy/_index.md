---
title: "Enumeración TxtLoadStyleStrategy"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Enumeración Aspose.Cells.TxtLoadStyleStrategy. Especifica cómo aplicar estilo a los valores analizados al convertir una cadena a número o fecha y hora"
type: docs
url: /es/net/aspose.cells/txtloadstylestrategy/
---
## TxtLoadStyleStrategy enumeration

Especifica cómo aplicar el estilo a los valores analizados al convertir una cadena a número o fecha y hora.

```csharp
public enum TxtLoadStyleStrategy
```

### Valores

| Nombre | Valor | Descripción |
| --- | --- | --- |
| None | `0` | No establece estilo para el valor analizado. |
| BuiltIn | `1` | Establezca el estilo como número/fecha y hora incorporado cuando el valor analizado sea un valor numérico/fecha y hora simple. |
| ExactFormat | `2` | Establezca el formato personalizado exacto para el valor analizado para que el valor formateado sea igual al valor de entrada original. |

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class TxtLoadStyleStrategyDemo
    {
        public static void TxtLoadStyleStrategyExample()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Defina un contenido CSV de ejemplo
            string csvContent = "Name,Date,Value\nJohn,2023-01-01,100\nDoe,2023-01-02,200";

            // Guarde el contenido CSV en un archivo temporal
            string tempCsvFilePath = "sample.csv";
            System.IO.File.WriteAllText(tempCsvFilePath, csvContent);

            // Cree TxtLoadOptions y establezca LoadStyleStrategy
            TxtLoadOptions loadOptions = new TxtLoadOptions();
            loadOptions.LoadStyleStrategy = TxtLoadStyleStrategy.ExactFormat;

            // Cargue el archivo CSV en el libro de trabajo
            workbook = new Workbook(tempCsvFilePath, loadOptions);

            // Guarda el libro de trabajo en un archivo Excel
            workbook.Save("TxtLoadStyleStrategyExample.xlsx");

            // Limpie el archivo CSV temporal
            System.IO.File.Delete(tempCsvFilePath);

            Console.WriteLine("Workbook created and saved successfully.");
        }
    }
}
```

### Ver también

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


