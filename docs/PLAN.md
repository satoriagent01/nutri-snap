# NutriSnap - Plan

## Requirements
- Take photos of nutrition labels from product packaging
- Use OCR + AI to extract nutrition information (calories, fats, carbs, proteins, sodium, etc.)
- Allow custom tracking of any nutritional component
- Meal planner: specify grams of each product in a plate
- Free and open source, no ads
- Support for multiple languages (Dutch, German, French, Italian, English, Spanish)

## Architecture
- **Frontend**: Vanilla HTML/CSS/JS (no framework needed for simplicity)
- **Backend**: Node.js + Express (serves static files, proxies OCR requests)
- **OCR**: Uses Tesseract.js client-side for label recognition
- **Storage**: localStorage for persistence (no backend database needed)
- **Testing**: Jest for unit tests on parsing logic

## Key Decisions
1. **Client-side OCR**: Tesseract.js runs in the browser, no API keys needed
2. **localStorage**: Simple persistence, no server required beyond static hosting
3. **Custom nutrients**: Users can define their own tracking metrics
4. **Multi-language**: OCR handles multiple languages, UI in English with i18n support
5. **No ads, free**: Pure open source project

## What's Not Done Yet
- Cloud sync between devices
- Barcode scanning for product lookup
- Recipe integration
- Export/import data
- Mobile app (PWA support could be added)

## Next Steps
- Implement the core UI and OCR flow
- Add meal planning features
- Polish the UI/UX
- Add PWA support for mobile use