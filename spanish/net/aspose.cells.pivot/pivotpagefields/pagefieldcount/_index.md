---
title: "PivotPageFields.PageFieldCount"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad PivotPageFields. Obtiene el número de campos de página"
type: docs
url: /es/net/aspose.cells.pivot/pivotpagefields/pagefieldcount/
---
## PivotPageFields.PageFieldCount property

Obtiene el número de campos de página.

```csharp
public int PageFieldCount { get; }
```

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class PivotPageFieldsPropertyPageFieldCountDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();

            // Crear hojas de cálculo de ejemplo con datos
            Worksheet sheet1 = workbook.Worksheets[0];
            sheet1.Name = "Data1";
            FillSampleData(sheet1);

            Worksheet sheet2 = workbook.Worksheets.Add("Data2");
            FillSampleData(sheet2);

            // Crear una hoja dinámica
            Worksheet pivotSheet = workbook.Worksheets.Add("PivotSheet");

            // Crear instancia de PivotPageFields
            PivotPageFields pageFields = new PivotPageFields();

            // Agregar campos de página para demostrar la propiedad PageFieldCount
            pageFields.AddPageField(new string[] { "Category1", "Category2" });
            pageFields.AddPageField(new string[] { "Region1", "Region2" });

            try
            {
                // Mostrar el valor de la propiedad PageFieldCount
                Console.WriteLine("Number of page fields: " + pageFields.PageFieldCount);

                // Agregar identificación para los campos de página
                pageFields.AddIdentify(0, new int[] { 0, 1 });
                pageFields.AddIdentify(1, new int[] { 1, 0 });

                // Verificar que el recuento permanezca igual después de agregar identificaciones
                Console.WriteLine("PageFieldCount after adding identifications: " + pageFields.PageFieldCount);

                // Crear tabla dinámica usando los campos de página
                string[] sources = { "=Data1!A1:C4", "=Data2!A1:C4" };
                pivotSheet.PivotTables.Add(sources, false, pageFields, "E3", "DemoPivot");

                // Guarda el libro de trabajo
                workbook.Save("PageFieldCountDemo.xlsx");
                Console.WriteLine("Demo completed successfully. File saved.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }

        private static void FillSampleData(Worksheet sheet)
        {
            Cells cells = sheet.Cells;
            cells["A1"].PutValue("Category");
            cells["B1"].PutValue("Region");
            cells["C1"].PutValue("Value");

            cells["A2"].PutValue("Category1");
            cells["B2"].PutValue("Region1");
            cells["C2"].PutValue(100);

            cells["A3"].PutValue("Category2");
            cells["B3"].PutValue("Region2");
            cells["C3"].PutValue(200);
        }
    }
}
```

### Ver también

* class [PivotPageFields](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


