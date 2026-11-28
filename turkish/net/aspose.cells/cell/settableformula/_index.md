---
title: "Cell.SetTableFormula"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Cell yöntemi. Bu hücreden başlayan verilen aralık için iki değişkenli veri tablosu oluştur"
type: docs
url: /tr/net/aspose.cells/cell/settableformula/
---
## SetTableFormula(int, int, string, string, object[][]) {#settableformula_3}

Bu hücreden başlayarak verilen aralık için iki değişkenli veri tablosu oluştur.

```csharp
public void SetTableFormula(int rowNumber, int columnNumber, string rowInputCell, 
    string columnInputCell, object[][] values)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| rowNumber | Int32 | Formülü doldurmak için satır sayısı. |
| columnNumber | Int32 | Formülü doldurmak için sütun sayısı. |
| rowInputCell | String | satır giriş hücresi |
| columnInputCell | String | sütun giriş hücresi |
| değerler | Object[][] | tablo formül aralığındaki hücreler için değerler |

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CellMethodSetTableFormulaWithInt32Int32StringStringObjectArrayDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            Cells cells = workbook.Worksheets[0].Cells;
            cells[1, 1].Formula = "=A1+A2";

            cells[1, 2].PutValue(2);
            cells[1, 3].PutValue(3);
            cells[2, 1].PutValue(2);
            cells[3, 1].PutValue(3);
            cells[4, 1].PutValue(4);

            // Tablo formülünün ayarlanacağı hedef hücre
            Cell targetCell = worksheet.Cells["C3"];

            // SetTableFormula için parametreleri hazırla
            int rowNumber = 3;
            int columnNumber = 2;
            string rowInputCell = "A1";
            string columnInputCell = "A2";
            object[][] values = new object[][]
            {
                new object[] { 1, 2 },    // Row 1 data
                new object[] { 3, 4 },    // Row 2 data
                new object[] { 5, 6 }     // Row 3 data
            };

            try
            {
                // Hedef hücreye tablo formülünü ayarla
                targetCell.SetTableFormula(rowNumber, columnNumber, rowInputCell, columnInputCell, values);

                // Sonuçları yenilemek için çalışma kitabı formüllerini hesapla
                workbook.CalculateFormula();

                Console.WriteLine("Table formula set successfully. Check D1:" + targetCell.StringValue);
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error setting table formula: {ex.Message}");
            }

            // Değiştirilmiş çalışma kitabını kaydet
            workbook.Save("SetTableFormulaDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## SetTableFormula(int, int, string, bool, object[][]) {#settableformula_2}

Bu hücreden başlayarak verilen aralık için tek değişkenli veri tablosu oluştur.

```csharp
public void SetTableFormula(int rowNumber, int columnNumber, string inputCell, bool isRowInput, 
    object[][] values)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| rowNumber | Int32 | Formülü doldurmak için satır sayısı. |
