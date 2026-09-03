# SC-900 — Exam Tips

## The traps, by domain

**Domain 1 — Concepts**

- In IaaS the **customer** owns the guest OS. Microsoft's responsibility stops at the physical host and hypervisor.
- **Data, devices and identities are always the customer's**, in every service model. That row never changes.
- Hashing is **not** encryption. "Verified but never recovered" = hashing.
- Zero Trust is **not a product**. You can't buy it; it's a strategy implemented with many products.
- Federation is the trust *between organizations*; SSO is the user experience that results.

**Domain 2 — Entra**

- **Conditional Access = P1. Identity Protection and PIM = P2.** Expect at least one question on this.
- Security defaults and Conditional Access are **mutually exclusive**.
- Dynamic groups need P1.
- **Defender for Identity** protects on-premises AD; **Entra ID Protection** protects cloud identities.
- A managed identity is a service principal Azure manages for you — no secrets to rotate.

**Domain 3 — Security solutions**

- **Defender for Cloud ≠ Defender for Cloud Apps.** Posture vs CASB.
- Sentinel is SIEM **and** SOAR, billed by data ingested and retained.
- NSG = basic allow/deny. Azure Firewall = managed and stateful. WAF = web application layer.
- Two similarly named scores: **Secure Score** in Defender for Cloud (Azure posture) vs **Microsoft Secure Score** (Microsoft 365 posture).

**Domain 4 — Compliance**

- **Sensitivity label** protects content and travels with the file. **Retention label** controls lifespan.
- Conflicting retention: **retention beats deletion, longest period wins.**
- **Service Trust Portal** = Microsoft's audit reports. **Compliance Manager** = your posture.
- Insider Risk Management is about *internal* users.

---

## Exam-day strategy

**Before**

- Take the official practice assessment. It's free and its wording is the closest to the real thing.
- Last day: index cards only. No new material.
- Check the "Skills measured as of" date one final time.

**During**

1. **Read the last line of the question first.** It tells you what's actually being asked; the paragraph above is often scenario padding.
2. **Watch the number of answers required.** If it says "select two," a perfect single answer is still wrong.
3. **Eliminate by surface.** Most Defender questions resolve the moment you ask: what is being protected here — a device, a mailbox, on-prem AD, or a SaaS app?
4. **Licence keywords are decisive.** Risk-based policies or just-in-time roles put you in P2 territory.
5. **Mark and move on.** Nothing costs more points than four minutes on one question.
6. **Don't overthink.** Fundamentals exams reward the textbook answer, not the clever one.

**After**

- You get your result on screen immediately.
- Add the badge to LinkedIn the same day, and post about what you learned. That post reaches further than the badge alone — and if you did the labs, you have screenshots to prove you practised.
