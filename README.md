
## دليل فهم وتشغيل المشروع

**أعضاء لجنة التقييم المحترمين،**

يهدف هذا الملف إلى تقديم دليل شامل ومبسط لفهم بنية المشروع، مكوناته الرئيسية، وكيفية نشره وتشغيله. تم تصميم المشروع كحل موزع يعالج تحديات البحث عن الملفات النصية وتقديم اقتراحات الإكمال التلقائي بفعالية.

يتألف النظام الكلي المقترح من نظامين فرعيين رئيسيين (Two Subsystems) يعملان بتناغم لتحقيق الوظائف المطلوبة، مع الحفاظ على استقلالية ومرونة كل منهما.

---

### **1. نظام البحث (Search Subsystem)**

هذا النظام مسؤول عن فهرسة الملفات النصية وتنفيذ عمليات البحث الرئيسية وتقديم النتائج للمستخدمين.

**الروابط:**

* **نظام محرك البحث الأساسي:**
    * يحتوي على المنطق الأساسي لعمليات الفهرسة والبحث ضمن الملفات الموزعة.
    * **رابط المستودع (Repository URL):** [https://github.com/kheder-hassoun/Tf-IDF-Distributed-System.git](https://github.com/kheder-hassoun/Tf-IDF-Distributed-System.git)

* **خدمة نقطة الدخول لنظام البحث (Search Service Entry Point):**
    * تمثل الواجهة الأمامية لنظام البحث، وتستقبل استعلامات البحث من المستخدمين وتوجهها إلى محرك البحث الأساسي.
    * **رابط المستودع (Repository URL):** [https://github.com/kheder-hassoun/search-service-entry-point.git](https://github.com/kheder-hassoun/search-service-entry-point.git)

---

### **2. نظام الإكمال التلقائي (Autocomplete Subsystem)**

هذا النظام مخصص لمعالجة البيانات وإنشاء اقتراحات الإكمال التلقائي، وتقديمها بسرعة للمستخدمين أثناء الكتابة.

**الروابط:**

* **خدمة المعالجة الدفعية (Batch Processing Pipeline):**
    * مسؤولة عن معالجة البيانات النصية بشكل دوري أو دفعي لإنشاء وتحديث قاموس كلمات الإكمال التلقائي.
    * **رابط المستودع (Repository URL):** [https://github.com/kheder-hassoun/batch-processing-pipeline.git](https://github.com/kheder-hassoun/batch-processing-pipeline.git)

* **خدمة السياسات (Policy Service):**
    * تُعنى بإدارة وتطبيق القواعد والسياسات المتعلقة بإنشاء وتصفية اقتراحات الإكمال التلقائي.
    * **رابط المستودع (Repository URL):** [https://github.com/kheder-hassoun/policy-service.git](https://github.com/kheder-hassoun/policy-service.git)

* **خدمة الإكمال التلقائي (Autocomplete Service Entry Point):**
    * تمثل نقطة الدخول لاقتراحات الإكمال التلقائي، حيث تتلقى مدخلات المستخدم وتوفر المقترحات المناسبة في زمن استجابة سريع.
    * **رابط المستودع (Repository URL):** [https://github.com/kheder-hassoun/autocomplete-service-entry-point.git](https://github.com/kheder-hassoun/autocomplete-service-entry-point.git) 

---

### **3. النشر والتشغيل (Deployment and Operations)**

تم تصميم النظام ليتم نشره وتشغيله ضمن بيئة Kubernetes، وذلك لضمان قابلية التوسع، التوفر العالي، وسهولة الإدارة. يتضمن كل مستودع الأكواد والملفات اللازمة لبناء صور الحاويات (Container Images) الخاصة بالخدمة، بالإضافة إلى ملفات تعريف Kubernetes (Kubernetes Manifests) اللازمة للنشر.
**مع خالص التقدير،**
[اعداد : خضر حسون]

اشراف 
ما. محمد بشار دسوقي
م. علي سعيد

