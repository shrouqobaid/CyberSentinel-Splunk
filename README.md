# CyberSentinel: Splunk Security Analytics

![Tool](https://img.shields.io/badge/Tool-Splunk-blue) ![Status](https://img.shields.io/badge/Status-Completed-brightgreen) ![Category](https://img.shields.io/badge/Category-Threat_Detection-red)

## 🔍 نبذة عن المشروع
هذا المشروع ليس مجرد توثيق لخطوات تقنية، بل هو محاكاة لعملية رصد وتحليل تهديدات أمنية رقمية. قمتُ باستخدام **Splunk** لتحليل سجلات ويندوز ضمن مجموعة بيانات **BOTSv3**، بهدف اكتشاف هجمات القوة الغاشمة (Brute-Force Attacks)، وتطوير نظام إنذار مبكر يحمي الأصول الرقمية.

---

## ⚙️ إعداد البيئة وتدفق البيانات
بدأتُ العمل بتهيئة الفهارس (Indexes) واستيعاب البيانات (Data Ingestion) لضمان دقة النتائج وفهم حجم حركة المرور.

* **Environment Setup:** ![Setup](screenshots/environment-setup.png)
*شرح: تهيئة بيئة Splunk وربط الفهارس لضمان دقة البيانات.*
* **Data Source Analysis:** ![Source](screenshots/data-source.png)
*شرح: تحليل مصادر البيانات لفهم حركة المرور داخل الشبكة.*
* **Ingestion Overview:** ![Volume](screenshots/data-volume.png)
*شرح: استعراض حجم البيانات المستوعبة للتأكد من شمولية الرصد.*
* **Initial Event Count:** ![Count](screenshots/ingestion-count.png)
*شرح: فحص عدد الأحداث المبدئي لضمان عدم وجود فقدان في سجلات النظام.*

---

## 🛠 التحقيق والتحليل الأمني
باستخدام لغة استعلامات Splunk (SPL)، قمتُ باستخراج الأنماط المشبوهة وتحديد المتغيرات الأساسية للهجوم.

* **Raw Log Data Inspection:** ![Logs](screenshots/raw-logs.png)
*شرح: فحص السجلات الخام لتحديد المتغيرات الأساسية مثل اسم المستخدم وعنوان الـ IP.*
* **General Auth Failure Query:** ![General](screenshots/auth-failure-query.png)
*شرح: تشغيل الاستعلامات المبدئية لحصر محاولات تسجيل الدخول الفاشلة (EventCode 4625).*
* **Precision SPL Detection:** ![SPL](screenshots/brute-force-spl.png)
*شرح: قمت بصياغة استعلام SPL دقيق لاكتشاف أنماط الهجوم المتكررة (Brute-Force) وتصنيفها حسب التكرار.*

---

## 📊 النتائج الجنائية وتحليل المهاجمين
بعد التحليل، تم تحديد مصادر الهجوم الأكثر خطورة والحسابات التي كانت عرضة للاختراق.

* **Top Attacking IPs:** ![IPs](screenshots/top-ips.png)
*شرح: تحديد عناوين الـ IP الأكثر نشاطاً في الهجوم للبدء في إجراءات الحظر.*
* **IP Activity Map:** ![Map](screenshots/ip-activity.png)
*شرح: رسم بياني يوضح توزيع أنشطة الـ IP المهاجمة زمنياً.*
* **Targeted Account Analysis:** ![Targeted](screenshots/targeted-accounts.png)
*شرح: حصر الحسابات الأكثر تعرضاً للاختراق لتقديم توصيات أمنية بحمايتها.*
* **Compromised Accounts Viz:** ![Viz](screenshots/compromised-accounts.png)
*شرح: تحليل مرئي للحسابات التي تم استهدافها أو محاولة الوصول إليها.*
* **Attacker Identification:** ![Attacker](screenshots/attacker-id.png)
*شرح: الكشف عن هوية المهاجم وتحديد النمط السلوكي له.*

---

## 🖥 الرصد والإنذار
صممتُ واجهة رصد مركزية توفر رؤية شاملة لحظية للتهديدات (Real-time Monitoring).

* **SOC Dashboard:** ![Dashboard](screenshots/soc-dashboard.png)
*شرح: الداشبورد المركزية التي صممتُها لرصد التهديدات لحظياً.*
* **Incident Alert Details:** ![Details](screenshots/alert-details.png)
*شرح: تحليل تفصيلي لبيانات التنبيه الأمني المسجل.*
* **Alert Workflow:** ![Workflow](screenshots/alert-workflow.png)
*شرح: لقد قمت ببرمجة التنبيه ليعمل بشكل دوري كل ساعة لرصد أي نشاط غير طبيعي وتنبيه الفريق الأمني فوراً.*
* **Active Alert Management:** ![Active](screenshots/active-alerts.png)
*شرح: إدارة الحالة التشغيلية للتنبيهات لضمان أعلى مستوى من الاستجابة.*

---

## 🏁 الخاتمة
نجح هذا المشروع في تحويل السجلات الخام إلى معلومات استخباراتية قابلة للتنفيذ. لقد كان تحدياً تقنياً ممتعاً في ربط الاستعلامات بنتائج أمنية ملموسة، مما ساهم في بناء بيئة رقمية أكثر أماناً.

---

