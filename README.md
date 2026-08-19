# مركز أهل الحديث والأثر — Markaz Ahl Al-Hadith Wal-Athar

<div dir="rtl">

التطبيق الرسمي لمركز أهل الحديث والأثر: فصول صوتية مباشرة، قنوات منفصلة
للرجال والنساء، عضوية مُراجَعة، محادثات، ومكتبة تسجيلات الدروس. عربي
أولاً، من اليمين إلى اليسار.

**هذا المستودع للإصدارات فقط** — حمّل التطبيق من
[صفحة الإصدارات](../../releases)، واقرأ ملف `VERIFY.md` المرفق مع كل
إصدار لتتحقق من سلامة ما حمّلته. الكود المصدري في مستودع خاص، وكل ملف
منشور هنا مبني آلياً منه داخل GitHub Actions ومرفق بإثبات مصدر مشفّر.

</div>

---

The official app of Markaz Ahl Al-Hadith Wal-Athar: live audio
classrooms, gender-segregated channels, vetted membership, chat, and an
archived lecture library. Arabic-first, RTL throughout.

**This repository hosts releases only.** Download from the
[releases page](../../releases) and read the `VERIFY.md` attached to each
release for verification instructions. The source code lives in a private
repository; every artifact published here is built from it by the GitHub
Actions workflow in this repo and ships with a cryptographic provenance
attestation.

## Integrity at a glance

- **Checksums** — every release includes `checksums.txt` (SHA-256 for
  each file).
- **Signing certificate** — all APKs are signed by one certificate whose
  SHA-256 fingerprint is permanent across every release:

  ```
  4369304c6323fe994dd1069f99898a527d0ac05815d99ed62570d2fb8ab4eca9
  ```

  Android refuses to update an installed original with anything signed
  differently.
- **Build provenance** — verify any downloaded file was built by this
  repo's workflow, not swapped afterwards:

  ```
  gh attestation verify <file> -R walidalbabi/Markaz-Ahl-Al-Hadith-Wal-Athar
  ```

## Which file do I download?

| Your phone | File |
|---|---|
| Most phones (2019+) | `app-arm64-v8a-release.apk` |
| Older 32-bit phones | `app-armeabi-v7a-release.apk` |
| Emulator (x86_64) | `app-x86_64-release.apk` |

The `.aab` file is for Google Play submission only — it cannot be
installed directly.
