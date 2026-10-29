# Kanha RO Services Website

A six-page responsive website built with HTML5, CSS3 and vanilla JavaScript.

## Project structure

```text
Kanha-RO-Website/
├── index.html
├── services.html
├── sales.html
├── distribution.html
├── installation.html
├── contact.html
├── css/
│   └── style.css
├── js/
│   └── script.js
├── images/
│   ├── kanha-ro-logo.png       # Add your original logo here
│   ├── hero-ro.svg
│   ├── ro-service.svg
│   ├── ro-products.svg
│   ├── ro-installation.svg
│   └── ro-spare-parts.svg
└── README.md
```

## Open in Visual Studio Code

1. Download and extract `Kanha-RO-Website.zip`.
2. Open Visual Studio Code.
3. Select **File → Open Folder**.
4. Choose the extracted `Kanha-RO-Website` folder.
5. Add your original logo to `images/` and name it `kanha-ro-logo.png`.

## Run locally with Live Server

1. Install the **Live Server** extension in VS Code.
2. Open `index.html`.
3. Right-click inside the editor and choose **Open with Live Server**.
4. The site will open in your browser. Navigate through the six pages using the header.

You can also double-click `index.html` to open it directly, but Live Server is recommended.

## Important setup before publishing

### 1. Contact details and WhatsApp

Open `js/script.js` and update:

```js
const KANHA_CONFIG = {
  whatsappNumber: "91XXXXXXXXXX", // digits only, with country code
  phoneNumber: "+91XXXXXXXXXX"
};
```

Use your actual business phone number. The WhatsApp number should be digits only, for example `919876543210`.

Also search the HTML files for:
- `[Add business phone number]`
- `[Add WhatsApp number]`
- `[Add business email]`
- `[Add complete business address]`
- `[Add days and working hours]`
- `[Add city and nearby areas]`

Replace all placeholders with verified details.

### 2. Logo

Copy your original, unchanged logo into `images/kanha-ro-logo.png`. The header already points to that exact path.

### 3. SEO and local business data

In every HTML file, replace:
- `https://www.example.com/...` in the canonical and Open Graph URL fields.
- `https://www.example.com/images/...` in the Open Graph and JSON-LD image fields.
- Placeholder telephone, email, address and opening hours in the LocalBusiness JSON-LD.

Use one consistent preferred domain (www or non-www) and set canonical URLs to the live page URLs.

### 4. Google Maps

On `contact.html`, replace the map placeholder with a Google Maps iframe embed for your verified business address. Use the embed code from Google Maps → Share → Embed a map. Add a descriptive `title` attribute to the iframe.

### 5. Forms

Forms validate required fields in the browser and then prepare a WhatsApp message. They do not submit to a server, store customer data, or display a false server-submission confirmation. A customer must review and press Send in WhatsApp.

### 6. Product claims and pricing

Product cards are category-level examples. Add real product images and verified model-specific features, specifications, warranty and pricing before publishing. AMC prices and inclusions are editable placeholders.

## Files to edit

- Content and page sections: the relevant `.html` file.
- Colours, spacing and responsive layout: `css/style.css` (edit the CSS variables at the top first).
- WhatsApp number, mobile menu, forms and interactions: `js/script.js`.
- Images: `images/`.

## Pre-launch checklist

- [ ] Add the original logo as `images/kanha-ro-logo.png`.
- [ ] Update phone and WhatsApp numbers.
- [ ] Update email, address, hours and service locations.
- [ ] Replace canonical URLs and structured-data placeholders.
- [ ] Add the correct Google Maps embed.
- [ ] Replace illustrative product/category images with genuine authorized product images where available.
- [ ] Verify all product claims, pricing, AMC coverage and service availability.
- [ ] Test all six pages on mobile and desktop.
- [ ] Test call links, WhatsApp links, forms, FAQ accordion and navigation.
- [ ] Add a privacy policy if collecting personal information through a backend in the future.
