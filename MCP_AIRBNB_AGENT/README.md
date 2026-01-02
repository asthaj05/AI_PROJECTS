## 🌍 MCP Travel Planner Agent Team

A sophisticated Streamlit-based AI travel planning application that creates extremely detailed, personalized travel itineraries using multiple MCP servers and Google Maps integration. The app uses Airbnb MCP for real accommodation data and a custom Google Maps MCP for precise distance calculations and location services.

## ✨ Features

### 🤖 AI-Powered Travel Planning
- **Extremely Detailed Itineraries**: Creates comprehensive day-by-day schedules with specific timing, addresses, and costs
- **Distance Calculations**: Uses Google Maps MCP to calculate precise distances and travel times between all locations
- **Real-Time Accommodation Data**: Integrates with Airbnb MCP for current pricing and availability
- **Personalized Recommendations**: Customizes itineraries based on user preferences and budget constraints

### 🏨 Airbnb MCP Integration
- **Real accommodation listings** with current pricing and availability
- **Property details** including amenities, guest reviews, and booking availability
- **Budget-conscious recommendations** filtered by location and preferences
- **Direct booking information** with real-time rates

### 🗺️ Google Maps MCP Integration
- **Precise distance calculations** between all locations in the itinerary
- **Travel time estimates** for transportation planning
- **Location services** for points of interest and navigation
- **Address verification** for all recommended places
- **Transportation optimization** with turn-by-turn guidance

### 🔍 Google Search Integration
- **Current weather forecasts** with detailed clothing recommendations
- **Restaurant research** with specific addresses, price ranges, and reviews
- **Attraction details** including opening hours, ticket prices, and best visiting times
- **Local insights** and cultural information
- **Practical travel tips** including currency exchange and safety information

### 📅 Additional Features
- **Calendar Export**: Download your itinerary as a .ics file for Google Calendar, Apple Calendar, or Outlook
- **Comprehensive Cost Breakdown**: Detailed budget analysis for all trip components
- **Buffer Time Planning**: Includes travel time and unexpected delays in scheduling
- **Multiple Accommodation Options**: Provides 3 accommodation choices with distances from city center


## Setup

### Requirements

1. **Python 3.8+**: Ensure you have Python 3.8 or higher installed.

2. **MCP Servers**: The app automatically connects to:
    - **Airbnb MCP Server**: Provides real Airbnb listings and pricing data
    - **Custom Google Maps MCP**: Enables precise distance calculations and location services

### Installation

1. Clone this repository:
   ```bash
   git clone https://github.com/asthaj05/AI_PROJECTS.git
   cd AI_PROJECTS/MCP_AIRBNB_AGENT
   ```

2. Install the required Python packages:
   ```bash
   pip install -r requirements.txt
   ```

### Running the App

1. Start the Streamlit app:
   ```bash
   streamlit run app.py
   ```

2. In the app interface:
   - Specify your destination, trip duration, budget, and preferences
   - Click "🎯 Generate Itinerary" to create your detailed travel plan

3. **Optional**: Download your itinerary as a calendar file (.ics) for import into Google Calendar, Apple Calendar, or Outlook

## Troubleshooting

### Common Issues & Solutions

- **Missing distance information**: Google Maps MCP connection issue
  - Check your Google Maps API key validity
  - Ensure your API key has the necessary permissions for Maps API
  - Try refreshing the page and entering the keys again

- **Slow response times**: MCP servers can take time to respond
  - The app has a 60-second timeout configured
  - Wait for the process to complete - detailed itineraries take time to generate

### Tool Status

The app will show you which data sources were successfully used:
- 📝 **"Used general knowledge for accommodation suggestions"** = Airbnb MCP failed, using general knowledge as fallback

**The app is designed to work reliably!** Even if MCP connections fail, it will generate comprehensive itineraries using available tools and information.

## Project Structure

```
├── app.py              # Main Streamlit application with MCP integration
├── requirements.txt    # Python dependencies
└── README.md          # This documentation
```

## How It Works

The AI Travel Planner Agent Team uses a sophisticated multi-step process to create extremely detailed travel itineraries:

### 🤖 AI Agent Architecture
- User inputs trip details
- AI Agent activates MCP tools
- Google Maps MCP calculates distances
- Airbnb MCP fetches accommodations
- Web tools gather live information
- Agent composes a complete itinerary in one response
- Optional .ics calendar export generated

### 🚀 Why This Project Is Different

✔ Fully open-source
✔ No API key friction
✔ Production-ready
✔ Real-time MCP data
✔ Designed for extensibility
