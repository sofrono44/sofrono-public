# FINRA Marketing Content Compliance Review Skill

A Claude skill for reviewing broker-dealer marketing materials against FINRA Rule 2210 and related regulations. This tool assists compliance teams with preliminary content review by identifying potential issues, providing rule citations, and suggesting compliant alternatives.

## ⚠️ Important Disclaimer

**This skill is a productivity tool for preliminary compliance review. It does not constitute legal, regulatory, or compliance advice.**

- Final compliance determinations must be made by qualified compliance personnel
- This tool does not replace registered principal review, FINRA filing requirements, or legal counsel
- FINRA rules and interpretations change; always verify current requirements
- Users are solely responsible for ensuring their content meets all applicable regulatory requirements

## Overview

This skill analyzes marketing content against FINRA communications rules and provides:

- **Issue Identification** – Flags potential compliance problems with specific text citations
- **Rule References** – Cites applicable FINRA rules for each issue
- **Suggested Revisions** – Provides compliant alternative language
- **Risk Assessment** – Categorizes issues by severity
- **Approval Guidance** – Outlines filing and recordkeeping requirements

## Invocation

```
/finra-review
```

Or ask Claude to:
- "Review this marketing content for FINRA compliance"
- "Check this advertisement for regulatory issues"
- "Analyze this social media post for FINRA rules"

## Supported Content Types

| Content Type | Notes |
|--------------|-------|
| Website content | Landing pages, hero copy, about sections |
| Social media posts | Triggers additional platform-specific guidance |
| White papers | Long-form educational content |
| Case studies | Client success stories, outcomes |
| Press releases | Company announcements |
| Email marketing | Campaigns, newsletters |
| Brochures/Sales literature | PDF collateral, leave-behinds |
| Advertisements | Paid media, display ads |
| Video scripts | YouTube, webinar content |

## Workflow

### Step 1: Gather Context

Before reviewing, the skill collects:

**Communication Category** (per FINRA Rule 2210(a)):
- **Retail Communication** – Distributed to more than 25 retail investors within 30 days
- **Institutional Communication** – Exclusively for institutional investors
- **Correspondence** – Written communication with 25 or fewer retail investors

**Product Type:**
- General securities (stocks, bonds, ETFs)
- Mutual funds
- Variable annuities / Variable life insurance
- Options
- 529 education savings plans
- Alternative investments
- Fixed income / Structured products
- General firm marketing (no specific product)

**Target Audience:**
- Retail investors (general public)
- Institutional investors
- Existing clients
- Prospective clients

### Step 2: Compliance Analysis

The skill analyzes content against these primary areas:

#### FINRA Rule 2210 – Communications with the Public

| Section | Requirement |
|---------|-------------|
| 2210(d)(1)(A) | Fair and balanced presentation; no omission of material facts |
| 2210(d)(1)(B) | No false, exaggerated, unwarranted, promissory, or misleading statements |
| 2210(d)(1)(F) | Performance presentation standards |
| 2210(d)(2) | Required disclosures for performance data |
| 2210(d)(3) | Clear and prominent disclosure requirements |

#### Related Rules

| Rule | Description |
|------|-------------|
| 2210(b) | Approval and review requirements |
| 2210(c) | FINRA filing requirements |
| 2211 | Communications regarding variable insurance products |
| 2220 | Options communications |
| 2111 | Suitability |
| 4511 | Recordkeeping requirements |

#### SEC Marketing Rule

| Section | Description |
|---------|-------------|
| 206(4)-1 | Testimonials and endorsements |

### Step 3: Social Media Mode

When reviewing social media content, additional guidance applies per FINRA Regulatory Notices 17-18 and 19-31:

**Platform-Specific Considerations:**
- **Character-limited platforms (X/Twitter):** Link to full disclosures acceptable with clear reference
- **LinkedIn:** Professional context but retail communication rules apply
- **Facebook/Instagram:** Visual content meets same standards as text
- **YouTube/Video:** Disclosures must appear in video, not just description

