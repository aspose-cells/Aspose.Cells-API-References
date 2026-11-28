---
title: "Cells.ImportArray"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Cells yöntemi."
type: docs
url: /tr/net/aspose.cells/cells/importarray/
---
## ImportArray(string[], int, int) {#importarray_4}

```csharp
public void ImportArray(string[] stringArray, int firstRow, int firstColumn)
```

### Ayrıca Bakınız

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## ImportArray(string[], int, int, bool) {#importarray_5}

Bir çalışma sayfasına string dizisini içe aktarır.

```csharp
public void ImportArray(string[] stringArray, int firstRow, int firstColumn, bool isVertical)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| stringArray | String[] | String dizisi. |
| firstRow | Int32 | İçe aktarılacak ilk hücrenin satır numarası. |
| firstColumn | Int32 | İçe aktarılacak ilk hücrenin sütun numarası. |
| isVertical | Boolean | Verinin dikey mi yoksa yatay mı aktarılacağını belirtir. |

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CellsMethodImportArrayWithStringInt32Int32BooleanDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // string dizi verisini hazırla
            string[] fruitArray = new string[] { "Apple", "Banana", "Cherry", "Date", "Elderberry" };

            try
            {
                // ImportArray'i şu parametrelerle çağır: (String[], Int32, Int32, Boolean)
                // İçe aktarmayı satır 2'de (3. satır), sütun 1'de (B sütunu), dikey olarak başlat
                worksheet.Cells.ImportArray(fruitArray, 2, 1, true);

                Console.WriteLine("Imported string array vertically starting from cell B3:");
                foreach (string fruit in fruitArray)
                {
                    Console.WriteLine(fruit);
                }
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing ImportArray method: {ex.Message}");
            }

            // Sonucu kaydet
            workbook.Save("CellsMethodImportArrayWithStringInt32Int32BooleanDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## ImportArray(int[], int, int) {#importarray_2}

```csharp
public void ImportArray(int[] intArray, int firstRow, int firstColumn)
```

### Ayrıca Bakınız

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## ImportArray(int[], int, int, bool) {#importarray_3}

Bir çalışma sayfasına integer dizisini içe aktarır.

```csharp
public void ImportArray(int[] intArray, int firstRow, int firstColumn, bool isVertical)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| intArray | Int32[] | Tam sayı dizisi. |
| firstRow | Int32 | İçe aktarılacak ilk hücrenin satır numarası. |
| firstColumn | Int32 | İçe aktarılacak ilk hücrenin sütun numarası. |
| isVertical | Boolean | Verinin dikey mi yoksa yatay mı aktarılacağını belirtir. |

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CellsMethodImportArrayWithInt32Int32Int32BooleanDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Int32 dizi verisini hazırla
            int[] data = new int[] { 1, 2, 3, 4, 5 };

            try
            {
                // ImportArray'i şu parametrelerle çağır: (Int32[], firstRow=2, firstColumn=1, isVertical=true)
                worksheet.Cells.ImportArray(data, 2, 1, true);

                Console.WriteLine("Imported array vertically starting from cell B3:");
                for (int i = 0; i < data.Length; i++)
                {
                    Console.WriteLine($"Cell B{3 + i}: {worksheet.Cells[2 + i, 1].Value}");
                }
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing ImportArray method: {ex.Message}");
            }

            // Sonucu kaydet
            workbook.Save("CellsMethodImportArrayWithInt32Int32Int32BooleanDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## ImportArray(double[], int, int) {#importarray}

```csharp
public void ImportArray(double[] doubleArray, int firstRow, int firstColumn)
```

### Ayrıca Bakınız

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## ImportArray(double[], int, int, bool) {#importarray_1}

Bir çalışma sayfasına double dizisini içe aktarır.

```csharp
public void ImportArray(double[] doubleArray, int firstRow, int firstColumn, bool isVertical)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| doubleArray | Double[] | Double dizisi. |
| firstRow | Int32 | İçe aktarılacak ilk hücrenin satır numarası. |
| firstColumn | Int32 | İçe aktarılacak ilk hücrenin sütun numarası. |
| isVertical | Boolean | Verinin dikey mi yoksa yatay mı aktarılacağını belirtir. |

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CellsMethodImportArrayWithDoubleInt32Int32BooleanDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Örnek double dizi verisini hazırla
            double[] dataArray = new double[] { 1.23, 4.56, 7.89, 10.11, 12.13 };
            const int targetRow = 2;    // 0-based row index (3rd row)
            const int targetColumn = 1; // 0-based column index (2nd column)
            const bool isVertical = true;

            try
            {
                // Hücre koleksiyonunu al ve ImportArray'i çağır
                Cells cells = worksheet.Cells;
                cells.ImportArray(dataArray, targetRow, targetColumn, isVertical);
                
                Console.WriteLine($"Imported {dataArray.Length} double values starting at row {targetRow + 1}, column {targetColumn + 1}");
                Console.WriteLine($"Data orientation: {(isVertical ? "Vertical" : "Horizontal")}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing ImportArray method: {ex.Message}");
            }
            
            // Sonucu kaydet
            workbook.Save("CellsImportArrayDoubleVerticalDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


