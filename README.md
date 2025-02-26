# Desi Videsi Restaurant - Digital Menu System

This repository contains the digital menu system for Desi Videsi Restaurant, featuring QR code menu access and customer review collection.

## Overview

The digital menu system consists of three main components:

1. **Main QR Page** (`index.html`) - A QR code that customers can scan to view the restaurant menu
2. **Menu Viewer** (`viewer.html`) - The page that loads when customers scan the QR code
3. **Review Collection** (`review.html`) - A page with a QR code for collecting Google Reviews

## Features

- **Mobile-Optimized**: All pages are fully responsive and work well on all device sizes
- **QR Code Menu**: Easy access to the restaurant menu through a simple QR scan
- **Digital Menu Access**: Options to view the menu online or download as PDF
- **Google Review Collection**: Dedicated page for collecting customer reviews
- **Contact Information**: Easily accessible restaurant details including:
  - Address with Google Maps integration
  - Phone numbers with click-to-call functionality
  - Business hours

## Technical Details

### File Structure

- `index.html` - Main QR code page
- `viewer.html` - Menu viewing page
- `review.html` - Review collection page
- `Menu Card.pdf` - The actual menu PDF file
- `Desi Videsi Final edit Transparent Format.png` - Restaurant logo

### QR Code Usage

The QR codes are generated using the [QRCode.js](https://github.com/davidshimjs/qrcodejs) library. When scanned:

- The menu QR code directs customers to the viewer page
- The review QR code directs customers to Google Reviews

## Installation and Usage

### Local Testing

1. Clone this repository
2. Open the HTML files in a web browser to preview

### Deployment

This project is designed to be hosted on GitHub Pages:

1. Fork or clone this repository
2. Enable GitHub Pages in repository settings
3. Set the source to the main branch
4. Access your site at `https://[username].github.io/restaurent-files/`

### Customization

To customize this for another restaurant:

1. Replace the logo image
2. Update contact information in all HTML files
3. Replace the menu PDF file
4. Update the Google Review link in `review.html`

## Print Usage

The index.html page is optimized for printing as a 4x6 inch standee. Use the browser's print function and set the paper size to 4x6 inches for best results.

## Contact

For questions or assistance, please contact:
- Phone: +91 9051355751 / +91 9331645333
- Address: Ajmir Tower 14B Beleghata Main Road, Kolkata 700 010

## License

This project is available for use by Desi Videsi Restaurant.
