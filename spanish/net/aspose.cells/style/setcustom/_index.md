---
title: "Style.SetCustom"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método Style. Establece la cadena de formato numérico personalizado de una celda"
type: docs
url: /es/net/aspose.cells/style/setcustom/
---
## Style.SetCustom method

Establece la cadena de formato numérico personalizado de una celda.

```csharp
public void SetCustom(string custom, bool builtinPreference)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| personalizado | String | Cadena de formato numérico personalizado, debe ser un patrón InvariantCulture. |
| builtinPreference | Booleano | Si la cadena de formato numérico Custom coincide con uno de los formatos numéricos incorporados correspondientes a la configuración regional actual, indica si se debe establecer el formato numérico como incorporado en lugar de Custom. |

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class StyleMethodSetCustomWithStringBooleanDemo
    {
        public static void Run()
        {
            Workbook wb = new Workbook();
            wb.Settings.Region = CountryCode.USA;
            Style style = wb.CreateStyle();
            
            string customFormat1 = "_(\"$\"* #,##0.00_);_(\"$\"* (#,##0.00);_(\"$\"* \"-\"??_);_(@_)";
            style.SetCustom(customFormat1, true);
            Console.WriteLine("Custom format 1 applied. Style number: " + style.Number);

            string customFormat2 = "_($* #,##0.00_);_(\"$\"* (#,##0.00);_(\"$\"* \"-\"??_);_(@_)";
            style.SetCustom(customFormat2, true);
            Console.WriteLine("Custom format 2 applied. Style number: " + style.Number);

            string customFormat3 = "_($* #,##0.00_);_(\"$\"* (#,##0.00);_(\"$\"* -??_);_(@_)";
            style.SetCustom(customFormat3, true);
            Console.WriteLine("Custom format 3 applied. Style number: " + style.Number);
        }
    }
}
```

### Ver también

* class [Style](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


