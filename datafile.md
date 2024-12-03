---
invoice:
  number: 2025-01-01
  title: Invoice
  with-number: true
  currency: USD
author: John Doe
place: Anyplace
from:
  format:
    us: true
  company: Company A
  department: Department X
  street: 123 Main Street
  suffix: Floor 4
  city: Anytown
  postal: CA 12345
  state: Anystate
  country: USA
  phone: +1 561-555-7689
  url: www.example-company.com
  email: example@company.com
to:
  format:
    us: true
  name: Jane Roe
  company: Company B
  department: Department Y
  street: 456 Elm Street
  suffix: Floor 1
  city: Anytown
  postal: CA 12345
  state: Anystate
  country: USA
VAT: 20
service:
  - description: Yoga Course
    amount: 2
    unit: h
    rate: 75.00
    price: 150.00
    details:
  - description: Availability
    price: 200.00
    amount: 10
    unit: d
    rate: 20.00
    details:
      - Includes setting up studio
      - Offers 24/7 phone line

openingnote: |
  Some information before the main section.

closingnote: |
  Please transfer the due amount to the following account within the next 30 days:

  Company A
  Bank: Anytown National Bank
  Account Number: 1234567890
  Routing Number: 123456789

  Thank you for your business. We look forward to working with you again.

# commasep: true
lang: english
...
