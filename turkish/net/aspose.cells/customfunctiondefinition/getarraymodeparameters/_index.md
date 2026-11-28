---
title: "CustomFunctionDefinition.GetArrayModeParameters"
second_title: "Aspose.Cells için .NET API Referansı"
description: "CustomFunctionDefinition yöntemi. Dizi modunda hesaplanması gereken verilen özel fonksiyon parametrelerinin indekslerini alır"
type: docs
url: /tr/net/aspose.cells/customfunctiondefinition/getarraymodeparameters/
---
## CustomFunctionDefinition.GetArrayModeParameters method

Verilen özel fonksiyonun dizi modunda hesaplanması gereken parametre indekslerini alır.

```csharp
public virtual int[] GetArrayModeParameters(string functionName)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| functionName | String | Özel fonksiyonun adı. |

### Dönüş Değeri

Verilen özel fonksiyon için dizi modunda hesaplanması gereken parametrelerin indeksleri. Varsayılan değer null'dır, özel fonksiyon için dizi modunda hesaplanması gereken bir parametre yoktur.

### Açıklamalar

Hesaplanması gereken bir ifade için, A:A+B:B örneğini alalım: Genel olarak değer modunda, mevcut hücre temeline göre tek bir değere hesaplanır. Ancak dizi modunda, A1+B1, A2+B2, A3+B3, ... gibi tüm değerler hesaplanır ve hesaplama için kullanılır.

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CustomFunctionDefinitionMethodGetArrayModeParametersWithStringDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // CustomFunctionDefinition örneği oluştur
            CustomFunctionDefinition customFunction = new CustomFunctionDefinition();

            try
            {
                // GetArrayModeParameters'ı bir fonksiyon adı parametresiyle çağır
                string functionName = "SUM";
                int[] result = customFunction.GetArrayModeParameters(functionName);

                // Sonucu göster
                if (result != null)
                {
                    Console.WriteLine("Array mode parameters for function '{0}':", functionName);
                    foreach (int param in result)
                    {
                        Console.WriteLine(param);
                    }
                }
                else
                {
                    Console.WriteLine("No array mode parameters defined for function '{0}'", functionName);
                }
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetArrayModeParameters method: {ex.Message}");
            }

            // Çalışma kitabını kaydedin
            workbook.Save("CustomFunctionDefinitionGetArrayModeParametersDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [CustomFunctionDefinition](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


