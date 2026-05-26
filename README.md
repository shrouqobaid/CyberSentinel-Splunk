# CyberSentinel: Splunk Security Analytics

![Tool](https://img.shields.io/badge/Tool-Splunk-blue) ![Status](https://img.shields.io/badge/Status-Completed-brightgreen) ![Category](https://img.shields.io/badge/Category-Threat_Detection-red)

## 🔍 نبذة عن المشروع
هذا المشروع ليس مجرد توثيق لخطوات تقنية، بل هو محاكاة لعملية رصد وتحليل تهديدات أمنية رقمية. قمتُ باستخدام **Splunk** لتحليل سجلات ويندوز ضمن مجموعة بيانات **BOTSv3**، بهدف اكتشاف هجمات القوة الغاشمة (Brute-Force Attacks)، وتطوير نظام إنذار مبكر يحمي الأصول الرقمية.

---

## ⚙️ تفاصيل بيئة العمل
* **الأداة الأساسية:** Splunk Enterprise.
* **مجموعة البيانات:** BOTSv3 Dataset.
* **الهدف الأمني:** رصد الأحداث الأمنية ذات الرمز `4625` (فشل تسجيل الدخول) وتتبع مصادر الهجوم.

---

## 🛠 التسلسل الزمني والتحليل الفني (Investigation Steps)

### 1️⃣ إعداد البيئة وتدفق البيانات (Environment Setup)
بدأتُ العمل بتهيئة الفهارس (Indexes) واستيعاب البيانات (Data Ingestion) لضمان دقة النتائج، وفهم حجم حركة المرور داخل الشبكة.
* **Environment Setup & Index Configuration:** ![Setup](screenshots/Environment_Setup_&_Index_Configuration.png)
* **Data Source Analysis & Overview:** ![Analysis](screenshots/Data_Source_Analysis.png)
* **Initial Data Ingestion & Event Count:** ![Ingestion](screenshots/Initial_Data_Ingestion_&_Event_Count.png)

### 2️⃣ التحقيق في هجمات القوة الغاشمة (Brute-Force Investigation)
باستخدام لغة استعلامات Splunk (SPL)، قمتُ باستخراج الأنماط المشبوهة وتحديد المتغيرات الأساسية.
* **Raw Log Data Inspection:** ![Raw Logs](screenshots/Raw_Log_Data_Inspection.png)
*شرح: فحص السجلات الخام لتحديد اسم المستخدم وعنوان الـ IP المصدر للهجوم.*
* **Precision SPL for Brute-Force Detection:** ![SPL Query](screenshots/Precision_SPL_for_Brute-Force_Detection.png)
*شرح: قمت بصياغة استعلام SPL دقيق لحصر محاولات الدخول الفاشلة وتصنيفها حسب التكرار.*

### 3️⃣ النتائج الجنائية وتحليل المهاجمين (Forensic Results)
بعد التحليل، تم تحديد مصادر الهجوم الأكثر خطورة والحسابات التي كانت عرضة للاختراق.
* **Top Attacking Source IPs Analysis:** ![Attacking IPs](screenshots/Top_Attacking_Source_IPs_Analysis.png)
*شرح: استخرجتُ عناوين الـ IP الأكثر نشاطاً، مما مكنني من ربط المصادر المشبوهة ببداية سلسلة الهجوم.*
* **Targeted Account Analysis:** ![Targeted Accounts](screenshots/Targeted_Account_Analysis.png)
*شرح: حصر الحسابات الأكثر استهدافاً لتقييم مدى الضرر وتقديم توصيات أمنية بحمايتها.*

---

## الرصد والإنذار (Dashboard & Alerting)

###  بناء الداشبورد الأمنية (SOC Dashboard)
صممتُ واجهة رصد مركزية توفر رؤية شاملة لحظية للتهديدات، مما يسهل على المحللين مراقبة الشبكة.
* **SOC Threat Monitoring Dashboard:** ![SOC Dashboard](screenshots/SOC_Threat_Monitoring_Dashboard.png)

### 🔔 أتمتة التنبيهات (Automated Alerting)
* **Alert Creation Workflow:** ![Alerts](screenshots/Alert_Creation_Workflow.png)
*شرح: لقد قمت ببرمجة التنبيه ليعمل بشكل دوري كل ساعة لرصد أي نشاط غير طبيعي وتنبيه الفريق الأمني فوراً كما يظهر في اللقطة أعلاه.*
* **Active Alert Management:** ![Active Alerts](screenshots/Active_Alert_Management_&_Status.png)
*شرح: قمتُ بإدارة حالة التنبيهات النشطة للتأكد من فاعلية قواعد الرصد وسرعة الاستجابة.*

---

## الخاتمة
نجح هذا المشروع في تحويل السجلات الخام إلى معلومات استخباراتية قابلة للتنفيذ. لقد كان تحدياً تقنياً ممتعاً في ربط الاستعلامات بنتائج أمنية ملموسة.

---
