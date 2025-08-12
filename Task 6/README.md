# Password Strength Evaluation – Task 6

##  Objective
The objective of this task was to **understand what makes a password strong** and test it against an online password strength tool. The goal was to learn **best practices** for password creation, identify weaknesses, and explore how complexity impacts password security.

---

##  Tools Used
- **Password Strength Checker** – [PasswordMeter.com](https://passwordmeter.com/)  
  This tool evaluates password strength based on:
  - Length
  - Uppercase & lowercase letters
  - Numbers
  - Symbols
  - Placement of numbers/symbols
  - Repetition & sequential patterns

---

##  Results
I tested multiple passwords of varying complexity and recorded their scores from the password meter tool.

| Password        | Score  | Complexity     | Observations |
|----------------|--------|---------------|--------------|
| `prashant123`  | 44%    | Good           | Lacks symbols, no uppercase letters, has sequential lowercase letters. |
| `prashant@123` | 66%    | Strong         | Added a symbol, meets more requirements, but still lacks uppercase letters. |
| `Prashant@123` | 94%    | Very Strong    | Added uppercase letter, meets all requirements, reduced deductions. |
| `Prashant@1234`| 100%   | Very Strong    | Increased length, meets all requirements, minimal deductions. |
| `qwerty`       | 8%     | Very Weak      | Short length, only lowercase letters, no complexity. |

*(Screenshots are included in this repository for reference.)*

---

##  Analysis
### 1. Factors Improving Password Strength
- **Length** – Longer passwords score higher.
- **Character Variety** – Using uppercase, lowercase, numbers, and symbols.
- **Randomness** – Avoiding predictable patterns or dictionary words.
- **Mixing Positions** – Placing numbers/symbols in the middle increases strength.

### 2. Factors Reducing Password Strength
- **Only Letters or Numbers** – Easy to guess.
- **Sequential Characters** – Like `123`, `abc`, `qwerty`.
- **Repetition** – Same characters reduce complexity.
- **Common Words** – Easily found in dictionary attack lists.

---

##  Best Practices for Strong Passwords
1. **Use at least 12–14 characters**.
2. **Mix uppercase, lowercase, numbers, and symbols**.
3. Avoid dictionary words or personal information.
4. Avoid sequences (`abc123`) and repeated characters.
5. Place numbers and symbols in the **middle**, not just at the end.
6. Use a **passphrase** (e.g., `Purple!Tiger$Runs2025`).
7. Consider a **password manager** for storing complex passwords.

---

##  Common Password Attacks
- **Brute Force Attack** – Tries all possible combinations.
- **Dictionary Attack** – Uses a list of common words/passwords.
- **Credential Stuffing** – Uses stolen credentials from breaches.
- **Phishing** – Tricks users into revealing passwords.

---

##  Key Learnings
- Small changes (like adding symbols or uppercase letters) can drastically improve password scores.
- Password length has a significant effect on security.
- Complex and unpredictable passwords are much harder to crack.
- Tools like PasswordMeter help visualize strengths and weaknesses, reinforcing best practices.

---

##  Outcome
After testing multiple passwords, I learned how small improvements can turn a weak password into a strong one. My final password, `Prashant@1234`, achieved **100% score** with **Very Strong** complexity.
