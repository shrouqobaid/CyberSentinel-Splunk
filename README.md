# CyberSentinel: Splunk Security Analytics

![Tool](https://img.shields.io/badge/Tool-Splunk-blue) ![Status](https://img.shields.io/badge/Status-Completed-brightgreen) ![Category](https://img.shields.io/badge/Threat_Investigation-red)

## <div dir="rtl" align="right">سيناريو التحقيق الأمني (The Investigation Story)</div>
<div dir="rtl" align="right">في هذا المشروع، أتقمص دور <b>محلل أمن سيبراني (SOC Analyst)</b> يواجه سلسلة من محاولات اختراق مشبوهة. بدأت القصة بظهور ارتفاع غير مبرر في سجلات فشل تسجيل الدخول، مما دفعني لفتح تحقيق جنائي رقمي باستخدام Splunk للكشف عن هوية المهاجم وتأمين الأصول الرقمية للشركة.</div>

---

## <div dir="rtl" align="right">المرحلة الأولى: الاستطلاع وتحليل البيئة (Phase 1: Recon & Ingestion)</div>
<div dir="rtl" align="right">بدأتُ الرحلة بتهيئة البيئة وفهم حجم التهديد الذي أواجهه.</div>

* **Environment Setup & Source Analysis:** ![Setup](screenshots/environment-setup.png) ![Source](screenshots/data-source.png)
<div dir="rtl" align="right"><i>شرح: تهيئة الفهارس للتأكد من أننا نرى الصورة الكاملة للهجوم.</i></div>

* **Ingestion Overview:** ![Volume](screenshots/data-volume.png) ![Count](screenshots/ingestion-count.png)
<div dir="rtl" align="right"><i>شرح: التأكد من تدفق البيانات لضمان عدم وجود "بقع عمياء" في رصدنا.</i></div>

---

## <div dir="rtl" align="right">المرحلة الثانية: مطاردة المهاجم (Phase 2: The Hunt)</div>
<div dir="rtl" align="right">استخدمتُ لغة SPL لتحويل السجلات الصامتة إلى أدلة ملموسة.</div>

* **Log Inspection & Auth Failures:** ![Logs](screenshots/raw-logs.png) ![General](screenshots/auth-failure-query.png)
<div dir="rtl" align="right"><i>شرح: تحليل سجلات 4625. اكتشفتُ نمطاً متكرراً يشير بوضوح إلى هجوم Brute-Force.</i></div>

* **Precision SPL Detection:** ![SPL](screenshots/brute-force-spl.png)
<div dir="rtl" align="right"><i>شرح: صياغة استعلام ذكي لاكتشاف المحاولات الأكثر كثافة ومحاصرة المهاجم.</i></div>

---

## <div dir="rtl" align="right">المرحلة الثالثة: التحليل الجنائي (Phase 3: Forensic Findings)</div>
<div dir="rtl" align="right">هنا بدأت أربط النقاط ببعضها وأفهم "من" و"ماذا" استهدفوا.</div>

* **IP Activity & Attacker Identity:** ![IPs](screenshots/top-ips.png) ![Map](screenshots/ip-activity.png) ![Attacker](screenshots/attacker-id.png)
<div dir="rtl" align="right"><i>شرح: تحديد عناوين الـ IP المهاجمة ورسم خرائط زمنية لنشاطهم.</i></div>

* **Targeted Account Analysis:** ![Targeted](screenshots/targeted-accounts.png) ![Viz](screenshots/compromised-accounts.png)
<div dir="rtl" align="right"><i>شرح: اكتشاف الحسابات الحساسة التي حاول المهاجم الوصول إليها وتقديم تقرير بها.</i></div>

---

## <div dir="rtl" align="right">المرحلة الرابعة: الاستجابة والتحصين (Phase 4: Response & Defense)</div>
<div dir="rtl" align="right">لا يكفي الكشف، يجب أن نغلق الأبواب ونراقب في المستقبل.</div>

* **SOC Dashboard & Alerting:** ![Dashboard](screenshots/soc-dashboard.png) ![Details](screenshots/alert-details.png)
<div dir="rtl" align="right"><i>شرح: بناء واجهة تحكم لحظية تضعني في قلب الحدث.</i></div>

* **Automated Alerting Workflow:** ![Workflow](screenshots/alert-workflow.png) ![Active](screenshots/active-alerts.png)
<div dir="rtl" align="right"><i>شرح: "السيناريو الدفاعي": برمجة تنبيهات تعمل كل ساعة لرصد أي محاولة تكرار للهجوم فور وقوعها.</i></div>

---

## 🏁 <div dir="rtl" align="right">الخاتمة (Closing the Case)</div>
<div dir="rtl" align="right">تم إغلاق التحقيق بعد تحديد المصادر المهاجمة وتفعيل إجراءات الصد. لقد حولنا السجلات الخام إلى "معلومات استخباراتية" (Threat Intel) تحمي المنظمة.</div>

---
