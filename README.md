# 3CubedAI SEO Content Request Form

<!-- Last Deployment: July 18, 2025, 3:45 PM -->

A comprehensive SEO content request form designed for pharmaceutical products, built for Netlify Forms integration.

## 📋 Features

### Mandatory Fields (15)
- Product Name & Identifier
- Therapeutic Area & Medical Indication
- Development Stage
- Target Audience (multi-select)
- Geography (multi-select)
- Key Differentiators
- Competitor Products (with URLs)
- Unmet Medical Need
- Treatment Settings (multi-select)
- Competitive Positioning
- Brand Name Status
- Expected Launch Date
- Priority Markets (dynamic ranking)

### Optional Fields (15)
- Mechanism of Action
- Clinical Trial Details
- Primary Endpoints
- Safety Profile
- Dosing Information
- Patient Population
- Regulatory Status
- Market Size
- Additional Keywords
- Special Considerations
- Content Restrictions
- Existing Digital Assets
- Primary Advantage Type
- Conference Presence
- Key Opinion Leaders

### Dynamic Features
- Stage-based product name prefixing
- Conditional fields (Other therapeutic area, Brand name)
- Dynamic lists for competitors, conferences, and KOLs
- Priority market ranking when multiple geographies selected
- Form validation for required multi-selects

## 🚀 Deployment

### 1. Deploy to Netlify
- Fork or clone this repository
- Connect to Netlify
- Deploy site

### 2. Form Configuration
The form is pre-configured with:
```html
<form name="seo-content-request" method="POST" data-netlify="true" action="/success">
```

### 3. Success Page
Make sure to deploy the included `success.html` page for form submission confirmation.

## 📊 Integration

### Netlify Forms
- Forms are automatically detected on deploy
- Submissions stored in Netlify dashboard
- Webhook notifications available

### n8n Workflow
Configure n8n to:
1. Receive Netlify webhook
2. Process form fields
3. Insert into Supabase

### Supabase Schema
Matches the comprehensive schema with:
- `seo_requests` table (main fields)
- `seo_request_approvals` table
- All 30+ fields properly typed

## 📱 Features

- **Mobile Responsive**: Adapts to all screen sizes
- **Professional Design**: Clean, modern UI
- **Validation**: Client-side validation for required fields
- **User-Friendly**: Clear sections, help text, and examples

## 🔧 Customization

### Styling
Modify the embedded CSS in the `<style>` section to match your brand.

### Fields
Add or remove fields by editing the form sections. Remember to update:
- HTML form fields
- JavaScript validation
- Supabase schema
- n8n workflow mapping

## 📞 Support

For questions or issues:
- Check Netlify Forms documentation
- Review n8n webhook setup
- Verify Supabase schema matches

---

Built for 3CubedAI by InnovareAI