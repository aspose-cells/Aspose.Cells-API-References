---
title: "NameCollection.Filter"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método NameCollection. Obtiene todos los nombres definidos por ámbito"
type: docs
url: /es/net/aspose.cells/namecollection/filter/
---
## NameCollection.Filter method

Obtiene todos los nombres definidos por ámbito.

```csharp
public Name[] Filter(NameScopeType type, int sheetIndex)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| type | NameScopeType | El tipo de ámbito. |
| sheetIndex | Int32 | El índice de hoja. Solo tiene efecto cuando el tipo de ámbito es Worksheet |

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class NameCollectionMethodFilterWithNameScopeTypeInt32Demo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            
            // Agregue algunos nombres al libro de trabajo y a las hojas de cálculo
            workbook.Worksheets.Names.Add("GlobalName");
            Worksheet worksheet1 = workbook.Worksheets[0];
            workbook.Worksheets.Names.Add("Sheet1Name");
            Worksheet worksheet2 = workbook.Worksheets.Add("Sheet2");
            workbook.Worksheets.Names.Add("Sheet2Name");

            // Filtre los nombres por tipo de ámbito e índice de hoja
            Name[] workbookScopeNames = workbook.Worksheets.Names.Filter(NameScopeType.Workbook, -1);
            Name[] worksheetScopeNames = workbook.Worksheets.Names.Filter(NameScopeType.Worksheet, -1);
            Name[] sheet1Names = workbook.Worksheets.Names.Filter(NameScopeType.Worksheet, 0);

            // Mostrar resultados
            Console.WriteLine($"Workbook-scoped names count: {workbookScopeNames.Length}");
            Console.WriteLine($"Worksheet-scoped names count: {worksheetScopeNames.Length}");
            Console.WriteLine($"Sheet1 names count: {sheet1Names.Length}");
        }
    }
}
```

### Ver también

* class [Name](../../name/)
* enum [NameScopeType](../../namescopetype/)
* class [NameCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


