# LA Chargers 2026 Salary Cap Dashboard

An interactive web dashboard for analyzing the LA Chargers' 2026 salary cap situation, featuring cut candidates analysis and a drag-and-drop depth chart builder.

## Features

- **Salary Cap Analysis**: View current cap space and impact of potential cuts
- **Cut Candidates**: Track 4 key players (Mekhi Becton, Bradley Bozeman, Bud Dupree, Will Dissly) with detailed cap savings breakdown
- **Interactive Depth Chart**:
  - Drag-and-drop player positioning for Offense, Defense, and Special Teams
  - Proper football formation layouts
  - Player pool sidebar for roster management
  - Auto-save functionality (persists across page refreshes)
  - Visual distinction for cut candidates (red borders)
- **Cap Savings Calculator**: Real-time calculation showing new available cap space after cuts

## Live Demo

Visit the live dashboard: [https://joshgray300.github.io/chargers-dashboard/](https://joshgray300.github.io/chargers-dashboard/)

## Data Source

All player data and salary cap information sourced from [Over The Cap - LA Chargers](https://overthecap.com/salary-cap/los-angeles-chargers)

## How to Use

1. **View Cut Candidates**: See the potential cap savings from cutting each player
2. **Interact with Depth Chart**:
   - Drag any player card to a different position
   - Move players between the main depth chart and player pool
   - Your changes are automatically saved in your browser
   - Click "Reset to Default" to restore original positions
3. **Analyze Cap Impact**: Review the total savings calculation showing how cuts increase available cap space

## Technical Details

- Single HTML file with embedded CSS and JavaScript
- No dependencies or external libraries
- Uses browser localStorage for persistence
- Fully responsive design
- Team colors: Chargers Blue (#0080C6) and Gold (#FFC20E)

## Local Development

Simply open `index.html` in any modern web browser. No build process required.

## Project Structure

```
chargers-dashboard/
├── index.html          # Main dashboard file
└── README.md          # This file
```

## Key Players & Cap Savings (2026)

| Player | Position | Cap Hit | Dead Money | Cap Savings |
|--------|----------|---------|------------|-------------|
| Mekhi Becton | OL | $12.2M | $2.5M | $9.7M |
| Bradley Bozeman | C | $6.935M | $1.06M | $5.875M |
| Will Dissly | TE | $5.5M | $1.5M | $4M |
| Bud Dupree | EDGE | $3.74M | $250K | $3.49M |
| **TOTAL** | | **$28.375M** | **$5.31M** | **$23.065M** |

Cutting all four players would increase available cap space from $80.6M to **$103.665M**.

## Browser Compatibility

Works in all modern browsers:
- Chrome/Edge (recommended)
- Firefox
- Safari
- Opera

## License

This is a fan-made project for educational and analytical purposes. All team trademarks and player data belong to their respective owners.

## Contributing

Feel free to fork this repository and submit pull requests for improvements!

## Author

Created by Josh Gray ([@joshgray300](https://github.com/joshgray300))

## Updates

To push updates to this dashboard:
1. Make your changes to `index.html` locally
2. Test in your browser
3. Run: `git add .`
4. Run: `git commit -m "Your update message"`
5. Run: `git push origin main`

---

**Bolt Up!** ⚡
