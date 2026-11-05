# CSV Import Starter Kit

A free, read-only CSV/TSV checker that runs on your own computer, with six synthetic practice files and an import handoff checklist. No installation, account, API key or subscription is needed to run it.

## Download and run

1. [Download the kit ZIP](../../raw/refs/heads/main/csv-import-starter-kit-1.0.zip).
2. Extract it, then open `start-here.html` in a modern desktop browser.
3. Click **Load an imperfect example**, select Contacts, Inventory or Orders, and inspect the findings.
4. Try the matching clean file. All three clean examples produce zero findings under their matching profiles.

The standalone [start-here.html](start-here.html) file also works when saved locally. GitHub displays HTML source; download it rather than expecting the repository preview to run the app.

## What it checks

Basic structure checks include missing headers, uneven record widths, duplicate records and formula-like cells. Fixed profiles add exact required/unique/type rules:

| Profile | Practice fields | Needs-review findings | Clean findings |
| --- | --- | ---: | ---: |
| Contacts | id, name, email | 5 | 0 |
| Inventory | sku, name, quantity, unit_price | 4 | 0 |
| Orders | order_id, email, date, total | 4 | 0 |

Header names are exact and case-sensitive. For your own schema, use **Basic structure**, which does not infer custom business rules. Email validation checks basic syntax, not deliverability. Numbers are ungrouped decimals and dates use real YYYY-MM-DD dates. The included JSON presets work with the full RowReady application; this free checker has the fixed rules built in.

## Limits and privacy

- UTF-8 CSV/TSV; 200 data records, 50 header columns and 512 KiB per file.
- Files over the limits are rejected, not silently truncated.
- Read-only: no cleaning, modified CSV export, custom rules or batch folder processing.
- The downloaded checker makes no network requests and uses no analytics or browser storage. Store links navigate only when clicked.
- Reports may contain private filenames and column names. Keep reports private.
- These are generic practice schemas, not official CRM or accounting import templates. A clean report does not guarantee destination compatibility.

## A nine-step import handoff

1. Keep an untouched source copy and identify the system of record.
2. Confirm destination headers, required fields, unique keys and allowed values.
3. Agree on date/decimal formats, units, currency and encoding.
4. Preserve leading zeros and long identifiers as text.
5. Review duplicates, missing values, record widths and formula-like cells.
6. Resolve ambiguous values using source evidence; do not invent data.
7. Rehearse a small subset in a test workspace or destination preview.
8. Reconcile source, accepted, rejected and skipped record counts.
9. Spot-check imported values and retain an error report and rollback plan.

## 한국어 빠른 시작

ZIP을 내려받아 압축을 풀고 `start-here.html`을 브라우저에서 여세요. 설치나 유료 계정 없이 작은 CSV/TSV 파일을 검사할 수 있습니다. **Load an imperfect example**로 예제를 불러오거나 본인 파일을 선택하세요. 데이터는 파일을 연 브라우저에서 처리하며 서버로 업로드하지 않습니다.

무료판 한도는 UTF-8, 데이터 200행, 헤더 50열, 512 KiB입니다. 원본을 수정하지 않으며, 검사 결과가 깨끗해도 실제 대상 시스템에 작은 표본을 먼저 넣어 확인해야 합니다. Excel 파일은 CSV로 내보내야 합니다.

## License and provenance

This is the creator's official GitHub mirror of the free kit. The included [free internal-use license](LICENSE.txt) applies. **Publicly readable source does not mean an open-source license.** This repository does not grant rights to the paid applications. All practice records are synthetic; email addresses use the reserved `.invalid` domain.

The free checker passed 14 automated tests covering known findings, clean inputs, limits, malformed CSV, fixed profile validation and read-only behavior. Synthetic examples and a clean file were also checked in a browser. This is not a guarantee of complete error detection.

## Related tools from the same creator

Use this free kit first if its limits fit your task. No purchase is needed to use it.

- [Free kit on Gumroad](https://genosyde.gumroad.com/l/csv-import-starter-kit?utm_source=github&utm_medium=readme&utm_campaign=csv_kit_launch).
- [RowReady](https://genosyde.gumroad.com/l/rowready?utm_source=github&utm_medium=readme&utm_campaign=csv_kit_launch): larger CSV checks, custom rules, opt-in cleanup and a Node.js folder checker. USD 19 base price.
- [NameHarbor](https://genosyde.gumroad.com/l/nameharbor?utm_source=github&utm_medium=readme&utm_campaign=csv_kit_launch): preview Windows file renames and restore unchanged files when original names are available. Windows 10/11 x64 only; unsigned EXE. USD 9 base price.
- [Offline Desk Toolkit](https://genosyde.gumroad.com/l/offline-desk-toolkit?utm_source=github&utm_medium=readme&utm_campaign=csv_kit_launch): both full tools for USD 22 versus USD 28 separately.

Prices are base USD prices as of November 5, 2026. Check current checkout prices, currency, tax, requirements and license terms. Keep backups and review outputs. No future updates or custom support are promised.
