# FingerLock 下載 / Download

**[⬇️ 下載最新版 FingerLock.exe / Download latest](https://github.com/jayren1121-afk/fingerlock-download/releases/latest)**

[繁體中文](#繁體中文) ｜ [English](#english)

---

## 繁體中文

### FingerLock 是什麼？
FingerLock 是免費的 Windows 檔案鎖，用 AES-256-GCM 把你選的資料夾加密鎖起來。解鎖時：
- **提示問題（必選）**：自己設定 10 題，每次隨機抽 5 題、隨機順序，全部答對才解鎖。
- **手機指紋（可選）**：用手機指紋 / 刷臉（passkey）做第二道確認，指紋不會離開手機。
- 忘記答案或遺失手機：可寄一次性、15 分鐘有效的重設連結到你的 Email。
- 閒置自動上鎖、一鍵「立即上鎖」。

### ⚠️ 重要警告與免責聲明
1. 沒有任何安全工具是 100% 安全的（防不勝防），本軟體只能降低風險。
2. 請保護好你的提示問題答案與密碼：不要和別人分享、不要和其他網站重複使用。
3. 不要用容易被猜到或查到的個人資料（生日、電話、寵物名、學校等）當答案。
4. Email 一定要開啟兩步驟驗證（2FA）——誰控制你的 Email，誰就能重設。
5. 保持 Windows 更新、開啟防毒軟體（Windows Defender 即可）。
6. 小心釣魚信：重設連結只會在你自己按「忘記答案」後才寄出，且網址必須是你自己的 FingerLock 網址；沒按卻收到信，請不要點。
7. 定期備份 data 資料夾，遺失就無法解鎖檔案。
8. 本軟體「依現狀」免費提供，不提供任何保證；使用造成的任何資料遺失或損害，作者不負任何責任。

### 下載與驗證
1. 到 [Releases](https://github.com/jayren1121-afk/fingerlock-download/releases/latest) 下載 `FingerLock.exe` 和 `SHA256SUMS.txt`。**只從這裡下載。**
2. 在下載資料夾按 Shift + 右鍵 →「在終端機中開啟」，執行：
   ```
   certutil -hashfile FingerLock.exe SHA256
   ```
3. 結果必須和 `SHA256SUMS.txt`（及 Release 說明）中的值**完全相同**，不同就刪掉不要執行。
4. 本程式目前沒有程式碼簽章，Windows SmartScreen 可能會警告；確認雜湊正確後再按「其他資訊 → 仍要執行」。

### 使用說明書
每個 Release 都附有 PDF 說明書：`FingerLock_使用說明書.pdf`（中文）與 `FingerLock_Manual_EN.pdf`（英文）。

---

## English

### What is FingerLock?
A free Windows file locker that encrypts chosen folders with AES-256-GCM. To unlock:
- **Security questions (required)**: you set 10; each unlock asks a random 5 in random order, all must be correct.
- **Phone fingerprint (optional)**: a passkey on your phone as a second check; your fingerprint never leaves the phone.
- Forgot answers / lost phone: a single-use reset link (valid 15 minutes) is emailed to you.
- Auto-lock when idle and a one-click "Lock now".

### ⚠️ Important warning and disclaimer
1. No security tool is 100% safe; this software only reduces risk.
2. Protect your answers and passwords: never share or reuse them.
3. Don't use guessable or searchable personal info as answers.
4. Turn on 2-step verification for your email — whoever controls it can reset FingerLock.
5. Keep Windows updated and antivirus on.
6. Beware of phishing: reset emails are only sent after YOU press "Forgot answers", and the link must point to your own FingerLock address.
7. Back up the `data` folder regularly; without it locked files can't be unlocked.
8. Provided free "as is" with no warranty; the author accepts no liability for any data loss or damage.

### Download and verify
1. Download `FingerLock.exe` and `SHA256SUMS.txt` from [Releases](https://github.com/jayren1121-afk/fingerlock-download/releases/latest). **Only download from here.**
2. In the download folder: Shift + right-click → "Open in Terminal", then run:
   ```
   certutil -hashfile FingerLock.exe SHA256
   ```
3. The result must **exactly** match `SHA256SUMS.txt` (and the release notes). If not, delete the file.
4. The exe is not code-signed yet, so SmartScreen may warn; only after the hash matches choose "More info → Run anyway".

### Manuals
Each release includes PDF manuals: `FingerLock_使用說明書.pdf` (Traditional Chinese) and `FingerLock_Manual_EN.pdf` (English).
