---
marp: true
theme: default
paginate: true
style: |
  section {
    font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
  }
  h1 {
    color: #002C6C;
  }
  h2 {
    color: #F26334;
  }
  section.split {
    display: flex;
    flex-direction: row;
    flex-wrap: wrap;
  }
  section.split h1 {
    width: 100%;
  }
  section.split .column-left {
    flex: 1;
  }
  section.split .column-right {
    flex: 0 0 35%;
    display: flex;
    align-items: center;
    justify-content: center;
  }
---

<!-- _class: split -->
# Introduction to the GTIN

<div class="column-left">

**Global Trade Item Number**
The globally unique identification key for trade items

*GS1 Germany – Training Module 1*

</div>
<div class="column-right">

![h:400](/images/logistics-person.svg)

</div>

---

## What is a GTIN?

- **G**lobal **T**rade **I**tem **N**umber
- Uniquely identifies every trade item **worldwide**
- Assigned by GS1 Member Organisations
- Used in: retail, logistics, healthcare, e-commerce

> 💡 A GTIN is **not a price** – it is an **identity**.

---

## Structure of a GTIN-13

| Component            | Digits  | Example      |
|----------------------|---------|--------------|
| GS1 Company Prefix   | 6–12    | `4012345`    |
| Item Reference        | 0–6     | `77777`      |
| Check Digit           | 1       | `5`          |

**Result:** `402345777775`

---

## Where do we encounter the GTIN?

- 🛒 **Supermarket checkout** – EAN-13 barcode on every product
- 📦 **Logistics** – GTIN-14 on shipping cartons
- 🌐 **E-commerce** – Product identification on Amazon, Google Shopping
- 🏥 **Healthcare** – Unique identification of medical devices

---

## GTIN vs. Barcode

Note that a GTIN is the **Identifier**, not the **Data Carrier**. 

Here you can see the GTIN encoded in an EAN-13 barcode:

![h:150](/images/honeyPotOneEAN.png)

---

## GTIN in QR Codes Powered by GS1

From 2028, the GTIN can be embedded in a web address – giving your customers direct access to product-related information.

Using the same GTIN as before: it now appears in what is called a
*GS1 Digital Link URI* and is encoded into a QR Code:

![h:100](/images/honeyPotOneQR.png)

Encoded content:


```
https://id.gs1.de/01/04012345999969

```

---

## Summary

✅ GTIN = globally unique trade item key
✅ Assigned via a GS1 Company Prefix
✅ Used across **all** industries and channels
✅ Foundation for barcodes, QR Codes and GS1 Digital Link

---

## Next Module

**Module 2:** GS1 Digital Link – from barcode to URL

*Questions? → streaming@example.example*



