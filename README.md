# Restaurant QR Menu System

A simple, mobile-friendly QR code menu system for restaurants that can be easily deployed on GitHub Pages. This project allows restaurant owners to create a digital menu system with QR codes that customers can scan to view menus and leave reviews.

## Overview

The digital menu system consists of three main components:

1. **Main QR Page** (`index.html`) - A QR code that customers can scan to view the restaurant menu
2. **Menu Viewer** (`viewer.html`) - The page that loads when customers scan the QR code
3. **Review Collection** (`review.html`) - A page with a QR code for collecting Google Reviews

## Demo

You can see a live demo of this project at:
- [https://desi-videsi.github.io/restaurent-files/](https://desi-videsi.github.io/restaurent-files/)

Please note that this demo uses the proprietary logo and menu of Desi Videsi Restaurant. When you fork this project, you must replace these with your own content.

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

## How to Use This Project

### Fork and Deploy
1. Fork this repository to your GitHub account
2. **Replace the logo and menu PDF with your own content** (the current logo and menu are proprietary and not for redistribution)
3. Update the restaurant information in all HTML files:
   - Restaurant name
   - Address and map link
   - Phone numbers
   - Hours of operation
   - Google review link
4. Enable GitHub Pages in repository settings
5. Your menu system will be available at `https://[your-username].github.io/[repository-name]/`

### Customization
You can easily customize the look and feel by modifying the CSS in the HTML files:
- Change colors to match your brand
- Adjust sizes and spacing
- Modify layout as needed

## Contributing
Contributions are welcome! If you'd like to improve this project:
1. Fork the repository
2. Create a feature branch (`git checkout -b feature/amazing-feature`)
3. Commit your changes (`git commit -m 'Add some amazing feature'`)
4. Push to the branch (`git push origin feature/amazing-feature`)
5. Open a Pull Request

## Print Usage

The index.html page is optimized for printing as a 4x6 inch standee. Use the browser's print function and set the paper size to 4x6 inches for best results.

## Contact

For questions or assistance, please contact:
- Name: Gopal Kedia
- Phone: +91 7894420103

## License

The code in this project is open source and available under the MIT License. This includes all HTML, CSS, and JavaScript code.

```
MIT License

Copyright (c) 2025 Gopal Kedia

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
SOFTWARE.
```

**Note:** The logo, menu PDF, and any other branding elements specific to Desi Videsi Restaurant are proprietary and are NOT covered by this license. These elements must be replaced if you fork this repository.
