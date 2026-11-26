---
title: "Style.IsModified"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método Style. Verifica si las propiedades especificadas del estilo han sido modificadas. Se usa para el estilo de ConditionalFormattings para comprobar si las propiedades especificadas de este estilo deben usarse al aplicar los ConditionalFormattings en una celda"
type: docs
url: /es/net/aspose.cells/style/ismodified/
---
## Style.IsModified method

Comprueba si las propiedades especificadas del estilo han sido modificadas. Se usa para el estilo de ConditionalFormattings para comprobar si las propiedades especificadas de este estilo deben usarse al aplicar ConditionalFormattings en una celda.

```csharp
public bool IsModified(StyleModifyFlag modifyFlag)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| modifyFlag | StyleModifyFlag | Banderas de estilo modificado |

### Valor de retorno

verdadero si las propiedades especificadas han sido modificadas

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class StyleMethodIsModifiedWithStyleModifyFlagDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            
            // Acceder a la primera hoja de cálculo
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Obtener el estilo de la celda A1
            Style style = worksheet.Cells["A1"].GetStyle();
            
            // Modificar el patrón (fondo) del estilo
            style.Pattern = BackgroundType.Solid;
            style.ForegroundColor = System.Drawing.Color.Yellow;
            
            // Comprobar si el patrón fue modificado
            bool isPatternModified = style.IsModified(StyleModifyFlag.Pattern);
            
            // Mostrar el resultado
            Console.WriteLine("Is pattern modified: " + isPatternModified);
        }
    }
}
```

### Ver también

* enum [StyleModifyFlag](../../stylemodifyflag/)
* class [Style](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


