# Vegas Casino with Fraud Detection

This repository contains the **Vegas Casino** application specifically designed for ACE-BOX deployment. It demonstrates advanced fraud detection capabilities with comprehensive gaming analytics, real-time cheat monitoring, and business observability integration.

## 🚀 Quick Start

Deploy this application using ACE-BOX in one command:

```bash
ace enable https://github.com/lawrobar90/ace-box-ext-hot-perform-vegasapp.git
```

## 📋 What Gets Deployed

### Core Applications
- **Vegas Casino**: Multi-game casino platform with fraud detection
- **Dynatrace Integration**: OneAgent, Monaco configuration, and business events
- **Mattermost**: Team collaboration platform
- **nginx Dashboard**: ACE-BOX standard dashboard with OneAgent compatibility

### ACE-BOX Features
- ✅ **Automated Deployment**: Role-based Ansible automation
- ✅ **Kubernetes Integration**: Professional service mesh and ingress
- ✅ **OneAgent Compatible**: nginx-based dashboard eliminates Node.js conflicts
- ✅ **Monaco Configuration**: Automated Dynatrace setup via configuration as code
- ✅ **Health Monitoring**: Comprehensive health checks and auto-recovery
- ✅ **Public Access**: Properly configured ingress without authentication barriers

## 🎰 Casino Games

The Vegas Casino application includes multiple games with fraud detection:

### Available Games
- **🎰 Slot Machines**: Multi-reel slots with anomaly detection
- **🃏 Blackjack**: Classic card game with cheat pattern monitoring  
- **🎡 Roulette**: European roulette with betting pattern analysis
- **🎲 Dice Game**: Craps-style dice with outcome validation

### Fraud Detection Features
- **Silent Cheat Monitoring**: Background fraud detection without user disruption
- **Pattern Recognition**: AI-powered analysis of unusual gaming patterns
- **Lockout System**: Automatic user lockout for detected fraud
- **Comprehensive Logging**: Full audit trail of all gaming activities
- **Real-time Alerts**: Instant notifications for fraud detection events

## 🔗 Access URLs

After deployment, access your services at:

- **Dashboard**: `https://dashboard.{your-domain}/` (ACE-BOX control panel)
- **Vegas Casino**: `https://vegas.{your-domain}/` (Main casino lobby)  
- **Mattermost**: `https://mattermost.{your-domain}/` (Collaboration)
- **Dynatrace**: Your configured tenant URL

## 🎯 Gaming Features

### Casino Games
- **Slot Machines**: `/slots.html` - Multi-line slot machines with progressive jackpots
- **Blackjack**: `/blackjack.html` - Classic 21 with dealer AI
- **Roulette**: `/roulette.html` - European roulette with comprehensive betting
- **Dice Game**: `/dice.html` - Craps-style dice game with side bets

### Player Management
- **Leaderboard**: `/leaderboard.html` - Top players and high scores
- **Analytics**: `/analytics.html` - Real-time gaming analytics
- **Account Management**: Player profiles and game history

### Admin Capabilities
- Service health monitoring: `/api/admin/services/status`
- Fraud detection control: `/api/admin/lockout-user-cheat`
- Player analytics: `/api/admin/player-stats`
- System health checks: `/health`

## 🛡️ Fraud Detection System

### Cheat Detection Algorithms
- **Pattern Analysis**: Unusual win/loss patterns detection
- **Betting Anomalies**: Suspicious betting behavior identification  
- **Timing Analysis**: Game timing pattern irregularities
- **Statistical Outliers**: Win rates beyond statistical norms

### Response Mechanisms
- **Silent Monitoring**: Background fraud detection without game disruption
- **Graduated Response**: Warning → Monitoring → Lockout progression
- **Business Events**: Automatic Dynatrace business event creation
- **Audit Logging**: Comprehensive fraud detection logs

## 🛠️ Architecture