| columnNumber | Int32 | Formülü doldurmak için sütun sayısı. |
| inputCell | String | giriş hücresi |
| isRowInput | Boolean | Giriş hücresinin satır giriş hücresi (true) mı yoksa sütun giriş hücresi (false) mı olduğunu gösterir. |
| değerler | Object[][] | tablo formül aralığındaki hücreler için değerler |

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CellMethodSetTableFormulaWithInt32Int32StringBooleanObjectDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluşturun ve ilk çalışma sayfasına erişin
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            Cells cells = worksheet.Cells;
            cells[1, 1].Formula = "=A1+A2";

            cells[1, 2].PutValue(100000);
            cells[1, 3].PutValue(0.05);
            cells[1, 4].PutValue(2);
            cells[2, 1].PutValue(360);
            cells[3, 1].PutValue(30);
            cells[4, 1].PutValue(40);
            
            try
            {
                // SetTableFormula için parametreleri hazırla
                int rowCount = 3;
                int colCount = 3;
                object[][] inputValues = new object[][] 
                {
                    new object[] { 0.05, 0.06, 0.07 },
                    new object[] { 1000, 2000, 3000 },
                    new object[] { 100, 200, 300 }
                };

                // Veri tablosu için hedef hücreyi al (C3)
                Cell tableCell = worksheet.Cells["C3"];
                // Faiz oranı varyasyonlarıyla SetTableFormula'yu çağır
                tableCell.SetTableFormula(
                    rowNumber: rowCount,
                    columnNumber: colCount,
                    inputCell: "A1",
                    isRowInput: true,
                    values: inputValues
                );

                // Tablo sonuçlarını yenilemek için formülleri hesapla
                workbook.CalculateFormula();

                Console.WriteLine("Data table created successfully with varying interest rates");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error creating data table: {ex.Message}");
            }

            // Değiştirilmiş çalışma kitabını kaydet
            workbook.Save("SetTableFormulaDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## SetTableFormula(int, int, int, int, int, int, object[][]) {#settableformula_1}

Bu hücreden başlayarak verilen aralık için iki değişkenli veri tablosu oluştur.

```csharp
public void SetTableFormula(int rowNumber, int columnNumber, int rowIndexOfRowInputCell, 
    int columnIndexOfRowInputCell, int rowIndexOfColumnInputCell, int columnIndexOfColumnInputCell, 
    object[][] values)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| rowNumber | Int32 | Formülü doldurmak için satır sayısı. |
| columnNumber | Int32 | Formülü doldurmak için sütun sayısı. |
| rowIndexOfRowInputCell | Int32 | satır giriş hücresinin satır indeksi |
| columnIndexOfRowInputCell | Int32 | satır giriş hücresinin sütun indeksi |
| rowIndexOfColumnInputCell | Int32 | sütun giriş hücresinin satır indeksi |
| columnIndexOfColumnInputCell | Int32 | sütun giriş hücresinin sütun indeksi |
| değerler | Object[][] | tablo formül aralığındaki hücreler için değerler |

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CellMethodSetTableFormulaWithInt32Int32Int32Int32Int32Int32Demo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Cells cells = workbook.Worksheets[0].Cells;
            cells[1, 1].Formula = "=A1+A2";

            cells[1, 2].PutValue(2);
            cells[1, 3].PutValue(3);
            cells[1, 4].PutValue(4);
            cells[2, 1].PutValue(2);
            cells[3, 1].PutValue(3);
            cells[4, 1].PutValue(4);
            
            Cell formulaCell = cells[2, 2];

            // Veri tablosu için giriş değerlerini hazırlayın (faiz oranları ve kredi tutarları)
            object[][] tableValues = new object[3][];
            tableValues[0] = new object[] { 0.05, 0.06, 0.07 };
            tableValues[1] = new object[] { 1000, 2000, 3000 };
            tableValues[2] = new object[] { 100, 200, 300 };

            try
            {
                // Tablo formülünü 3x3 veri tablosu boyutları ve giriş hücresi ofsetleriyle ayarlayın
                formulaCell.SetTableFormula(
                    rowNumber: 3,
                    columnNumber: 3,
                    rowIndexOfRowInputCell: 0,  
                    columnIndexOfRowInputCell: 0,   
                    rowIndexOfColumnInputCell: 1,   
                    columnIndexOfColumnInputCell: 0, 
                    values: tableValues
                );

                workbook.CalculateFormula();
                Console.WriteLine("Data table formula set successfully. Check B2:D4 in output.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error setting table formula: {ex.Message}");
            }

            workbook.Save("CellTableFormulaDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## SetTableFormula(int, int, int, int, bool, object[][]) {#settableformula}

Bu hücreden başlayarak verilen aralık için tek değişkenli veri tablosu oluştur.

```csharp
public void SetTableFormula(int rowNumber, int columnNumber, int rowIndexOfInputCell, 
    int columnIndexOfInputCell, bool isRowInput, object[][] values)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| rowNumber | Int32 | Formülü doldurmak için satır sayısı. |
| columnNumber | Int32 | Formülü doldurmak için sütun sayısı. |
| rowIndexOfInputCell | Int32 | giriş hücresinin satır indeksi |
| columnIndexOfInputCell | Int32 | giriş hücresinin sütun indeksi |
| isRowInput | Boolean | Giriş hücresinin satır giriş hücresi (true) mı yoksa sütun giriş hücresi (false) mı olduğunu gösterir. |
| değerler | Object[][] | tablo formül aralığındaki hücreler için değerler |

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CellMethodSetTableFormulaWithInt32Int32Int32Int32BooleanObjDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluşturun ve ilk çalışma sayfasına erişin
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            Cells cells = workbook.Worksheets[0].Cells;
            cells[1, 1].Formula = "=A1+A2";

            cells[1, 2].PutValue(20);
            cells[1, 3].PutValue(30);            
            cells[2, 1].PutValue(20);
            cells[3, 1].PutValue(30);
            cells[4, 1].PutValue(40);

            // Tablo formülü parametreleri için örnek veri dizisi oluşturun
            object[][] inputValues = new object[][]
            {
                new object[] { 10, 20 },
                new object[] { 30, 40 },
                new object[] { 50, 60 }
            };

            // Tablo formülünü uygulamak için hedef hücreyi alın
            Cell formulaCell = worksheet.Cells[2, 2];

            try
            {
                // Tablo formülünü şununla ayarlayın: 
                // 3 satır, 2 sütun, giriş hücresi A1 (0,0), 
                // satır giriş tipi ve örnek değerler
                formulaCell.SetTableFormula(
                    rowNumber: 3,
                    columnNumber: 2,
                    rowIndexOfInputCell: 0,
                    columnIndexOfInputCell: 0,
                    isRowInput: true,
                    values: inputValues
                );

                workbook.CalculateFormula();
                Console.WriteLine("Table formula applied successfully. " + 
                    "Saved workbook with 3x2 table formula at C3.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error setting table formula: {ex.Message}");
            }

            // Değiştirilmiş çalışma kitabını kaydet
            workbook.Save("TableFormulaDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


