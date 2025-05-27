# MVP User Stories - PredictVN Testnet

## 📋 Overview

This document outlines detailed user stories for the MVP testnet phase of PredictVN. These stories define the core functionality needed to validate the prediction market concept and gather user feedback.

## 👥 User Personas

### Primary Users:
- **🎲 Casual Trader** (60%) - Interested in predicting events for entertainment and potential profit
- **💼 Professional Trader** (25%) - Systematic approach to prediction market trading
- **🏦 Market Maker** (10%) - Provides liquidity to earn fees
- **👨‍💼 Platform Admin** (5%) - Manages platform operations and markets

---

## 🎲 Casual Trader User Stories

### Wallet & Setup
**As a casual trader, I want to easily connect my wallet and get started quickly.**

- **Story 1.1**: Connect Wallet
  - **As a** casual trader
  - **I want to** connect my MetaMask wallet to the platform
  - **So that** I can start trading on prediction markets
  - **Acceptance Criteria**:
    - Click "Connect Wallet" button
    - MetaMask popup appears for connection
    - Wallet address displayed after successful connection
    - Can disconnect and reconnect wallet

- **Story 1.2**: Get Test Tokens
  - **As a** casual trader
  - **I want to** get free test USDC from a faucet
  - **So that** I can try trading without real money
  - **Acceptance Criteria**:
    - "Get Test USDC" button visible when connected
    - Receive 1000 test USDC per day
    - Balance updates immediately after claiming
    - Clear instructions on testnet usage

### Market Discovery
**As a casual trader, I want to easily find interesting markets to trade.**

- **Story 2.1**: Browse Markets
  - **As a** casual trader
  - **I want to** see a list of available prediction markets
  - **So that** I can find topics I'm interested in
  - **Acceptance Criteria**:
    - Market list shows market name, description, end date
    - Current YES/NO prices visible
    - Trading volume displayed
    - Markets sorted by activity/volume

- **Story 2.2**: Search Markets
  - **As a** casual trader
  - **I want to** search for specific markets by keyword
  - **So that** I can quickly find markets about topics I care about
  - **Acceptance Criteria**:
    - Search bar prominent on market listing page
    - Results update as I type
    - Can search by market title, description, category
    - "No results found" message when appropriate

- **Story 2.3**: Filter Markets
  - **As a** casual trader
  - **I want to** filter markets by category and status
  - **So that** I can focus on relevant markets
  - **Acceptance Criteria**:
    - Filter options: All, Politics, Sports, Crypto, Entertainment
    - Filter by status: Active, Ending Soon, Recently Added
    - Filters can be combined
    - Clear filters option available

### Trading
**As a casual trader, I want to place trades easily and understand what's happening.**

- **Story 3.1**: View Market Details
  - **As a** casual trader
  - **I want to** see detailed information about a market
  - **So that** I can make informed trading decisions
  - **Acceptance Criteria**:
    - Market question clearly displayed
    - Resolution criteria explained
    - End date and current status visible
    - Recent trading activity shown
    - Current order book (simplified view)

- **Story 3.2**: Place Buy Order
  - **As a** casual trader
  - **I want to** buy YES or NO tokens for a market
  - **So that** I can express my prediction
  - **Acceptance Criteria**:
    - Simple buy interface with quantity and price inputs
    - Clear indication of YES vs NO selection
    - Total cost calculation displayed
    - Confirmation dialog before placing order
    - Order appears in "My Orders" section

- **Story 3.3**: Place Sell Order
  - **As a** casual trader
  - **I want to** sell my position tokens
  - **So that** I can lock in profits or cut losses
  - **Acceptance Criteria**:
    - Can only sell tokens I own
    - Current position displayed clearly
    - Estimated proceeds shown
    - Confirmation required before selling
    - Balance updates after successful sale

- **Story 3.4**: Cancel Orders
  - **As a** casual trader
  - **I want to** cancel my pending orders
  - **So that** I can change my mind or adjust my strategy
  - **Acceptance Criteria**:
    - "Cancel" button visible for pending orders
    - Confirmation dialog prevents accidental cancellation
    - Order removed from order book immediately
    - USDC returned to balance for buy orders
    - Tokens returned for sell orders

### Portfolio Management
**As a casual trader, I want to track my positions and performance.**

- **Story 4.1**: View Portfolio
  - **As a** casual trader
  - **I want to** see all my current positions
  - **So that** I can track my investments
  - **Acceptance Criteria**:
    - List of all markets I have positions in
    - Number of YES/NO tokens owned per market
    - Current market value of positions
    - Unrealized profit/loss displayed
    - Link to trade more in each market

