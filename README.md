# HRAI Test Automation

Bu repo, HRAI için geliştirilmiş test otomasyonlarını içerir:
- ✅ Playwright UI testleri
- ✅ Newman API testleri
- 🚀 JMeter performans testleri (manuel tetikleme)

## CI/CD Durumu

![CI](https://github.com/gullcan/hrai-tests/actions/workflows/ci.yml/badge.svg)

## Çalıştırma

```bash
# Playwright testleri
npx playwright test

# API testleri
newman run postman/hrai-collection.json -e postman/hrai-environment.postman_environment.json

# JMeter testleri
./jmeter/bin/jmeter -n -t hrai-test-plan.jmx -l results.jtl -e -o reports/hrai-report
