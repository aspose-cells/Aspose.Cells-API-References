---
title: "CalculationOptions.LinkedDataSources"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad CalculationOptions. Especifica las fuentes de datos para enlaces externos utilizados en fórmulas"
type: docs
url: /es/net/aspose.cells/calculationoptions/linkeddatasources/
---
## CalculationOptions.LinkedDataSources property

Especifica las fuentes de datos para los enlaces externos utilizados en fórmulas.

```csharp
public Workbook[] LinkedDataSources { get; set; }
```

### Observaciones

Al igual que [`UpdateLinkedDataSource`](../../workbook/updatelinkeddatasource/), aquí puede especificar fuentes de datos para enlaces externos utilizados en fórmulas que se van a calcular, especialmente los que se usan en la función INDIRECT. Para esos enlaces externos usados en la función INDIRECT, no se consideran parte de los enlaces externos del libro de trabajo y no pueden actualizarse mediante [`UpdateLinkedDataSource`](../../workbook/updatelinkeddatasource/). La coincidencia de esos libros de trabajo con enlaces externos se determina por [`FileName`](../../workbook/filename/) y [`DataSource`](../../externallink/datasource/). Por lo tanto, asegúrese de que [`FileName`](../../workbook/filename/) haya sido especificado con el valor adecuado (generalmente debería ser el mismo que el [`DataSource`](../../externallink/datasource/) correspondiente) para cada libro de trabajo, de modo que puedan enlazarse como se espera.

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CalculationOptionsPropertyLinkedDataSourcesDemo
    {
        public static void Run()
        {
            // Crear un libro de trabajo externo con datos
            Workbook wbExt = new Workbook();
            wbExt.Worksheets[0].Cells["A2"].PutValue(100);
            wbExt.Worksheets.Add("Sheet2").Cells["A2"].PutValue(200);
            
            // Agregar rangos nombrados en el libro de trabajo externo
            int nameIndex1 = wbExt.Worksheets.Names.Add("Sheet1!ExtNamedRange1");
            wbExt.Worksheets.Names[nameIndex1].RefersTo = "=Sheet1!$A$2";
            int nameIndex2 = wbExt.Worksheets.Names.Add("Sheet2!ExtNamedRange2");
            wbExt.Worksheets.Names[nameIndex2].RefersTo = "=Sheet2!$A$2";
            int nameIndex3 = wbExt.Worksheets.Names.Add("GlobalNamedRange");
            wbExt.Worksheets.Names[nameIndex3].RefersTo = "=Sheet1!$A$2";

            // Crear el libro de trabajo principal
            Workbook wb = new Workbook();
            Worksheet sheet = wb.Worksheets[0];
            
            // Establecer fórmulas que hacen referencia al libro de trabajo externo
            sheet.Cells["A1"].Formula = "=[External.xlsx]Sheet1!$A$2";
            sheet.Cells["A2"].Formula = "=INDIRECT(\"[External.xlsx]Sheet1!$A$2\")";
            sheet.Cells["A3"].Formula = "=INDIRECT(\"[External.xlsx]Sheet1!ExtNamedRange1\")";
            sheet.Cells["A4"].Formula = "=INDIRECT(\"[External.xlsx]!GlobalNamedRange\")";

            // Calcular fórmulas usando LinkedDataSources
            CalculationOptions options = new CalculationOptions();
            options.LinkedDataSources = new Workbook[] { wbExt };
            
            Console.WriteLine("Before calculation:");
            PrintCellValues(sheet);

            wb.CalculateFormula(options);
            
            Console.WriteLine("\nAfter calculation:");
            PrintCellValues(sheet);
        }

        private static void PrintCellValues(Worksheet sheet)
        {
            for (int i = 0; i < 4; i++)
            {
                Console.WriteLine($"Cell A{i+1}: {sheet.Cells[$"A{i+1}"].StringValue}");
            }
        }
    }
}
```

### Ver también

* class [Workbook](../../workbook/)
* class [CalculationOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


