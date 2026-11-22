---
title: "DataModelConnection.ClassType"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية DataModelConnection. يحصل على نوع كائن ExternalConnection هذا"
type: docs
url: /ar/net/aspose.cells.externalconnections/datamodelconnection/classtype/
---
## DataModelConnection.ClassType property

يحصل على نوع هذا الكائن [`ExternalConnection`](../../externalconnection/).

```csharp
public override ExternalConnectionClassType ClassType { get; }
```

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.ExternalConnections;
    using Aspose.Cells.QueryTables;
    using System;
    using System.Runtime.Serialization;

    public class DataModelConnectionPropertyClassTypeDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            
            // إنشاء مثيل DataModelConnection باستخدام كائن غير مهيأ
            DataModelConnection connection = (DataModelConnection)FormatterServices.GetUninitializedObject(typeof(DataModelConnection));
            ((IList<ExternalConnection>)workbook.DataConnections).Add(connection);

            // عرض قيمة ClassType الحالية (خاصية قراءة‑فقط)
            Console.WriteLine("Current ClassType value: " + connection.ClassType);

            // إعداد خصائص الاتصال
            connection.Command = "SELECT * FROM Products";
            connection.CommandType = OLEDBCommandType.SqlStatement;
            connection.ConnectionString = "Provider=SQLOLEDB;Data Source=Northwind;Integrated Security=SSPI";

            // توضيح كيف يؤثر ClassType على معالجة الاتصال
            if (connection.ClassType == ExternalConnectionClassType.DataModel)
            {
                Console.WriteLine("This is a Data Model connection");
                // إضافة PowerQueryFormula لاتصال نموذج البيانات
                PowerQueryFormulaCollection queries = workbook.DataMashup.PowerQueryFormulas;
                string formulaDef = "let Source = Sql.Database(\"myServer\", \"myDB\") in Source";
                PowerQueryFormula query = (PowerQueryFormula)FormatterServices.GetUninitializedObject(typeof(PowerQueryFormula));
                query.Name = "ProductQuery";
                typeof(PowerQueryFormula).GetProperty("FormulaDefinition").SetValue(query, formulaDef);
                ((IList<PowerQueryFormula>)queries).Add(query);
            }

            // احفظ المصنف
            workbook.Save("DataModelConnectionClassTypeDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* enum [ExternalConnectionClassType](../../externalconnectionclasstype/)
* class [DataModelConnection](../)
* namespace [Aspose.Cells.ExternalConnections](../../../aspose.cells.externalconnections/)
* assembly [Aspose.Cells](../../../)


