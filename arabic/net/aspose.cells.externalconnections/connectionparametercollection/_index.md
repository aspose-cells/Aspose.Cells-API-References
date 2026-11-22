---
title: "الفئة ConnectionParameterCollection"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "الفئة Aspose.Cells.ExternalConnections.ConnectionParameterCollection. تحدد مجموعة ConnectionParameter"
type: docs
url: /ar/net/aspose.cells.externalconnections/connectionparametercollection/
---
## ConnectionParameterCollection class

تحدد مجموعة [`ConnectionParameter`](../connectionparameter/)

```csharp
public class ConnectionParameterCollection : CollectionBase<ConnectionParameter>
```

## الخصائص

| الاسم | الوصف |
| --- | --- |
| [Capacity](../../aspose.cells/collectionbase-1/capacity/) { get; set; } |  |
| [Count](../../aspose.cells/collectionbase-1/count/) { get; } |  |
| [Item](../../aspose.cells.externalconnections/connectionparametercollection/item/) { get; } | تحصل على عنصر [`ConnectionParameter`](../connectionparameter/) في الفهرس المحدد. (مؤشرين) |
| [Item](../../aspose.cells/collectionbase-1/item/) { get; set; } |  |

## الطرق

| الاسم | الوصف |
| --- | --- |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(ConnectionParameter) |  |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(ConnectionParameter, IComparer&lt;ConnectionParameter&gt;) |  |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(int, int, ConnectionParameter, IComparer&lt;ConnectionParameter&gt;) |  |
| [Clear](../../aspose.cells/collectionbase-1/clear/)() |  |
| [Contains](../../aspose.cells/collectionbase-1/contains/)(ConnectionParameter) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(ConnectionParameter[]) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(ConnectionParameter[], int) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(int, ConnectionParameter[], int, int) |  |
| [Exists](../../aspose.cells/collectionbase-1/exists/)(Predicate&lt;ConnectionParameter&gt;) |  |
| [Find](../../aspose.cells/collectionbase-1/find/)(Predicate&lt;ConnectionParameter&gt;) |  |
| [FindAll](../../aspose.cells/collectionbase-1/findall/)(Predicate&lt;ConnectionParameter&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(Predicate&lt;ConnectionParameter&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(int, Predicate&lt;ConnectionParameter&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(int, int, Predicate&lt;ConnectionParameter&gt;) |  |
| [FindLast](../../aspose.cells/collectionbase-1/findlast/)(Predicate&lt;ConnectionParameter&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(Predicate&lt;ConnectionParameter&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(int, Predicate&lt;ConnectionParameter&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(int, int, Predicate&lt;ConnectionParameter&gt;) |  |
| [GetEnumerator](../../aspose.cells/collectionbase-1/getenumerator/)() |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(ConnectionParameter) |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(ConnectionParameter, int) |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(ConnectionParameter, int, int) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(ConnectionParameter) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(ConnectionParameter, int) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(ConnectionParameter, int, int) |  |
| [RemoveAt](../../aspose.cells/collectionbase-1/removeat/)(int) |  |

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.ExternalConnections;
    using System;

    public class ExternalConnectionsClassConnectionParameterCollectionDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد للعرض
            Workbook workbook = new Workbook();
            
            try
            {
                // احصل على أول اتصال خارجي (سيتم إنشاؤه إذا لم يكن موجودًا)
                ExternalConnection connection = workbook.DataConnections[0];
                
                // احصل على مجموعة المعلمات من الاتصال
                ConnectionParameterCollection parameters = connection.Parameters;
                
                // عرض الوظيفة الأساسية عن طريق فحص خصائص المجموعة
                Console.WriteLine($"ConnectionParameterCollection count: {parameters.Count}");
                
                // محاولة الوصول إلى عنصر (سيكون فارغًا إذا كانت المجموعة فارغة)
                if (parameters.Count > 0)
                {
                    ConnectionParameter param = parameters[0];
                    Console.WriteLine(param == null ? "No parameters in collection" : "Parameter exists");
                }
                else
                {
                    Console.WriteLine("No parameters in collection");
                }
                
                // احفظ المصنف
                workbook.Save("ConnectionParameterCollectionDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error working with ConnectionParameterCollection: {ex.Message}");
            }
        }
    }
}
```

### انظر أيضًا

* class [CollectionBase&lt;T&gt;](../../aspose.cells/collectionbase-1/)
* class [ConnectionParameter](../connectionparameter/)
* namespace [Aspose.Cells.ExternalConnections](../../aspose.cells.externalconnections/)
* assembly [Aspose.Cells](../../)


