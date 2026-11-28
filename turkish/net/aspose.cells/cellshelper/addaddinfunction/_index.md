---
title: "CellsHelper.AddAddInFunction"
second_title: "Aspose.Cells için .NET API Referansı"
description: "CellsHelper yöntemi. Eklenti işlevi ekle"
type: docs
url: /tr/net/aspose.cells/cellshelper/addaddinfunction/
---
## CellsHelper.AddAddInFunction method

Eklenti işlevi ekle.

```csharp
[Obsolete("Use WorksheetCollection.RegisterAddInFunction() methods instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public static void AddAddInFunction(string function, int minCountOfParameters, 
    int maxCountOfParameters, ParameterType[] paramersType, ParameterType functionValueType)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| fonksiyon | String | Fonksiyon adı. |
| minCountOfParameters | Int32 | Bu fonksiyonun gerektirdiği minimum parametre sayısı |
| maxCountOfParameters | Int32 | Bu fonksiyonun izin verdiği maksimum parametre sayısı. |
| paramersType | ParameterType[] | Fonksiyonun beklenen parametre tipi. |
| functionValueType | ParameterType | Fonksiyon değer tipi. |

### Açıklamalar

NOTE: Bu üye artık kullanımdan kaldırılmıştır. Bunun yerine lütfen WorksheetCollection.RegisterAddInFunction() yöntemlerini kullanın. Bu yöntem, Ocak 2022'den itibaren 12 ay sonra kaldırılacaktır. Aspose, yaşadığınız herhangi bir rahatsızlık için özür diler.

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CellsHelperMethodAddAddInFunctionWithStringInt32Int32ParameterTypeDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            try
            {
                // AddAddInFunction için parametreleri tanımla
                string functionName = "CUSTOMFUNCTION";
                int minParams = 2;
                int maxParams = 4;
                ParameterType[] paramTypes = new ParameterType[] { ParameterType.Value, ParameterType.Reference };
                ParameterType returnType = ParameterType.Value;

                // AddAddInFunction yöntemini çağır
                CellsHelper.AddAddInFunction(functionName, minParams, maxParams, paramTypes, returnType);

                // Özel fonksiyonu bir hücrede kullan
                worksheet.Cells["A1"].Formula = "=CUSTOMFUNCTION(5,B2)";
                worksheet.Cells["B2"].Value = 10;

                // Formülleri hesapla
                workbook.CalculateFormula();

                Console.WriteLine("AddAddInFunction executed successfully. Custom function added and used in A1.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing AddAddInFunction method: {ex.Message}");
            }

            // Sonucu kaydet
            workbook.Save("AddAddInFunctionDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* enum [ParameterType](../../parametertype/)
* class [CellsHelper](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


