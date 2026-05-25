# ☀️ Solar Quotation Tools - Bin Zareen Solar

## Overview
A comprehensive suite of professional solar quotation tools that allow instant creation, PDF export, and WhatsApp sharing of solar system quotations.

---

## 📁 Files Included

### 1. **quotations.html** (Main Landing Page)
- Landing page with both quotation tools
- Links to the fixed quotation and custom generator
- Professional design with company branding
- Contact information and features showcase

**How to access:**
```
http://localhost/quotations.html
```

---

### 2. **quotation.html** (Pre-built 1.3 kW System)
A professional quotation for the popular 1.3 kW daytime solar system with:

**System Details:**
- System Size: 1.3 kW (Daytime)
- Load: 1270 W
- Panels: 3 x Canadian Solar 540W BiHiKu6
- Total Cost: Rs. 206,000

**Included Items:**
- 3x Canadian Solar 540W BiHiKu6 Panels: Rs. 58,500
- 3x L2 Mounting Structure: Rs. 7,500
- Growatt SPH 5000 Hybrid Inverter: Rs. 95,000
- DC Cable (10m, 4mm): Rs. 15,000
- AC Cable (10m, 4mm): Rs. 15,000
- DB Box & Protection Set: Rs. 15,000

**Features:**
✅ One-click PDF download
✅ Direct WhatsApp sharing
✅ Professional formatting with company branding
✅ Mobile responsive design
✅ Print-friendly layout

**How to access:**
```
http://localhost/quotation.html
```

**How to use:**
1. Click "Download as PDF" button to save quotation
2. Click "Send on WhatsApp" to share directly (opens WhatsApp with pre-formatted message)

---

### 3. **quotation-generator.html** (Custom Quotation Builder)
A flexible tool to create custom quotations with:

**Features:**
- System type selection (Daytime, Hybrid, Off-Grid)
- Custom system size and load specification
- Add/remove/edit line items
- Custom pricing per item
- Customer details collection
- Live total calculation
- PDF export
- WhatsApp sharing

**How to use:**
1. Fill in system details (type, size, load)
2. Customize items list (add/remove as needed)
3. Enter your details (name, WhatsApp, city)
4. Click "Preview Quotation"
5. Download as PDF or send on WhatsApp

**How to access:**
```
http://localhost/quotation-generator.html
```

---

## 🚀 Key Features

### PDF Export
- Uses html2pdf.js library (CDN-based, no server required)
- Professional formatting
- Includes company branding
- Automatic file naming with date

### WhatsApp Integration
- One-click WhatsApp sharing
- Pre-formatted message with all details
- Automatic phone number routing (03252053313)
- Works on desktop and mobile
- No additional setup required

### Responsive Design
- Mobile-optimized
- Works on all screen sizes
- Touch-friendly buttons
- Print-ready formatting

---

## 📊 Technical Details

### Libraries Used
- **html2pdf.js**: PDF generation (CDN)
  ```html
  <script src="https://cdnjs.cloudflare.com/ajax/libs/html2pdf.js/0.10.1/html2pdf.bundle.min.js"></script>
  ```

### Browser Support
- Chrome/Edge: ✅ Full support
- Firefox: ✅ Full support
- Safari: ✅ Full support
- Mobile browsers: ✅ Full support

### No Backend Required
All tools work entirely client-side:
- No server-side processing
- No database required
- Works offline (except WhatsApp sharing)
- Fast performance

---

## 🔧 Customization Guide

### Change Company Phone Number
Find and replace `03252053313` with your number in all three files:

**quotation.html:**
```javascript
const whatsappURL = `https://wa.me/923252053313?text=...`;
```

**quotation-generator.html:**
```javascript
const whatsappURL = `https://wa.me/923252053313?text=...`;
```

### Change Company Details
Update company information in:
- Company name
- Email address
- Location
- Phone number
- Website URL

### Add/Remove System Items
In **quotation.html**, modify the items in the table:
```html
<tr>
    <td>Item Name</td>
    <td>Quantity</td>
    <td>Price</td>
    <td>Total</td>
