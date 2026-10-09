# Defect Report

- **Defect ID:** DEF-001
- **Title:** Decrement button increases the count
- **Related tests:** TC-03 and TC-05
- **Environment:** macOS, React, TypeScript, Vite, browser
- **Precondition:** Counter application is running.
- **Steps to reproduce:**
  1. Open the application.
  2. Increase the count to 2.
  3. Click Decrement once.
- **Expected result:** Count changes from 2 to 1.
- **Actual result:** Count: 3 was observed during testing.
- **Severity:** Medium — a core operation behaves incorrectly.
- **Priority:** High — fix before release.
- **Status:** Open.
- **Evidence:** Screenshot showing the count after clicking Decrement.
- **Suspected root cause:** The Decrement handler uses `setCount(count + 1)` instead of `setCount(count - 1)`.
- **Confirmation test:** After fixing the handler, repeat TC-03 and TC-05.
