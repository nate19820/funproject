# 🌊 Marine Life Explorer - Interactive Ocean Mapping & Research Platform

An interactive, map-based educational website for tracking marine life, habitats, and ecosystems with real-time internet search integration.

## 🎯 Core Features

### Interactive Ocean Map Interface
- Global ocean map with zoomable layers
- Click-to-zoom into oceans (Pacific, Atlantic, Indian, Arctic, Southern)
- Select regions and depth zones
- Smooth transitions and animations

### Marine Life Database
- Comprehensive species database organized by region and depth
- Organism cards with images, descriptions, and key traits
- Direct links to Wikipedia and educational sources
- Expandable detail panels/modals

### Real-Time Internet Search Integration
- Dynamic search capabilities for species information
- Integration with multiple data sources:
  - Wikipedia API
  - Google Custom Search API / Bing Search API
  - GBIF (Global Biodiversity Information Facility)
  - OBIS (Ocean Biodiversity Information System)
- Cached results for improved performance
- Auto-expand knowledge toggle

### Human Impact Layer
- Toggleable visualization of environmental impacts:
  - Pollution (plastic, oil spills)
  - Overfishing
  - Climate change effects
  - Ocean acidification
  - Habitat destruction
- Visual indicators and explanations
- Species impact correlation

### Smart Data Enrichment
- Merge static database with live API data
- Fallback data support
- Performance optimization through caching and lazy loading

## 📁 Project Structure

```
├── public/
│   ├── index.html
│   ├── css/
│   │   ├── main.css
│   │   ├── map.css
│   │   ├── sidebar.css
│   │   └── modals.css
│   ├── js/
│   │   ├── app.js
│   │   ├── map.js
│   │   ├── organisms.js
│   │   ├── search.js
│   │   ├── human-impact.js
│   │   └── utils.js
│   └── assets/
│       ├── images/
│       ├── icons/
│       └── data/
│
├── backend/
│   ├── server.js
│   ├── routes/
│   │   ├── search.js
│   │   ├── organisms.js
│   │   └── impacts.js
│   ├── middleware/
│   │   ├── rateLimit.js
│   │   └── cache.js
│   ├── services/
│   │   ├── wikiService.js
│   │   ├── gbifService.js
│   │   ├── obisService.js
│   │   └── searchService.js
│   ├── data/
│   │   ├── organisms.json
│   │   ├── regions.json
│   │   └── impacts.json
│   └── .env.example
│
├── tests/
│   ├── unit/
│   ├── integration/
│   └── e2e/
│
├── docs/
│   ├── API.md
│   ├── ARCHITECTURE.md
│   └── DATA_STRUCTURE.md
│
├── .gitignore
├── package.json
├── docker-compose.yml
└── README.md
```

## 🚀 Getting Started

### Prerequisites
- Node.js 16+
- npm or yarn
- API keys for:
  - Google Custom Search API (or Bing Search)
  - GBIF and OBIS APIs (free)

### Installation

1. Clone the repository:
```bash
git clone https://github.com/nate19820/funproject.git
cd funproject
```

2. Install dependencies:
```bash
npm install
```

3. Setup environment variables:
```bash
cp backend/.env.example backend/.env
# Edit .env with your API keys
```

4. Start the development server:
```bash
npm run dev
```

5. Open browser at `http://localhost:3000`

## 🛠 Technology Stack

**Frontend:**
- HTML5 / CSS3 / JavaScript ES6+
- Mapbox GL JS or Leaflet (map visualization)
- D3.js (supplementary data visualization)
- Axios (HTTP requests)

**Backend:**
- Node.js + Express.js
- Caching layer (Redis or in-memory)
- Rate limiting
- CORS support

**APIs & Data Sources:**
- Wikipedia API
- Google Custom Search API / Bing Search
- GBIF (Global Biodiversity Information Facility)
- OBIS (Ocean Biodiversity Information System)

**DevOps:**
- Docker & Docker Compose
- Environment-based configuration

## 📊 Data Structure

See `docs/DATA_STRUCTURE.md` for detailed schema information.

Key entities:
- Organisms
- Regions
- Depth Zones
- Human Impacts
- Search Results Cache

## 🎨 UI/UX Highlights

- Ocean-themed color palette (blues, gradients)
- Smooth zoom transitions
- Responsive design (mobile + desktop)
- Sidebar with filters and search panel
- Modal/detail panels for organism info
- Loading states and error handling

## ✨ Bonus Features

- Ecosystem health indicators
- Timeline slider for ecosystem changes
- Endangered species highlighting
- AI-generated search result summaries
- Interactive learning quiz mode

## 📖 Documentation

- `docs/API.md` - API endpoint documentation
- `docs/ARCHITECTURE.md` - System architecture
- `docs/DATA_STRUCTURE.md` - Data schema details

## 🤝 Contributing

See `CONTRIBUTING.md` for guidelines.

## 📄 License

MIT License - See LICENSE file

## 🔗 Resources

- [Mapbox GL JS Docs](https://docs.mapbox.com/mapbox-gl-js/)
- [GBIF API](https://www.gbif.org/developer)
- [OBIS API](https://www.obis.org/)
- [Wikipedia API](https://www.mediawiki.org/wiki/API)

---

**Created:** 2026-04-07 14:03:24  
**Status:** In Development
