# FINRA Marketing Compliance Review Skill

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)

A Claude skill that reviews broker-dealer marketing materials for FINRA Rule 2210 compliance. Identifies potential issues, provides rule citations, and suggests compliant alternatives.

## 🎯 What It Does

- **Scans marketing content** for common FINRA compliance issues
- **Cites specific rules** (2210, 2111, 2220, SEC Marketing Rule)
- **Suggests compliant rewrites** for problematic language
- **Generates structured reports** with approval checklists
- **Handles social media** with platform-specific guidance

## ⚡ Quick Start

1. Add the skill to your Claude environment
2. Share your marketing content
3. Invoke with `/finra-review` or ask Claude to review for FINRA compliance
4. Receive a structured compliance report

## 📋 Example

**Input:**
> "Achieve guaranteed returns with our proven investment strategy."

**Output:**
> **Issue:** Promissory language  
> **Rule:** FINRA 2210(d)(1)(B)  
> **Suggested:** "Our investment strategy seeks competitive returns. All investments involve risk, including potential loss of principal."

## 🔍 What It Checks

| Category | Examples |
|----------|----------|
| Promissory language | "Guaranteed," "Ensure," "Always" |
| Unbalanced claims | Benefits without risk disclosure |
| Performance issues | Returns without required disclosures |
| Testimonial violations | Missing compensation/typicality disclosures |
| Suitability problems | "Perfect for everyone" claims |

## 📁 Files

```
├── SKILL.md      # Full skill documentation and workflow
├── LICENSE       # MIT License with compliance disclaimer
└── README.md     # This file
```

## ⚠️ Important

**This is a review aid, not compliance advice.**

- Does not replace registered principal review
- Does not constitute legal advice
- Final determinations require qualified compliance personnel
- FINRA rules change; verify current requirements

## 📄 License

MIT License with additional compliance tool disclaimer. See [LICENSE](LICENSE).

## 🤝 Contributing

PRs welcome. Please cite FINRA regulatory notices for any rule updates.

---

*Built for broker-dealer marketing teams and compliance professionals.*
