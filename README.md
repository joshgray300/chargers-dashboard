# Guilty As Charged 2026 Offseason Hub

An interactive web dashboard for analyzing the LA Chargers' 2026 salary cap situation, featuring cut candidates analysis, drag-and-drop depth chart builder, and comprehensive free agency tools.

## Features

### Salary Cap Management
- **Real-time Cap Tracking**: View current cap space ($80.6M) and dynamic adjustments
- **Cut Candidates Analysis**: Track 4 key players with detailed cap savings breakdown
  - Mekhi Becton (OL): $9.7M savings
  - Bradley Bozeman (C): $5.875M savings
  - Will Dissly (TE): $4M savings
  - Bud Dupree (EDGE): $3.49M savings
  - **Total savings**: $23.065M → increases cap to $103.665M
- **Automatic Cap Calculator**: Real-time updates as you move players and set contracts

### Coaching Staff & Front Office
- **Organizational Chart**: Color-coded hierarchy display
  - Front Office: GM Joe Hortiz, AGM Chad Alexander
  - Head Coach: Jim Harbaugh
  - Coordinators: OC Mike McDaniel, DC Chris O'Leary
  - Position coaches and special teams staff
  - Visual color coding by department

### Interactive Depth Chart
- **Drag-and-Drop Interface**: Move players between any position
- **Full Roster Management**:
  - Offense: All 11 positions with depth
  - Defense: 4-3 formation with multiple depth levels
  - Special Teams: K, P, LS positions
  - Reserves: Flexible practice squad simulation
- **Proper Football Formations**: Authentic offensive and defensive alignments
- **Auto-save**: All changes persist across page refreshes via localStorage
- **Visual Indicators**: Cut candidates marked with red borders

### Free Agent Pool (2026 FA Class)
- **Tabbed Interface**: Easy navigation across 10 position groups
  - **RB**: 50+ running backs (Najee Harris, Saquon Barkley, Breece Hall, etc.)
  - **TE**: 15+ tight ends (Dallas Goedert, David Njoku, etc.)
  - **LT**: 33+ left tackles (Jonah Williams, Cam Robinson, Charles Cross, etc.)
  - **LG**: 15+ left guards (Joel Bitonio, Zion Johnson, etc.)
  - **C**: 15+ centers (Connor McGovern, Tyler Linderbaum, etc.)
  - **RG**: 14+ right guards (Wyatt Teller, Alijah Vera-Tucker, etc.)
  - **EDGE**: Edge rushers available
  - **IDL**: Interior defensive linemen
  - **LB**: 85+ linebackers (Lavonte David, Bobby Wagner, Demario Davis, Devin White, etc.)
  - **S**: 15+ safeties (Tony Jefferson, Chauncey Gardner-Johnson, etc.)
- **Sticky Sidebar**: Pool stays visible while scrolling main page
- **Internal Scrolling**: Smooth scrolling within FA pool (85vh height)
- **Contract Setting**: Click any FA to set contract value
- **Team & Age Display**: Shows player's current team and age
- **Edit Contracts**: Double-click green cards to modify existing contracts

### Custom Player Tools
- **Add Custom Player**: Create free agents with custom details
  - Enter name, age (20-45), position, and contract value
  - Automatically added to appropriate FA pool tab
  - Full drag-and-drop support
  - Editable via double-click
- **Add Draft Pick**: Simulate draft selections
  - Select draft round (1-7)
  - Assign position and rookie contract value
  - Displays as "Draft Pick • Rd X"
  - Full roster integration with drag-and-drop
  - Yellow-themed interface matching cap space colors

## Live Demo