```
ACE-BOX Extension
├── ace-ext.config.yml          # Extension configuration
├── main.yml                    # Role orchestration  
└── roles/vegas-casino/         # Main deployment role
    ├── tasks/main.yml          # Deployment automation (500+ lines)
    ├── defaults/main.yml       # Default variables with fraud settings
    ├── templates/              # Kubernetes and dashboard templates
    └── files/monaco/           # Dynatrace configuration as code
```

### Deployment Flow
1. **Infrastructure Setup**: OneAgent, Kubernetes, Node.js
2. **Monaco Configuration**: Automated Dynatrace setup with fraud detection
3. **Application Deployment**: Vegas Casino with comprehensive fraud monitoring
4. **Service Mesh**: Kubernetes services, ingress, and load balancing
5. **Dashboard Deployment**: nginx-based ACE-BOX dashboard  
6. **Public Access**: Automated ingress configuration
7. **Health Verification**: End-to-end health checks

## 📊 Monitoring & Observability

### Dynatrace Integration
- **Business Events**: Automatic fraud detection event creation
- **Workflows**: Automated fraud response workflows
- **Dashboards**: Pre-configured gaming and fraud analytics dashboards
- **Service Monitoring**: Full-stack casino application performance monitoring

### Health Checks
- Application health: `GET /health`
- Admin services: `GET /api/admin/services/status`  
- Game service status: Individual game health monitoring
- Kubernetes readiness and liveness probes
- Automated restart and recovery logic

## 🔧 Configuration

### Environment Variables
- `COMPANY_NAME`: Demo company context (default: "Dynatrace")
- `COMPANY_DOMAIN`: Company domain for scenarios  
- `INDUSTRY_TYPE`: Industry context (default: "gaming")
- `ACE_BOX_ID`: Unique identifier for the ACE-BOX instance

### Fraud Detection Settings
- `ENABLE_FRAUD_DETECTION`: Enable/disable fraud monitoring (default: true)
- `CHEAT_LOCKOUT_DURATION`: User lockout duration in seconds (default: 3600)  
- `SILENT_CHEAT_MONITORING`: Background monitoring without user notification

### Monaco Configuration  
The application includes pre-configured Monaco projects:
- Fraud detection business event definitions
- Cheat lockout workflow automation
- Gaming analytics dashboard templates
- Alert policies for critical fraud detection metrics

## 🤝 Integration Points

### Dynatrace Platform
- OneAgent automatic instrumentation
- Fraud detection business event ingestion via CloudEvents format
- DQL query integration for gaming analytics
- Workflow automation for fraud response processes

### ACE-BOX Ecosystem  
- Standard role-based deployment pattern
- nginx dashboard integration with casino game links
- Kubernetes service mesh compatibility
- Public ingress configuration following ACE-BOX standards

## 🚀 Use Cases

### Fraud Detection Demos
1. **Real-time Cheat Detection**: Monitor and respond to gaming fraud
2. **Pattern Recognition**: AI-powered analysis of suspicious behavior
3. **Business Impact Analysis**: Track fraud impact on casino revenue
4. **Automated Response**: Workflow-driven fraud mitigation

### Gaming Analytics Demonstrations  
1. **Player Behavior Analytics**: Track gaming patterns and preferences
2. **Revenue Optimization**: Monitor game performance and profitability
3. **Real-time Gaming Metrics**: Live dashboard of casino operations
4. **Predictive Analytics**: AI-powered gaming trend analysis

## 📝 Requirements

- ACE-BOX environment with Kubernetes
- Dynatrace tenant with OneAgent deployment capabilities  
- Ingress controller configured (nginx recommended)
- Node.js support (automatically installed via ACE-BOX role)

## 🔄 Updates & Maintenance

The application includes:
- Automated health monitoring and restart capabilities  
- Rolling update support via Kubernetes deployments
- Configuration drift detection and correction
- Comprehensive fraud detection logging for troubleshooting

---

**Ready to demonstrate the power of Dynatrace Business Observability with Vegas Casino fraud detection and ACE-BOX professional deployment!** 🎰🛡️
