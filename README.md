# Excel-Spilled-Feature

# 💧 No Sense Crying Over Spilt Formulas: Excel Loan Schedule Demo

This Excel demo showcases how to use **dynamic array formulas and the spill feature** in Microsoft Excel to build a flexible loan amortization schedule using:

- `SEQUENCE()` to generate payment periods
- `PPMT()` to calculate the **principal** portion of each payment
- `IPMT()` to calculate the **interest** portion of each payment

---

## 📊 Inputs (Editable Fields)

| Cell | Description            |
|------|------------------------|
| A2   | Number of Payments     |
| C2   | Loan Amount            |
| E2   | Interest Rate (Annual) |

Change these values and Excel will automatically update all calculations using spill logic.

---

## 🧮 Key Formulas

```excel
=SEQUENCE(A2)
=PPMT(E2/12, A5#, A2, C2)
=IPMT(E2/12, A5#, A2, C2)
