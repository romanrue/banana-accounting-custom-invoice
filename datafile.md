---
letter:
  author: Person Alpha
  place: Zurich
  closing: Sincerely,
  from:
    format: eu
    name: Person Alpha
    department: Department Cinema
    company: Example Company Ltd.
    street: Bahnhofstrasse
    building-number: 12
    postal-code: 8000
    town: Zurich
    country: CH
    phone: +41 44 726 30 00
    url: www.example-company.com
    email: p.alpha@example-company.com
  to:
    name: Person Beta
    department: Department Rollercoaster
    company: Ultimate Deptor AG
    street: Musterstrasse
    building-number: 5
    postal-code: 4001
    town: Basel
    country: CH

invoice:
  title: Invoice
  number: 2025-01-01
  with-number: true
  currency: CHF
  vat: 8.1
  autoround: true
  service:
    - description: Work Package
      price: 150.00
      quantity: 2.00
      unit: h
      rate: 75.00
      details:
    - description: Service
      price: 200.00
      quantity: 10.00
      unit: d
      rate: 20.00
      details:
        - Includes setup
        - Offers 24/7 phone line
  sum:
    net: 350
    vat: 28.35
    gross: 378.35


  openingnote: |
    Some information before the main section.

  closingnote: |
    Please transfer the due amount to the following account within the next 30 days:

    Thank you for your business. We look forward to working with you again.

# commasep: true
lang: english
# Legend - M: Mandatory, D: Dependent, B: Additional, O: Optional, X: Do not fill
qrch:
  header:
    qrtype: SPC # M
    version: 0200 # M
    coding: 1 # M
  creditor-information:
    iban: CH9300762011623852957 # M
  creditor:
    #TODO: Implement creditor Address-Type
    # address-type: S # M
    name: Example Company Ltd. # M
    street: Bahnhofstrasse # O
    building-number: 12 # O
    postal-code: 8000 # D
    town: Zürich # D
    country: CH # M
  ultimate-creditor:
    #TODO: Implement ultimate-creditor Address-Type
    # address-type: S # X
    name: Ultimate Creditor AG # X
    street: Seestrasse # X
    building-number: 45 # X
    postal-code: 6300 # X
    town: Zug # X
    country: CH # X
  payment-amount:
    amount: 1234.56 # M
    currency: CHF
  ultimate-deptor:
    #TODO: Implement ultimate-deptor Address-Type
    # address-type: S # D
    name: Person Beta
    street: Musterstrasse # O
    building-number: 5 # O
    postal-code: 4001 # D
    town: Basel # D
    country: CH # D
  payment-reference:
    type: QRR # M
    reference: 210000000003139471430009017 # D
  additional-information:
    message: | # O
      Order #3456 (01.01.2025)
    trailer: EDP # M
    billing-information: Invoice 12345 # A
  alternative-procedures:
    av1-parameters: ebill/B/info@ultimate-creditor.com # A
    av2-parameters: Payment can also be made via TWINT # A
---
