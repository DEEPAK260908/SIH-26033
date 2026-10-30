# Smart India Hackathon Workshop
# Date:30/10/26
## Reference Number:26005420
## Name: DEEPAK N 

## Problem Title
SIH 26033: Multiple intermediaries reduce farmers earnings and increase consumer prices.

## Problem Creater's Organization
Ministry of Consumer Affairs, Food & Public Distribution

## Theme
Agriculture, FoodTech & Rural Development

## Problem Description
Expected Solution: Create a digital marketplace that:

• Connects farmers/FPOs directly with consumers and bulk buyers.
• Provides logistics support.
• Uses AI for demand forecasting and route optimization.

Benefits:

• Better prices for farmers.
• Lower prices for consumers.
• Reduced supply chain inefficiencies.

## Proposed Solution

Detailed explanation

Mobile-first (Android + web) marketplace connecting farmers/FPOs directly with consumers and bulk buyers
Marketplace: produce listing, orders, bulk requirements, UPI payments with escrow-style release after delivery
Logistics: village collection → FPO hub → city hub → buyer, with pooled loads and consignment tracking
Intelligence: AI for demand forecasting, price suggestions, harvest timing and route optimization

How it addresses the problem

Direct listing removes intermediary layers, leaving only a small transparent platform fee
Live mandi prices plus AI price suggestions in local languages
Harvest against confirmed orders reduces spoilage
FPOs aggregate small lots into bulk-grade supply
Load pooling and route optimization cut logistics cost
Price breakup shows the farmer’s share to consumers

Innovation and uniqueness

Demand-first harvesting (forecasts and pre-orders before harvest)
Transparent price breakup on every order
Pooled logistics for small farmers
Voice-first vernacular interface with IVR/WhatsApp fallback
Government dashboard for monitoring price spreads and supply gaps
FPOs as aggregation and quality-control nodes

## Technical Approach
Technologies

App: Flutter (offline-capable, multilingual)
Web/admin: React.js
Backend: Python (FastAPI) or Node.js
Database: PostgreSQL + PostGIS, Redis
AI/ML: scikit-learn, XGBoost, Prophet/LSTM
Routing: Google OR-Tools + OpenStreetMap/Maps API
Voice/language: Bhashini APIs
Payments: UPI with escrow-style settlement
Identity: Aadhaar eKYC, AgriStack registry
Alerts: SMS, WhatsApp Business API, push
Cloud: AWS/Azure/MeghRaj, Docker + Kubernetes
Optional: IoT temperature/humidity sensors for cold chain

Methodology

Farmer/FPO lists produce (photo, quantity, voice option)
AI suggests price and best sale window
Buyers place individual or pooled orders
System clusters orders and plans routes
Produce is collected, graded at the FPO hub, dispatched
Buyer confirms delivery, payment is released
Ratings and data feed back into the models

Flow chart:

<img width="1220" height="1127" alt="WhatsApp Image 2026-10-30 at 10 12 57 AM" src="https://github.com/user-attachments/assets/887aa090-3513-494b-b914-5628e0485a63" />

Prototype:

<img width="576" height="1280" alt="image" src="https://github.com/user-attachments/assets/364f4d9b-de1e-4453-9844-f1a1e62fbd7d" />

<img width="576" height="1280" alt="image" src="https://github.com/user-attachments/assets/1e89eac6-f98d-4c7e-b113-56bba05d0604" />

<img width="576" height="1280" alt="image" src="https://github.com/user-attachments/assets/e3981615-128d-407a-9649-54d1099d20ce" />

## Feasibility and Viability

Feasibility

Technical: all components use mature tools
Operational: existing FPOs serve as aggregation points
Economic: about 2–4% commission, logistics margin, premium analytics
Policy: fits e-NAM, ONDC, AgriStack, Digital India, FPO scheme

Challenges and risks

Low digital literacy and poor connectivity
Trust, since farmers are used to cash and trader credit
Cold-chain and logistics gaps
Quality disputes
Cold start (buyers vs farmers)
Trader resistance
Price and weather volatility affecting forecasts

Strategies

Voice-first UI, regional languages, offline mode, FPO “Kisan Mitra” agents
Escrow with 24–48 hr settlement, ratings, FPO guarantees
Partner with existing transporters, shared cold storage at hubs
Hub grading with photo evidence and a clear return policy
Start with one crop cluster and one city, onboard institutional buyers first
Give traders roles as licensed aggregators or logistics partners
Ensemble models with confidence ranges, retrained on live data

## Impact and Benefits

 Impact on target audience

Farmers/FPOs: higher price, faster payment, wider market, crop planning data
Consumers: fresher, cheaper produce with origin transparency
Bulk buyers: reliable supply and consistent quality
Ministry: real-time price, supply gap and spread visibility

Benefits

Economic: higher farmer income, lower consumer prices, less wastage
Social: empowers small farmers, digital financial inclusion, rural jobs
Environmental: less food waste, lower fuel use and emissions
Systemic: data-driven planning to reduce boom-bust price cycles (tomato, onion)

## Research and References

Research and References
e-NAM: enam.gov.in
Agmarknet: agmarknet.gov.in
ONDC: ondc.org
AgriStack: agristack.gov.in
Dept. of Consumer Affairs: consumeraffairs.gov.in
SFAC (FPO scheme): sfacindia.com
Bhashini: bhashini.gov.in
Google OR-Tools: developers.google.com/optimization
Farmer’s share studies (tomato, onion, potato) and ICAR-CIPHET post-harvest loss study: look up and cite exact figures
Comparable platforms: DeHaat, Ninjacart, AgroStar, Kisan Rath