</tr>
```

In **quotation-generator.html**, edit the `defaultItems` array:
```javascript
const defaultItems = [
    { name: 'Item Name', qty: 1, price: 0 },
];
```

### Modify Colors/Branding
CSS variables at the top of each file:
```css
--red-deep: #7F1D1D;
--red-mid: #B91C1C;
--red-bright: #DC2626;
```

---

## 📱 Integration with Main Website

To integrate with your main index.html, add navigation links:

```html
<!-- In navbar or menu -->
<a href="quotations.html">Create Quotation</a>
<a href="quotation.html">View 1.3kW Quote</a>
<a href="quotation-generator.html">Custom Quote</a>
```

---

## 📋 WhatsApp Message Format

When sharing on WhatsApp, the following information is included:
- Company name and branding
- System specifications
- Itemized pricing list
- Total cost
- Important notes
- Benefits summary
- Contact information
- Warranty details

---

## ⚙️ Setup Instructions

### Step 1: Upload Files
Place all three HTML files in your web directory:
```
/quotations.html
/quotation.html
/quotation-generator.html
/favicon.png (optional, for branding)
```

### Step 2: Update Phone Number
Replace `923252053313` with your country code and WhatsApp number:
- Format: `[country-code][phone-number]`
- Example: `923001234567` for Pakistan

### Step 3: Customize Company Details
Edit company information in each file:
- Company name
- Contact details
- Email
- Location

### Step 4: Test
1. Open `quotations.html` in browser
2. Test PDF download
3. Test WhatsApp sharing (on mobile or WhatsApp Desktop)
4. Verify formatting and details

---

## 🎯 Usage Scenarios

### Scenario 1: Sales Representative
Quickly generate and share quotes with customers:
1. Use custom quotation generator
2. Enter customer details
3. Adjust items/pricing as needed
4. Share on WhatsApp instantly

### Scenario 2: Website Visitor
Self-service quotation creation:
1. Navigate to quotations.html
2. Choose pre-built or custom quote
3. Download PDF to review
4. Share on WhatsApp to inquire

### Scenario 3: Email Proposal
Send professional quotation:
1. Generate custom quote
2. Download as PDF
3. Email PDF to customer
4. Follow up via WhatsApp

---

## 📞 Support & Troubleshooting

### PDF Not Downloading
- Check browser console for errors
- Ensure pop-ups are allowed
- Try different browser
- Check internet connection

### WhatsApp Not Opening
- Ensure WhatsApp is installed/set up
- On desktop: Install WhatsApp Desktop or Web
- On mobile: WhatsApp app must be default handler
- Check phone number format

### Formatting Issues
- Clear browser cache
- Try incognito/private window
- Test on different browser
- Check CSS loading

---

## 📈 Future Enhancements

Potential additions:
- ✨ Database integration for saved quotes
- ✨ Email delivery integration
- ✨ Multi-language support
- ✨ Signature/approval flow
- ✨ Payment integration
- ✨ Customer portal
- ✨ Analytics tracking
- ✨ Template customization UI

---

## 📄 License

These quotation tools are created for Bin Zareen Solar Pvt. Ltd.
For customization or licensing inquiries, contact the company.

---

## 🙏 Credits

Created for: **Bin Zareen Solar Pvt. Ltd.**
Location: **Islamabad, Pakistan**
Contact: **03252053313**

---

## 📞 Contact Information

**Bin Zareen Solar Pvt. Ltd.**
- 📱 WhatsApp: 03252053313
- 📞 Phone: 03252053313
- 📧 Email: binzareensolar@gmail.com
- 📍 Location: Islamabad, Pakistan
- 🌐 Website: binzareensolar.com

---

**Last Updated:** May 2024
**Version:** 1.0
