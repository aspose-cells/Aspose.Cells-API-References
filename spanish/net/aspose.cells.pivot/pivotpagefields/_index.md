---
title: "Clase PivotPageFields"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Clase Aspose.Cells.Pivot.PivotPageFields. Representa los elementos de página pivot si la fuente de datos de la tabla dinámica es rangos de consolidación. Sólo puede contener hasta 4 elementos"
type: docs
url: /es/net/aspose.cells.pivot/pivotpagefields/
---
## PivotPageFields class

Representa los elementos de página de tabla dinámica si la fuente de datos de la tabla dinámica son rangos de consolidación. Sólo puede contener hasta 4 elementos.

```csharp
public class PivotPageFields
```

## Constructores

| Nombre | Descripción |
| --- | --- |
| [PivotPageFields](pivotpagefields/)() | Representa los elementos de campo de página pivot. |

## Propiedades

| Nombre | Descripción |
| --- | --- |
| [PageFieldCount](../../aspose.cells.pivot/pivotpagefields/pagefieldcount/) { get; } | Obtiene el número de campos de página. |

## Métodos

| Nombre | Descripción |
| --- | --- |
| [AddIdentify](../../aspose.cells.pivot/pivotpagefields/addidentify/)(int, int[]) | Establece qué etiqueta de elemento en cada campo de página usar para identificar el rango de datos. pageItemIndex.Length debe ser igual a PageFieldCount, así que por favor agregue primero el campo de página. |
| [AddPageField](../../aspose.cells.pivot/pivotpagefields/addpagefield/)(string[]) | Agrega un campo de página. |

### Ejemplos

```csharp
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotClassPivotPageFieldsDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            
            Worksheet sheet1 = workbook.Worksheets[0];
            sheet1.Name = "Sheet1";
            FillData(sheet1);

            Worksheet sheet2 = workbook.Worksheets.Add("Sheet2");
            FillData(sheet2);

            Worksheet pivotSheet = workbook.Worksheets.Add("PivotSheet");
            PivotTableCollection pivotTables = pivotSheet.PivotTables;

            string[] src = { "=Sheet1!A1:C8", "=Sheet2!A1:C8" };
            PivotPageFields pageFields = new PivotPageFields();

            pageFields.AddPageField(new string[] { "item1", "item2" });
            pageFields.AddPageField(new string[] { "item3", "item4" });

            pageFields.AddIdentify(0, new int[] { 0, 1 });
            pageFields.AddIdentify(1, new int[] { 1, -1 });

            pivotTables.Add(src, false, pageFields, "E3", "PivotTable1");

            workbook.Save("output.xlsx", SaveFormat.Xlsx);
        }

        private static void FillData(Worksheet sheet)
        {
            Cells cells = sheet.Cells;
            cells["A1"].PutValue("Category");
            cells["B1"].PutValue("Value");
            cells["C1"].PutValue("Date");

            for (int i = 1; i < 8; i++)
            {
                cells[$"A{i+1}"].PutValue($"Item{i}");
                cells[$"B{i+1}"].PutValue(i * 100);
                cells[$"C{i+1}"].PutValue(System.DateTime.Now.AddDays(i).ToString("yyyy-MM-dd"));
            }
        }
    }
}
```

### Ver también

* namespace [Aspose.Cells.Pivot](../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../)


