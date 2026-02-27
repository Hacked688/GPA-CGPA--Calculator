# 🎓 GPA Calculator

A modern, feature-rich GPA calculator built with **Next.js 16**, **React 19**, and **Tailwind CSS 4**. Calculate your cumulative and semester GPA with customizable grading scales, what-if analysis, trend analytics, and achievement tracking.

![Next.js](https://img.shields.io/badge/Next.js-16-black?logo=next.js)
![React](https://img.shields.io/badge/React-19-61DAFB?logo=react)
![TypeScript](https://img.shields.io/badge/TypeScript-5-3178C6?logo=typescript)
![Tailwind CSS](https://img.shields.io/badge/Tailwind_CSS-4-06B6D4?logo=tailwindcss)
![License](https://img.shields.io/badge/License-MIT-green)

## ✨ Features

### Core Functionality
- **Cumulative & Semester GPA** — Calculate both overall and per-semester GPA with detailed breakdowns
- **Customizable Grading Scales** — Support for 4.0, 4.3, percentage-based, and fully custom scales
- **Plus/Minus Grading** — Optional +/- grade modifiers with configurable increments
- **Pass/Fail Handling** — Configurable pass/fail thresholds
- **Course Retake Support** — Automatic grade replacement for retaken courses

### Institution Presets
Pre-configured grading policies for universities worldwide:
- 🇺🇸 **USA** — Standard 4.0, Plus/Minus 4.0, Extended 4.3
- 🇮🇳 **India** — 10-Point CGPA, Percentage System
- 🇬🇧 **UK** — Honours Classification
- 🇨🇦 **Canada** — 4.0 Scale
- 🇦🇺 **Australia** — 7-Point Scale
- 🇩🇪 **Germany** — 1.0–5.0 Scale
- 🇫🇷 **France** — 20-Point Scale

### Advanced Analytics
- **What-If Analysis** — Simulate grade changes and see how they impact your GPA
- **Target GPA Tracker** — Find out what grades you need to reach your goal GPA
- **Trend Analytics** — Visualize your GPA trends across semesters with interactive charts
- **Achievement Badges** — Earn badges based on your academic milestones

### Export & Persistence
- **PDF & CSV Export** — Download your GPA report as a formatted PDF or CSV file
- **Local Storage** — Your data is automatically saved in the browser and restored on return

### User Experience
- **3-Step Guided Workflow** — Grading Policy → Add Courses → View Results
- **Sample Data** — Load sample courses to explore features instantly
- **Responsive Design** — Works seamlessly on desktop, tablet, and mobile
- **Glass Morphism UI** — Modern dark theme with glowing accents and smooth animations

## 🚀 Getting Started

### Prerequisites
- [Node.js](https://nodejs.org/) 18+
- [pnpm](https://pnpm.io/) (recommended) or npm

### Installation

```bash
# Clone the repository
git clone https://github.com/<your-username>/gpa-calculator-app.git
cd gpa-calculator-app

# Install dependencies
pnpm install

# Start the development server
pnpm dev
```

Open [http://localhost:3000](http://localhost:3000) in your browser.

### Build for Production

```bash
pnpm build
pnpm start
```

## 🛠️ Tech Stack

| Category | Technology |
|---|---|
| Framework | Next.js 16 (Turbopack) |
| Language | TypeScript 5 |
| UI Library | React 19 |
| Styling | Tailwind CSS 4, tw-animate-css |
| Components | Radix UI, shadcn/ui |
| Charts | Recharts |
| Forms | React Hook Form + Zod |
| PDF Export | jsPDF |
| Icons | Lucide React |
| Analytics | Vercel Analytics |

## 📁 Project Structure

```
├── app/                  # Next.js app router
│   ├── layout.tsx        # Root layout
│   ├── page.tsx          # Main page (3-step wizard)
│   └── globals.css       # Global styles
├── components/           # React components
│   ├── AchievementBadges.tsx
│   ├── CourseEntry.tsx
│   ├── ExportButtons.tsx
│   ├── GradingPolicySetup.tsx
│   ├── QuickPolicySetup.tsx
│   ├── ResultsDisplay.tsx
│   ├── TargetGPATracker.tsx
│   ├── TrendAnalytics.tsx
│   ├── WhatIfAnalysis.tsx
│   └── ui/               # shadcn/ui components
├── lib/                  # Core logic & utilities
│   ├── gpaCalculator.ts  # GPA calculation engine
│   ├── exportUtils.ts    # PDF & CSV export
│   ├── institutionPresets.ts  # Grading scale presets
│   ├── sampleData.ts     # Sample courses & policies
│   ├── types.ts          # TypeScript type definitions
│   └── __tests__/        # Unit tests
└── hooks/                # Custom React hooks
```

## 📄 License

This project is licensed under the MIT License.
