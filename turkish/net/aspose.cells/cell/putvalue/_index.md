---
title: "Cell.PutValue"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Cell yöntemi. Boolean değeri hücreye koyar"
type: docs
url: /tr/net/aspose.cells/cell/putvalue/
---
## PutValue(bool) {#putvalue}

Hücreye bir mantıksal değer koyar.

```csharp
public void PutValue(bool boolValue)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| boolValue | Boolean |  |

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellMethodPutValueWithBooleanDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // B3 hücresine (satır 2, sütun 2) boolean değer koy
            cells[2, 2].PutValue(true);

            // Değerin doğru ayarlandığını doğrula
            Console.WriteLine("Cell B3 value: " + cells[2, 2].Value);
        }
    }
}
```

### Ayrıca Bakınız

* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## PutValue(int) {#putvalue_2}

Hücreye bir tam sayı değeri koyar.

```csharp
public void PutValue(int intValue)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| intValue | Int32 | Giriş değeri |

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellMethodPutValueWithInt32Demo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Cells cells = workbook.Worksheets[0].Cells;
            
            // Int32 parametrelerle PutValue kullanarak
            cells[0, 0].PutValue(10);
            cells[1, 0].PutValue(20);
            cells[2, 0].PutValue(30);
            
            // Değerlerin toplamını hesapla
            cells[3, 0].Formula = "=SUM(A1:A3)";
            workbook.CalculateFormula();
            
            Console.WriteLine("Sum of values: " + cells[3, 0].IntValue);
        }
    }
}
```

### Ayrıca Bakınız

* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## PutValue(double) {#putvalue_1}

Hücreye bir double değeri koyar.