- **Story 4.2**: View Order History
  - **As a** casual trader
  - **I want to** see my past trades and orders
  - **So that** I can learn from my trading patterns
  - **Acceptance Criteria**:
    - Chronological list of all orders (filled, cancelled, pending)
    - Order details: market, side, quantity, price, timestamp
    - Filter by status, market, date range
    - Export to CSV option

- **Story 4.3**: See Balance
  - **As a** casual trader
  - **I want to** easily see my current USDC balance
  - **So that** I know how much I can trade with
  - **Acceptance Criteria**:
    - Balance prominently displayed in header
    - Updates in real-time after trades
    - Available vs locked balance shown
    - Balance history accessible

### Real-time Updates
**As a casual trader, I want to see live market activity.**

- **Story 5.1**: Live Price Updates
  - **As a** casual trader
  - **I want to** see prices update without refreshing the page
  - **So that** I can react quickly to market movements
  - **Acceptance Criteria**:
    - Prices update within 3 seconds of trades
    - Visual indication when prices change
    - No page refresh required
    - Works across all market pages

- **Story 5.2**: Order Notifications
  - **As a** casual trader
  - **I want to** be notified when my orders are filled
  - **So that** I know when my trades execute
  - **Acceptance Criteria**:
    - In-app notification when order fills
    - Shows market name, quantity, and price
    - Notification persists until acknowledged
    - Audio notification option

---

## 💼 Professional Trader User Stories

### Advanced Trading
**As a professional trader, I want efficient trading tools and detailed market data.**

- **Story 6.1**: Quick Order Entry
  - **As a** professional trader
  - **I want to** place orders quickly with keyboard shortcuts
  - **So that** I can execute my strategies efficiently
  - **Acceptance Criteria**:
    - Keyboard shortcuts for buy/sell (B/S keys)
    - Quick quantity selection (1%, 5%, 10%, 25%, 50%, 100% of balance)
    - Tab navigation between price and quantity fields
    - Enter key submits order

- **Story 6.2**: Order Book Analysis
  - **As a** professional trader
  - **I want to** see detailed order book information
  - **So that** I can understand market depth and liquidity
  - **Acceptance Criteria**:
    - Full order book display with all price levels
    - Cumulative volume at each level
    - Spread calculation shown
    - Order book depth visualization
    - My orders highlighted in different color

- **Story 6.3**: Market Data Export
  - **As a** professional trader
  - **I want to** export trading data and market history
  - **So that** I can analyze markets offline
  - **Acceptance Criteria**:
    - Export trades to CSV/JSON
    - Export order book snapshots
    - Export market price history
    - Date range selection for exports
    - API access for automated data collection

### Portfolio Analytics
**As a professional trader, I want detailed performance metrics.**

- **Story 7.1**: P&L Tracking
  - **As a** professional trader
  - **I want to** see detailed profit and loss calculations
  - **So that** I can measure my trading performance
  - **Acceptance Criteria**:
    - Realized vs unrealized P&L
    - P&L by market category
    - Daily, weekly, monthly P&L summaries
    - Return on investment percentage
    - Benchmark comparison (if available)

- **Story 7.2**: Trade Analytics
  - **As a** professional trader
  - **I want to** analyze my trading patterns
  - **So that** I can improve my strategies
  - **Acceptance Criteria**:
    - Win rate percentage
    - Average profit per winning trade
    - Average loss per losing trade
    - Trade frequency analysis
    - Market category performance breakdown

---

## 🏦 Market Maker User Stories

### Liquidity Provision
**As a market maker, I want to provide liquidity efficiently and earn fees.**

- **Story 8.1**: Bulk Order Placement
  - **As a** market maker
  - **I want to** place multiple orders quickly
  - **So that** I can provide liquidity across price levels
  - **Acceptance Criteria**:
    - Place orders for multiple price levels at once
    - Specify spread and quantity for each level
    - Bulk cancel all orders for a market
    - Template saving for common strategies

- **Story 8.2**: Inventory Management
  - **As a** market maker
  - **I want to** track my token inventory across markets
  - **So that** I can manage my risk exposure
  - **Acceptance Criteria**:
    - Dashboard showing YES/NO token holdings per market
    - Total exposure calculations
    - Alerts when exposure exceeds limits
    - Quick rebalancing tools

- **Story 8.3**: Fee Tracking
  - **As a** market maker
  - **I want to** track fees earned from providing liquidity
  - **So that** I can measure my market making profitability
  - **Acceptance Criteria**:
    - Fees earned per market displayed
    - Daily/weekly/monthly fee summaries
    - Fee rate calculations
    - Volume-based fee estimates

### API Access
**As a market maker, I want programmatic access to trading functions.**

- **Story 9.1**: API Key Management
  - **As a** market maker
  - **I want to** generate and manage API keys
  - **So that** I can automate my trading strategies
  - **Acceptance Criteria**:
    - Generate API keys with custom permissions
    - Revoke keys when needed
    - View API usage statistics
    - Rate limiting information displayed

