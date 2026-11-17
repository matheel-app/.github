# Matheel · ماثل

**ZATCA Phase 2 e-invoicing for Saudi Arabia in one API call.** Matheel signs the invoice (UBL 2.1, XAdES, QR), files it
with ZATCA (clearance or reporting) and returns ZATCA's answer, the legal XML and a bilingual PDF/A-3. It stores nothing.

```bash
# Try it now: the developer sandbox needs no key
curl https://matheel.app/api/v1/invoices -H "Content-Type: application/json" \
  -d '{"environment":"sandbox","pdf":true,"invoice":{"type":"simplified",
       "line_items":[{"name":"Coffee","quantity":2,"price":"50.00"}]}}'
```

| Repository | What it is | Install |
|---|---|---|
| [zatca-rules](https://github.com/matheel-app/zatca-rules) | Every ZATCA business rule explained in Arabic and English, 187 with tested examples, plus a local validator | `git clone` |
| [matheel-node](https://github.com/matheel-app/matheel-node) | Node.js client | `npm i matheel` |
| [matheel-python](https://github.com/matheel-app/matheel-python) | Python client | `pip install matheel-zatca` |
| [matheel-php](https://github.com/matheel-app/matheel-php) | PHP client | `composer require matheel/matheel-php` |
| [matheel-flutter](https://github.com/matheel-app/matheel-flutter) | Flutter: decode the ZATCA QR and show the invoice in your app | `flutter pub add matheel_zatca` |

- Docs: [matheel.app/en/docs](https://matheel.app/en/docs) · العربية: [matheel.app/docs](https://matheel.app/docs)
- Look up a ZATCA error: [matheel.app/en/zatca-errors](https://matheel.app/en/zatca-errors) · [أخطاء زاتكا](https://matheel.app/akhta)
- Validate an invoice in your browser: [matheel.app/en/zatca-validator](https://matheel.app/en/zatca-validator)

**بالعربي:** ماثل يربط فواتيرك بالمرحلة الثانية من الفوترة الإلكترونية بطلب واحد: يوقّع الفاتورة ويرسلها للهيئة ويرجّع ردها مع PDF عربي وإنجليزي. جرّبه بدون مفتاح على [matheel.app](https://matheel.app).

hello@matheel.app
