---
title: "PivotTable.AddFieldToArea"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод PivotTable. Добавляет поле в конкретную область"
type: docs
url: /ru/net/aspose.cells.pivot/pivottable/addfieldtoarea/
---
## AddFieldToArea(PivotFieldType, string) {#addfieldtoarea_2}

Добавляет поле в указанную область.

```csharp
public int AddFieldToArea(PivotFieldType fieldType, string fieldName)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| fieldType | PivotFieldType | Тип области полей. |
| fieldName | String | Имя в базовых полях. |

### Возвращаемое значение

Позиция поля в конкретных полях. Если поле с таким именем отсутствует, возвращается -1.

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotTableMethodAddFieldToAreaWithPivotFieldTypeStringDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Добавить примерные данные для сводной таблицы
            Cells cells = sheet.Cells;
            cells["A1"].Value = "Product";
            cells["B1"].Value = "Region";
            cells["C1"].Value = "Sales";
            cells["A2"].Value = "P1";
            cells["B2"].Value = "North";
            cells["C2"].Value = 1000;
            cells["A3"].Value = "P2";
            cells["B3"].Value = "South";
            cells["C3"].Value = 1500;
            cells["A4"].Value = "P3";
            cells["B4"].Value = "East";
            cells["C4"].Value = 2000;
            cells["A5"].Value = "P1";
            cells["B5"].Value = "West";
            cells["C5"].Value = 1200;

            // Добавить сводную таблицу
            int index = sheet.PivotTables.Add("A1:C5", "E3", "PivotTable1");
            PivotTable pivot = sheet.PivotTables[index];

            // Добавьте поля в разные области, используя AddFieldToArea со строковыми именами полей
            pivot.AddFieldToArea(PivotFieldType.Row, "Product");
            pivot.AddFieldToArea(PivotFieldType.Column, "Region");
            pivot.AddFieldToArea(PivotFieldType.Data, "Sales");

            // Обновить и вычислить сводную таблицу
            pivot.RefreshData();
            pivot.CalculateData();

            // Сохраните книгу
            workbook.Save("PivotTableDemo_out.xlsx");
        }
    }
}
```

### См. также

* enum [PivotFieldType](../../pivotfieldtype/)
* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)

---

## AddFieldToArea(PivotFieldType, int) {#addfieldtoarea_1}

Добавляет поле в указанную область.

```csharp
public int AddFieldToArea(PivotFieldType fieldType, int baseFieldIndex)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| fieldType | PivotFieldType | Тип области полей. |
| baseFieldIndex | Int32 | Индекс в базовых полях. |

### Возвращаемое значение

Позиция поля в конкретных полях.

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotTableMethodAddFieldToAreaWithPivotFieldTypeInt32Demo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавить примерные данные для PivotTable
            worksheet.Cells["A1"].PutValue("Product");
            worksheet.Cells["B1"].PutValue("Region");
            worksheet.Cells["C1"].PutValue("Sales");
            
            for (int i = 2; i <= 10; i++)
            {
                worksheet.Cells["A" + i].PutValue("Product " + (i % 3 + 1));
                worksheet.Cells["B" + i].PutValue("Region " + (i % 2 + 1));
                worksheet.Cells["C" + i].PutValue(i * 100);
            }

            // Добавить сводную таблицу
            int pivotTableIndex = worksheet.PivotTables.Add("=A1:C10", "E3", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[pivotTableIndex];

            // Добавить поля в области, используя AddFieldToArea(PivotFieldType, Int32)
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0); // Product as row field
            pivotTable.AddFieldToArea(PivotFieldType.Column, 1); // Region as column field
            pivotTable.AddFieldToArea(PivotFieldType.Data, 2); // Sales as data field

            // Сохраните книгу
            workbook.Save("PivotTableDemo_out.xlsx");
        }
    }
}
```

### См. также

* enum [PivotFieldType](../../pivotfieldtype/)
* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)

---

## AddFieldToArea(PivotFieldType, PivotField) {#addfieldtoarea}

Добавляет поле в указанную область.

```csharp
public int AddFieldToArea(PivotFieldType fieldType, PivotField pivotField)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| fieldType | PivotFieldType | тип области полей. |
| pivotField | PivotField | поле в базовых полях. |

### Возвращаемое значение

позиция поля в конкретных полях.

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotTableMethodAddFieldToAreaWithPivotFieldTypePivotFieldDemo
    {
        public static void Run()
        {
            // Создать книгу
            Workbook workbook = new Workbook();
            
            // Добавить лист с исходными данными
            Worksheet sourceSheet = workbook.Worksheets[0];
            sourceSheet.Name = "Source Data";
            
            // Добавьте примерные данные
            sourceSheet.Cells["A1"].PutValue("Product");
            sourceSheet.Cells["B1"].PutValue("Region");
            sourceSheet.Cells["C1"].PutValue("Sales");
            
            sourceSheet.Cells["A2"].PutValue("Product A");
            sourceSheet.Cells["B2"].PutValue("North");
            sourceSheet.Cells["C2"].PutValue(1000);
            
            sourceSheet.Cells["A3"].PutValue("Product B");
            sourceSheet.Cells["B3"].PutValue("South");
            sourceSheet.Cells["C3"].PutValue(2000);
            
            sourceSheet.Cells["A4"].PutValue("Product A");
            sourceSheet.Cells["B4"].PutValue("East");
            sourceSheet.Cells["C4"].PutValue(1500);
            
            sourceSheet.Cells["A5"].PutValue("Product B");
            sourceSheet.Cells["B5"].PutValue("West");
            sourceSheet.Cells["C5"].PutValue(2500);

            // Добавить сводную таблицу
            Worksheet pivotSheet = workbook.Worksheets.Add("PivotTable");
            PivotTableCollection pivotTables = pivotSheet.PivotTables;
            string source = "='Source Data'!A1:C5";
            int index = pivotTables.Add(source, "A1", "PivotTable");
            PivotTable pTable = pivotTables[index];

            // Добавить поля в области
            pTable.AddFieldToArea(PivotFieldType.Row, 0); // Product
            pTable.AddFieldToArea(PivotFieldType.Row, 1); // Region
            
            // Добавить поле данных
            pTable.AddFieldToArea(PivotFieldType.Data, "Sales");
            pTable.DataFields[0].Function = ConsolidationFunction.Sum;
            pTable.DataFields[0].NumberFormat = "$0.00";

            // Добавить поле данных в область столбцов, используя параметр PivotField
            if (pTable.DataField != null)
            {
                pTable.AddFieldToArea(PivotFieldType.Column, pTable.DataField);
            }

            // Сохраните книгу
            workbook.Save("PivotTableDemo.xlsx");
        }
    }
}
```

### См. также

* enum [PivotFieldType](../../pivotfieldtype/)
* class [PivotField](../../pivotfield/)
* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