**Additional Checks:**
- Space-constrained disclosure linking
- Third-party content sharing responsibilities
- Influencer/paid promotion disclosures
- Hashtag implications
- Recordkeeping for social media

### Step 4: Output Report

The skill generates a structured compliance report:

```
## FINRA Compliance Review Report

**Content Type:** [Type]
**Communication Category:** [Category]
**Product Type:** [Product]
**Review Date:** [Date]

### Compliance Issues Identified

#### Issue [#]: [Description]
**Original Text:** "[Quoted text]"
**Rule Citation:** FINRA Rule [XXXX]
**Compliance Concern:** [Explanation]
**Suggested Revision:** "[Compliant alternative]"
**Risk Level:** [High/Medium/Low]

### Required Disclosures
[List of missing disclosures with suggested language]

### Approval Checklist
- [ ] Registered Principal Review
- [ ] FINRA Filing Required: [Yes/No, type]
- [ ] Compliance Department Review
- [ ] Legal Review
- [ ] Recordkeeping requirements

### Compliance Risk Summary
**Overall Risk Level:** [High/Medium/Low]
**Issues by Category:** [Counts]
**Summary:** [Professional summary]

### Recommendations
[Prioritized action items]
```

## Common Issues Detected

| Issue Type | Example | Rule |
|------------|---------|------|
| Promissory language | "Guaranteed returns," "Ensure profits" | 2210(d)(1)(B) |
| Unbalanced presentation | Benefits without risks | 2210(d)(1)(A) |
| Performance without disclosure | "18% annual returns" (no context) | 2210(d)(1)(F) |
| Testimonial violations | Client quotes without required disclosures | SEC 206(4)-1 |
| Absolute claims | "Always outperforms," "Zero risk" | 2210(d)(1)(B) |
| Suitability implications | "Perfect for all investors" | 2111 |

## Example Usage

**Input:**
```
Review this for FINRA compliance:

"Achieve consistent, market-beating returns with our AI-driven strategies. 
Our platform delivers superior performance in all market conditions."
```

**Output:**
```
#### Issue 1: Promissory Performance Claims

**Original Text:** "Achieve consistent, market-beating returns"

**Rule Citation:** FINRA Rule 2210(d)(1)(B)

**Compliance Concern:** This language promises guaranteed outcomes. 
No investment strategy can guarantee market-beating performance.

**Suggested Revision:** "Our AI-driven strategies seek competitive 
risk-adjusted returns. Past performance is not indicative of future 
results, and all investments involve risk."

**Risk Level:** High
```

## Limitations

This skill:
- ❌ Does not provide legal or compliance advice
- ❌ Cannot make binding compliance determinations
- ❌ Does not replace registered principal review
- ❌ Cannot verify factual accuracy of performance claims
- ❌ Does not check state-specific securities regulations
- ❌ Cannot assess suitability for specific investors

This skill:
- ✅ Identifies potential compliance issues for human review
- ✅ Provides FINRA rule citations for reference
- ✅ Suggests compliant alternative language
- ✅ Outlines approval and filing requirements
- ✅ Helps standardize preliminary compliance review

## FINRA Rules Quick Reference

| Rule | Description |
|------|-------------|
| 2210 | Communications with the Public |
| 2210(a) | Definitions (Retail, Institutional, Correspondence) |
| 2210(b) | Approval, Review and Recordkeeping |
| 2210(c) | Filing Requirements |
| 2210(d) | Content Standards |
| 2211 | Variable Insurance Communications |
| 2220 | Options Communications |
| 2111 | Suitability |
| 4511 | General Recordkeeping Requirements |

## Version History

| Version | Date | Changes |
|---------|------|---------|
| 1.0.0 | 2025-01 | Initial release |

## License

MIT License – See LICENSE file

## Contributing

Issues and pull requests welcome. Please ensure any rule updates include citations to FINRA regulatory notices or rule amendments.

## Author

Doug Beeferman / Switchfin

---

*This skill references publicly available FINRA rules and SEC regulations. Rule text and interpretations are subject to change. Always consult current FINRA and SEC guidance.*