- **Story 9.2**: Automated Trading
  - **As a** market maker
  - **I want to** use APIs to place and manage orders
  - **So that** I can run automated market making strategies
  - **Acceptance Criteria**:
    - REST API for all trading functions
    - WebSocket API for real-time data
    - Order placement, cancellation, and modification
    - Real-time balance and position updates

---

## 👨‍💼 Platform Admin User Stories

### Market Management
**As a platform admin, I want to create and manage prediction markets.**

- **Story 10.1**: Create Market
  - **As a** platform admin
  - **I want to** create new prediction markets
  - **So that** users have interesting topics to trade on
  - **Acceptance Criteria**:
    - Form for market creation with question, description, category
    - Set end date and resolution criteria
    - Preview market before publishing
    - Draft saving functionality

- **Story 10.2**: Manage Market Status
  - **As a** platform admin
  - **I want to** pause, resume, or close markets
  - **So that** I can handle issues or end markets early
  - **Acceptance Criteria**:
    - Pause trading on specific markets
    - Resume trading with admin confirmation
    - Close markets before end date if needed
    - Notify users of status changes

- **Story 10.3**: Resolve Markets
  - **As a** platform admin
  - **I want to** resolve markets when events conclude
  - **So that** users can claim their winnings
  - **Acceptance Criteria**:
    - Mark markets as YES or NO outcome
    - Add resolution notes/evidence
    - Confirmation step before finalizing
    - Automatic payout processing after resolution

### Platform Monitoring
**As a platform admin, I want to monitor platform activity and health.**

- **Story 11.1**: Activity Dashboard
  - **As a** platform admin
  - **I want to** see platform activity metrics
  - **So that** I can monitor platform health and growth
  - **Acceptance Criteria**:
    - Daily/weekly active users
    - Trading volume statistics
    - Number of markets and trades
    - Revenue and fee collection metrics

- **Story 11.2**: User Management
  - **As a** platform admin
  - **I want to** view and manage user accounts
  - **So that** I can handle support issues and compliance
  - **Acceptance Criteria**:
    - User list with basic information
    - Search users by wallet address
    - View user trading history
    - Suspend/unsuspend accounts if needed

- **Story 11.3**: System Health Monitoring
  - **As a** platform admin
  - **I want to** monitor system performance
  - **So that** I can ensure good user experience
  - **Acceptance Criteria**:
    - Order execution time metrics
    - WebSocket connection status
    - API response time monitoring
    - Error rate tracking and alerts

---

## 🔄 Core User Flows

### Flow 1: New User Onboarding
1. User visits platform
2. Clicks "Connect Wallet"
3. Connects MetaMask wallet
4. Claims test USDC from faucet
5. Browses available markets
6. Places first trade
7. Receives order fill notification

### Flow 2: Market Discovery to Trade
1. User searches for specific topic
2. Filters results by category
3. Clicks on interesting market
4. Reviews market details and order book
5. Decides on position size and price
6. Places order
7. Monitors order status

### Flow 3: Portfolio Management
1. User checks portfolio dashboard
2. Reviews current positions
3. Sees unrealized P&L
4. Decides to take profits on one position
5. Places sell order
6. Order fills, realizes profit
7. Updates overall portfolio value

### Flow 4: Admin Market Creation
1. Admin logs into admin dashboard
2. Clicks "Create New Market"
3. Fills out market details form
4. Sets resolution criteria and end date
5. Previews market
6. Publishes market
7. Market appears on platform

### Flow 5: Market Resolution
1. Real-world event concludes
2. Admin reviews event outcome
3. Navigates to market resolution page
4. Selects correct outcome (YES/NO)
5. Adds resolution notes
6. Confirms resolution
7. Payouts automatically processed

---

## ✅ Definition of Done

For each user story to be considered complete:

1. **Functional Requirements**: All acceptance criteria met
2. **UI/UX**: Responsive design works on desktop and mobile
3. **Testing**: Unit tests and integration tests pass
4. **Performance**: Actions complete within 3 seconds
5. **Security**: Input validation and error handling implemented
6. **Documentation**: API endpoints documented (for technical features)
7. **Admin Approval**: Product owner/admin approves functionality

---

## 🚨 Out of Scope for MVP

The following are explicitly **NOT** included in MVP:
- Advanced order types (stop-loss, FOK, IOC)
- Automated market making algorithms
- Social features (comments, following)
- Mobile app
- KYC/AML compliance
- Multi-language support
- Advanced analytics and reporting
- Cross-chain functionality

---

**Created**: May 27, 2025  
**Version**: 1.0 - MVP Testnet User Stories  
**Total Stories**: 25 user stories across 4 personas