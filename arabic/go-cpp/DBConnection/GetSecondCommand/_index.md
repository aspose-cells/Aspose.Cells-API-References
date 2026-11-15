---
title: "طريقة GetSecondCommand"
linktitle: "GetSecondCommand"
second_title: "مرجع API لـ Aspose.Cells for Go عبر C++"
description: "طريقة GetSecondCommand. تغلف الدالة التي تمثل getsecondcommand في Go."
type: docs
weight: 200
url: /ar/go-cpp/dbconnection/getsecondcommand/
---

## GetSecondCommand function

يحدد سلسلة نص أمر ثانية تُحفظ عندما تكون حقول صفحة PivotTable المستندة إلى الخادم قيد الاستخدام. بالنسبة لاتصالات ODBC، عادةً ما يكون serverCommand استعلامًا أوسع من command (لا توجد جملة WHERE في الأول). بناءً على هذين الأمرين (Command و ServerCommand)، يمكن ملء واجهة المستخدم للمعلمات وإنشاء استعلامات معلمة.

```go

func (instance *DBConnection) GetSecondCommand()  (string,  error) 

```

## ملاحظات


## انظر أيضًا

* Class [DBConnection](../)
* Library [Aspose.Cells for Go](../../)
