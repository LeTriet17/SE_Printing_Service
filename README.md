# Student Smart Printing Service (HCMUT_SSPS) - System Requirements Document

## Introduction

This document specifies the requirements for the Student Smart Printing Service (HCMUT_SSPS) intended for students at HCMUT for printing documents across campus. This service aims to facilitate quick and efficient printing solutions for students while allowing the Student Printing Service Officer (SPSO) to manage and monitor the system effectively.

---

## Functional Requirements

### General

1. **Authentication**
   - All users must be authenticated via the HCMUT_SSO authentication service.

### For Students

1. **Document Upload**

   - Students can upload files for printing.
   - Supported file types are limited and configured by the SPSO.
2. **Printer Selection**

   - Students can select from a list of available printers identified by ID, brand name, printer model, and location.
3. **Printing Properties**

   - Students can specify the paper size, pages to be printed, one- or double-sided, and number of copies.
4. **Printing Log**

   - Students can view their printing history and summary of the number of printed pages for each page size.
5. **Page Quota and Payments**

   - Each student will have a default page quota each semester.
   - Students can buy additional pages via the 'Buy Printing Pages' feature using the BKPay system.

### For SPSO

1. **Printer Management**

   - The SPSO can add, enable, and disable printers.
2. **Configuration Management**

   - The SPSO can configure various system settings including the default page quota, accepted file types, etc.
3. **Printing Log**

   - The SPSO can view printing logs of all students or individual students within a date range and for all or some printers.
4. **Reports**

   - Monthly and yearly reports are generated automatically for review by the SPSO.

---

## Non-functional Requirements

1. **Scalability**

   - The system should be scalable to support an increasing number of printers and students.
2. **Performance**

   - The system should be responsive, with low latency in both the web-based and mobile apps.
3. **Security**

   - All data must be encrypted and secure to prevent unauthorized access.
4. **Accessibility**

   - The system should be accessible via both web and mobile applications.
5. **Auditability**

   - All actions must be logged to provide a comprehensive audit trail.

---

## Data Requirements

1. **Printer Data**

   - ID, Brand/Manufacturer Name, Printer Model, Description, Location (campus, building, room)
2. **Student Data**

   - Student ID, Name, Page Quota
3. **Printing Log Data**

   - Student ID, Printer ID, File Name, Start and End Time, Number of Pages, Page Size
4. **Payment Data**

   - Payment method, Number of Pages Bought, Payment Time

---

## Future Enhancements

1. Option for color or black-and-white printing.
2. Integrate with university library services for printing resources directly.
3. Support for additional payment methods.

---

This document serves as the base for the development of the HCMUT_SSPS system and will be updated as required.
