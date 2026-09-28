# NutriSnap

A free, open-source nutrition label scanner and meal planner. Snap a photo of any food label, extract the nutrition data with OCR, and track calories, macros, sodium, or any custom nutrient.

## Features

- **Photo to Nutrition Data**: Take a photo of a nutrition label and extract the data automatically
- **Custom Tracking**: Track any nutrient - calories, sodium, saturated fat, or anything else
- **Meal Planning**: Build custom meals by specifying grams of each ingredient
- **No Ads, No Paywalls**: Completely free and open source

## How It Works

1. Take a photo of a nutrition label (or upload one)
2. The app extracts the nutrition information using OCR
3. Parse and structure the data (calories, fats, carbs, proteins, etc.)
4. Add items to your daily meal plan
5. Track your intake across all meals

## Setup

### Prerequisites

- Node.js (v14 or higher)
- npm

### Installation

```bash
npm install
```

### Running

```bash
npm start
```

The app will be available at `http://localhost:3000`

## Testing

```bash
npm test
```

## Tech Stack

- **Frontend**: Vanilla HTML, CSS, JavaScript
- **Backend**: Node.js with Express
- **OCR**: Tesseract.js for text recognition
- **Testing**: Jest

## What's Not Done Yet

- Integration with external nutrition databases (USDA, OpenFoodFacts)
- User accounts and cloud sync
- Barcode scanning
- Recipe suggestions based on tracked nutrients
- Export data to CSV or other formats
- Mobile app (responsive web only for now)

## License

MIT