---
title: "CalculationOptions.CharacterEncoding"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad CalculationOptions. Especifica la codificación utilizada para codificar/decodificar caracteres al calcular fórmulas. Para funciones como CHAR CODE, el resultado calculado depende de la configuración regional y del conjunto de caracteres predeterminado del entorno. Con esta propiedad, el usuario puede especificar la codificación adecuada utilizada por esas funciones para obtener el resultado esperado"
type: docs
url: /es/net/aspose.cells/calculationoptions/characterencoding/
---
## CalculationOptions.CharacterEncoding property

Especifica la codificación utilizada para codificar/decodificar caracteres al calcular fórmulas. Para funciones como CHAR, CODE, el resultado calculado depende de la configuración regional y del juego de caracteres predeterminado del entorno. Con esta propiedad el usuario puede especificar la codificación adecuada para esas funciones y obtener el resultado esperado.

```csharp
public Encoding CharacterEncoding { get; set; }
```

### Ejemplos

```csharp
using System;
using System.Text;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CalculationOptionsPropertyCharacterEncodingDemo
    {
        public static void Run()
        {
            Workbook wb = new Workbook();
            Worksheet sheet = wb.Worksheets[0];
            wb.Settings.Region = CountryCode.Japan;
            
            CalculationOptions copts = new CalculationOptions();
            copts.CharacterEncoding = Encoding.GetEncoding("iso-2022-jp");
            
            string formula = "=TRIM(1)";
            string result = (string)sheet.CalculateFormula(formula, copts);
            
            Console.WriteLine("Calculation result: " + result);
        }
    }
}
```

### Ver también

* class [CalculationOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


