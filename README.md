# AI Return Evidence & Fraud Verification System

An intelligent, multi-stage automated return adjudication platform powered by computer vision, image forensics, perceptual hashing (pHash), Error Level Analysis (ELA), and risk-scoring decision engines.

---

## 🚀 Overview

This platform implements an automated pipeline for e-commerce return fraud prevention and damage inspection:

1. **Customer Evidence Portal**:
   - Product selection from purchase history
   - Multi-photo upload and video clip evidence
   - Real-time Laplacian blur and image clarity scoring
   - Instant decision result matching the 7 key metrics:
     - **Product**: Detected product category and contour
     - **Damage**: Damage classification (Crack, Scratch, Shatter, etc.)
     - **Severity**: Minor / Medium / Major / Critical
     - **Evidence**: Consistent vs. Inconclusive
     - **Image Quality**: Real-time sharpness scoring
     - **Duplicate**: Perceptual hash collision detection
     - **Risk Indicators**: Flagged risk score
     - **Decision Support**: `VALID` (Instant refund) / `REVIEW` (Hold for specialist) / `INSUFFICIENT` (Request clearer photos)
   - Prepaid shipping label generation and supplemental evidence upload.

2. **Admin Adjudication & Forensic Dashboard**:
   - Return claim queue with priority sorting and status filtering
   - **Evidence Comparison Engine**: Interactive split slider comparing return photos against seller shipment dispatch, product catalog CAD, and past return archives
   - **AI Vision & Forensics Core**: Product contour bounding boxes, damage trajectory localization, Error Level Analysis (ELA) compression heatmap, and EXIF metadata verification
   - **AI Decision Engine**: Explainable reasoning breakdown and manual adjudication overrides.

3. **Interactive Architecture Map**:
   - End-to-end interactive flowchart of the entire microservice ecosystem (Customer → Web/Mobile UI → FastAPI Gateway → Image/Order/Product Services → AI Vision Engine → Matcher → Severity → Comparison → Decision Engine → Portals)
   - Live JSON telemetry viewer for every node in the pipeline
   - Automated pulse simulation mode.

4. **Audit & Platform Statistics**:
   - Aggregated metrics on claims volume, autonomous approval rate (78.4%), fraud deflection savings, and damage type distribution.

---

## 🛠️ Technology Stack

- **Frontend**: React 18, TypeScript, Tailwind CSS, Lucide Icons
- **Fonts**: Syne (Headings), Outfit (Body), JetBrains Mono (Forensics & Code)
- **Forensic Utilities**: HTML5 Canvas Laplacian variance blur analysis, 64-bit perceptual hashing, error level manipulation simulation
- **Build Tool**: Vite

---

## 📦 Getting Started

### 1. Install Dependencies
```bash
npm install
```

### 2. Start Development Server
```bash
npm run dev
```
The application will be running at `http://localhost:3000`.

### 3. Build for Production
```bash
npm run build
```
The production bundle will be generated in the `dist/` directory.

---

## 📄 License
Apache-2.0