Visit the live dashboard: [https://joshgray300.github.io/chargers-dashboard/](https://joshgray300.github.io/chargers-dashboard/)

## Data Source

All player data and salary cap information sourced from [Over The Cap - LA Chargers](https://overthecap.com/salary-cap/los-angeles-chargers)

## How to Use

### Basic Operations
1. **View Coaching Staff**: See the complete organizational chart at the top
2. **Check Cap Space**: Monitor current cap space and see real-time adjustments
3. **Review Cut Candidates**: Analyze potential cap savings from each player

### Building Your Roster
4. **Browse Free Agents**:
   - Click position tabs (RB, TE, LT, LG, C, RG, EDGE, IDL, LB, S) to view available players
   - Scroll within the FA pool to see all options
   - FA pool stays visible as you scroll the main page
5. **Set Contracts**:
   - Click any gray free agent card to set their contract value
   - Green cards indicate contracts are set
   - Double-click green cards to edit contract amounts
6. **Add Custom Players**:
   - Click "+ Add Custom Player" (green button)
   - Enter player details: name, age, position, contract
   - Player automatically appears in their position's FA pool tab
7. **Add Draft Picks**:
   - Click "+ Add a draft pick" (yellow button)
   - Select round (1-7), position, and rookie contract value
   - Draft pick appears in appropriate FA pool tab

### Managing the Depth Chart
8. **Drag and Drop**:
   - Drag any player card to reposition them
   - Move players from FA pool to depth chart positions
   - Rearrange depth chart order (starters vs backups)
   - Move players to reserves or back to FA pool
9. **Auto-save**: All changes automatically save to your browser
10. **Reset**: Click "Reset to Default" to restore original lineup

### Cap Management
11. **Monitor Changes**: Watch the "ROSTER CHANGES" tracker update in real-time
12. **Calculate Available Cap**: See your total available cap space after all moves
13. **Optimize Roster**: Balance talent acquisition with cap space management

## Technical Details

### Architecture
- **Single HTML File**: Embedded CSS and JavaScript (~2000+ lines)
- **Zero Dependencies**: Pure vanilla JavaScript, no external libraries
- **Client-side Only**: All processing happens in the browser

### Data Persistence
- **localStorage API**: Saves complete roster state including:
  - Player positions and depth chart arrangements
  - Custom players and draft picks
  - Contract values for all free agents
  - Cut candidate status with cap savings data
- **Auto-save**: Triggers on every roster change
- **State Recovery**: Automatically loads saved state on page refresh

### Features Implementation
- **Drag & Drop API**: Native HTML5 drag-and-drop for player movement
- **Modal Dialogs**: Custom contract input and player creation interfaces
- **Tabbed Interface**: Dynamic tab switching for FA pool navigation
- **Sticky Positioning**: CSS position: sticky for FA pool sidebar
- **Viewport-based Sizing**: FA pool uses 85vh for optimal scrolling
- **Real-time Calculations**: Dynamic cap space tracking with every change

### Styling
- **Chargers Brand Colors**:
  - Primary Blue: #0080C6
  - Gold/Yellow: #FFC20E / #FFD700
  - Gradients for buttons and headers
- **Color-coded UI**:
  - Green: Add Custom Player, positive values
  - Yellow: Add Draft Pick, available cap
  - Red: Cut candidates, negative values
  - Blue: Front Office, Offensive Staff, Special Teams
  - Gold: Head Coach, Defensive Staff
- **Responsive Design**: Adapts to different screen sizes
- **Custom Scrollbars**: Chargers blue-themed scrollbars

## Local Development

Simply open `index.html` in any modern web browser. No build process required.

## Project Structure

```
chargers-dashboard/
├── index.html          # Main dashboard file
└── README.md          # This file
```

## Free Agent Pool Overview

The dashboard includes 235+ real 2026 free agents across 10 position groups:

| Position | Count | Notable Players |
|----------|-------|-----------------|
| RB | 50+ | Najee Harris, Saquon Barkley, Breece Hall, Kenneth Walker III, J.K. Dobbins, Kimani Vidal |
| TE | 15+ | Dallas Goedert, David Njoku, Cade Otton, Isaiah Likely |
| LT | 33+ | Jonah Williams, Cam Robinson, Charles Cross, Trevor Penning, Jermaine Eluemunor |
| LG | 15+ | Joel Bitonio, Isaac Seumalo, Zion Johnson, David Edwards |
| C | 15+ | Connor McGovern, Tyler Linderbaum, Ethan Pocic |
| RG | 14+ | Wyatt Teller, Alijah Vera-Tucker, Kevin Zeitler |
| EDGE | Multiple | Top pass rushers available |
| IDL | Multiple | Interior defensive line depth |
| LB | 85+ | Lavonte David, Bobby Wagner, Demario Davis, Kenneth Murray, Devin White, Denzel Perryman |
| S | 15+ | Tony Jefferson, Chauncey Gardner-Johnson, Bryan Cook |

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

## Recent Updates

### January 2026 - Latest Updates
- ✅ Rebranded to **"Guilty As Charged 2026 Offseason Hub"**
- ✅ Added LB tab with 85+ linebackers (Lavonte David, Bobby Wagner, Devin White, etc.)
- ✅ Updated coaching staff color scheme for better visual hierarchy
  - Offensive Staff & Special Teams: Chargers blue
  - Defensive Staff: Gold (matching Head Coach)
- ✅ Expanded to 10 total FA position tabs (235+ players)

### January 2026 - Major Feature Expansion
- ✅ Added RB tab with 50+ running backs to FA pool
- ✅ Added LT tab with 33+ left tackles to FA pool
- ✅ Expanded S pool with Tony Jefferson and others
- ✅ Implemented "Add a draft pick" functionality with round selection
- ✅ Added coaching staff organizational chart (DC Chris O'Leary, AGM Chad Alexander)
- ✅ Fixed FA pool with sticky positioning and internal scrolling
- ✅ Moved Cam Hart to CB1 behind Donte Jackson
- ✅ Enhanced UX with viewport-based sizing (85vh)

### Initial Release
- Interactive depth chart with drag-and-drop
- Cut candidates analysis with cap savings
- Free agent pool with contract management
- Auto-save functionality

## Contributing

To push updates to this dashboard:
1. Make your changes to `index.html` locally
2. Test in your browser
3. Run: `git add .`
4. Run: `git commit -m "Your update message"`
5. Run: `git push origin main`

Pull requests are welcome! Please ensure your changes:
- Maintain the existing color scheme
- Include proper error handling
- Test across different browsers
- Update this README with new features

---

**Bolt Up!** ⚡