```csharp
public void PutValue(double doubleValue)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| doubleValue | Double | Giriş değeri |

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellMethodPutValueWithDoubleDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Cells cells = workbook.Worksheets[0].Cells;
            
            // PutValue yöntemiyle double değerleri koy
            cells[0, 0].PutValue("Item");
            cells[0, 1].PutValue("Price");
            cells[1, 0].PutValue("Apple");
            cells[1, 1].PutValue(0.69);
            cells[2, 0].PutValue("Banana");
            cells[2, 1].PutValue(0.49);
            cells[3, 0].PutValue("Orange");
            cells[3, 1].PutValue(0.29);

            // Çalışma kitabını kaydedin
            workbook.Save("PutValueWithDoubleDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## PutValue(string, bool, bool) {#putvalue_7}

Hücreye bir değer koyar, uygun olduğunda değer başka bir veri tipine dönüştürülür ve hücrenin sayı biçimi sıfırlanır.

```csharp
public void PutValue(string stringValue, bool isConverted, bool setStyle)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| stringValue | String | Giriş değeri |
| isConverted | Boolean | Doğru: uygun ise başka veri tipine dönüştürüldü. |
| setStyle | Boolean | Doğru: başka veri tipine dönüştürürken sayı formatını hücrenin stiline ayarla |

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellMethodPutValueWithStringBooleanBooleanDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            
            // İlk çalışma sayfasına eriş
            Worksheet worksheet = workbook.Worksheets[0];
            
            // B3 hücresini al
            Cell cell = worksheet.Cells["B3"];
            
            // Yaş için veri doğrulamasını ayarla (pozitif sayı olmalı)
            Validation validation = cell.GetValidation();
            validation.Type = ValidationType.WholeNumber;
            validation.Operator = OperatorType.GreaterThan;
            validation.Formula1 = "0";
            
            // Dönüştürme ve doğrulama kontrolüyle değeri koy
            cell.PutValue("-60", true, false);
            
            // Formülleri hesapla (bu basit durumda gerekmese de)
            workbook.CalculateFormula();
            
            // Değerin geçerli olup olmadığını kontrol et
            bool isValid = cell.GetValidationValue();
            Console.WriteLine("Is value valid? " + isValid);
            
            // Çalışma kitabını kaydet
            workbook.Save("output.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## PutValue(string, bool) {#putvalue_6}

Hücreye bir dize değeri koyar ve uygun olduğunda değeri başka bir veri tipine dönüştürür.

```csharp
public void PutValue(string stringValue, bool isConverted)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| stringValue | String | Giriş değeri |
| isConverted | Boolean | Doğru: uygun ise başka veri tipine dönüştürüldü. |

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellMethodPutValueWithStringBooleanDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // PutValue'ı string ve boolean parametrelerle göster
            cells["B2"].PutValue("123", true);  // String value with conversion flag
            cells["C2"].PutValue("456", false); // String value without conversion
            
            // Değerleri doğrula
            Console.WriteLine("B2 value (converted): " + cells["B2"].Value); // Should show 123 as number
            Console.WriteLine("C2 value (raw): " + cells["C2"].Value);       // Should show "456" as string

            workbook.Save("PutValueDemo.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### Ayrıca Bakınız

* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## PutValue(string) {#putvalue_5}

Hücreye bir dize değeri koyar.

```csharp
public void PutValue(string stringValue)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| stringValue | String | Giriş değeri |

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellMethodPutValueWithStringDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Cells cells = workbook.Worksheets[0].Cells;
            
            // PutValue'yi string parametrelerle kullanma
            cells[0, 0].PutValue("Product");
            cells[0, 1].PutValue("Category");
            cells[0, 2].PutValue("Price");
            
            cells[1, 0].PutValue("Laptop");
            cells[1, 1].PutValue("Electronics");
            cells[1, 2].PutValue(999.99);
            
            cells[2, 0].PutValue("Desk Chair");
            cells[2, 1].PutValue("Furniture");
            cells[2, 2].PutValue(199.50);
            
            // Çalışma kitabını kaydedin
            workbook.Save("PutValueStringDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## PutValue(DateTime) {#putvalue_3}

Hücreye bir DateTime değeri koyar.

```csharp
public void PutValue(DateTime dateTime)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| dateTime | DateTime | Giriş değeri |

### Açıklamalar

Bir hücreye DateTime değeri ayarlamak, hücrenin otomatik olarak tarih-saat biçiminde olacağı anlamına gelmez. DateTime değeri, hem MS Excel hem de Aspose.Cells veri modelinde sayısal değer olarak tutulur. Sayısal değerin kendisi olarak mı yoksa tarih-saat olarak mı alınacağı, bu hücreye uygulanan sayı biçimine bağlıdır. Eğer bu hücre tarih-saat olarak biçimlendirilmemişse, girdiğiniz değer DateTime olsa bile sayısal değer olarak görüntülenecektir.

### Örnekler

Bu örnek, bir hücreye DateTime değeri nasıl ayarlanır ve tarih-saat olarak nasıl görüntülenir gösterir.

```csharp
[C#]

Workbook excel = new Workbook();
Cells cells = excel.Worksheets[0].Cells;

//DateTime'ı bir hücreye yerleştir
Cell cell = cells[0, 0];
cell.PutValue(new DateTime(2023, 5, 15));
Style style = cell.GetStyle(false);
style.Number = 14;
cell.SetStyle(style);
```

### Ayrıca Bakınız

* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## PutValue(object) {#putvalue_4}

Hücreye bir nesne değeri koyar.

```csharp
public void PutValue(object objectValue)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| objectValue | Object | girdi değeri |

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellMethodPutValueWithObjectDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Cells cells = workbook.Worksheets[0].Cells;
            
            // PutValue ile DateTime nesnesi
            DateTime dt = new DateTime(2008, 2, 2);
            cells[0, 0].PutValue((object)dt);
            
            // PutValue ile string nesnesi
            cells[1, 0].PutValue((object)"Hello World");
            
            // PutValue ile sayısal nesne
            cells[2, 0].PutValue((object)123.45);
            
            // Çalışma kitabını kaydedin
            workbook.Save("PutValueWithObjectDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


