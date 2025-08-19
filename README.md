# TOTP Generator

A modern, responsive web application for generating Time-based One-Time Passwords (TOTP) built with React and TypeScript.

## Features

- **Real-time TOTP Generation**: Generates TOTP codes that update automatically
- **Configurable Parameters**: 
  - Secret key (Base32 encoded)
  - Number of digits (6 or 8)
  - Time period (30 or 60 seconds)
  - Hash algorithm (SHA1, SHA256, SHA512)
- **Responsive Design**: Works seamlessly on desktop, tablet, and mobile devices
- **Modern UI**: Clean, intuitive interface with smooth animations
- **TypeScript**: Full type safety and better development experience

## Technology Stack

- **Frontend**: React 19 with TypeScript
- **Build Tool**: Vite
- **TOTP Library**: otplib
- **Styling**: CSS3 with modern features and responsive design

## Getting Started

### Prerequisites

- Node.js (version 16 or higher)
- npm or yarn

### Installation

1. Clone the repository:
```bash
git clone <repository-url>
cd totp-generator
```

2. Install dependencies:
```bash
npm install
```

3. Start the development server:
```bash
npm run dev
```

4. Open your browser and navigate to `http://localhost:5173`

### Building for Production

```bash
npm run build
```

The built files will be in the `dist` directory.

## Usage

1. **Enter Secret Key**: Input your Base32 encoded secret key in the configuration form
2. **Configure Parameters**: Select the desired number of digits, time period, and algorithm
3. **Generate TOTP**: The application will automatically generate and display TOTP codes
4. **Auto-refresh**: Codes refresh automatically based on the selected time period

## Project Structure

```
src/
├── components/
│   └── TOTPGenerator/
│       ├── TOTPGenerator.tsx      # Main component
│       ├── TOTPForm.tsx          # Configuration form
│       ├── TOTPDisplay.tsx       # TOTP display and timer
│       ├── TOTPGenerator.css     # Main styles
│       ├── TOTPForm.css          # Form styles
│       └── TOTPDisplay.css       # Display styles
├── types/
│   └── TOTPTypes.ts              # TypeScript interfaces
├── utils/
│   └── totpUtils.ts              # TOTP generation utilities
├── App.tsx                       # Main app component
├── main.tsx                      # Entry point
└── index.css                     # Global styles
```

## Contributing

1. Fork the repository
2. Create a feature branch
3. Make your changes
4. Add tests if applicable
5. Submit a pull request

## License

This project is open source and available under the [MIT License](LICENSE).

## Security Note

This application generates TOTP codes locally in your browser. Your secret keys are never sent to external servers. However, always ensure you're using this on a secure, trusted device and network.
