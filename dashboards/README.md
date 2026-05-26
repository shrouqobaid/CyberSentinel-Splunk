# SOC Dashboards & Visualizations

هذا المجلد يحتوي على واجهات المراقبة (Dashboards) التي قمتُ بتصميمها داخل Splunk لتعزيز الرؤية الأمنية (Security Visibility) وتسهيل عملية الاستجابة للحوادث.

## 📊 لوحات المراقبة:

### 1. SOC Threat Monitoring Dashboard
* **الهدف:** توفير ملخص تنفيذي لحظي للتهديدات النشطة في الشبكة.
* **البيانات المعروضة:** إجمالي الهجمات، الحسابات المستهدفة، والمصادر المشبوهة.
![SOC Dashboard](soc-dashboard.png)

### 2. Authentication Monitoring Dashboard
* **الهدف:** تتبع نشاط تسجيل الدخول (الناجح والفاشل) وتحديد أنماط الدخول غير الطبيعية.
* **البيانات المعروضة:** معدل فشل تسجيل الدخول، الحسابات الأكثر استهدافاً، وتوقيتات المحاولات.
![Auth Dashboard](auth-failure-query.png)

### 3. Brute-Force Visualization
* **الهدف:** تحليل مرئي متقدم لهجمات الـ Brute-Force.
* **البيانات المعروضة:** خريطة زمنية للارتفاعات (Spikes) في الهجمات، وربط عناوين الـ IP المهاجمة بالنشاط المسجل.
![Brute-Force Viz](brute-force-spl.png)

---

## 🔍 Visual Investigation Findings
هذه الرسوم البيانية هي جزء من التحليل الجنائي الرقمي الذي قمت بإجرائه داخل الـ Dashboard:

* **IP Activity Tracking:** تعقب حركة المهاجم ومصادر التهديد.
![IP Activity](ip-activity.png)

* **Compromised Accounts:** حصر الحسابات التي تم استهدافها أو اختراقها للحد من الأضرار.
![Compromised Accounts](compromised-accounts.png)

---
*ملاحظة: تم تصميم هذه اللوحات لدعم اتخاذ القرارات السريعة لفريق الـ SOC.*

