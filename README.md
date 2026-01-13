<div align="center">
  <h1>Mezon</h1>
	
---

### 🛠️ Development Setup

```bash
# Clone the repository
git clone https://github.com/mezonai/mezon.git
cd mezon

# Install dependencies
yarn install

# Available development commands
yarn dev:chat          # Start chat app (port 4200)
yarn dev:admin         # Start admin dashboard (port 4200)
yarn dev:mobile        # Start mobile development
yarn dev:desktop       # Start desktop app

# Build for production
yarn build:chat        # Build web chat app
yarn build:desktop     # Build desktop app
yarn build:mobile      # Build mobile apps

# Code quality
yarn lint              # Run linting
yarn format           # Format code
```

### 📁 Project Structure

```
mezon/
├── apps/              # Applications
│   ├── chat/          # Main web chat application
│   ├── admin/         # Admin dashboard
│   ├── desktop/       # Electron desktop app
│   ├── mobile/        # React Native mobile app
│   └── discover/      # Community discovery app
├── libs/              # Shared libraries
│   ├── components/    # Reusable UI components
│   ├── store/         # State management (Redux)
│   ├── transport/     # API & WebSocket clients
│   ├── core/          # Business logic
│   └── ui/            # Design system
└── docs/              # Documentation
```

### 🔧 Technology Stack

#### Frontend

-   **Framework**: React 18 with TypeScript
-   **State Management**: Redux Toolkit + RTK Query
-   **Styling**: Tailwind CSS
-   **Build Tool**: Nx Monorepo with Webpack
-   **Mobile**: React Native
-   **Desktop**: Electron

#### Backend & Infrastructure

-   **Core**: We built a custom server using Redis, ScyllaDB, and sockets to enable real-time communication.
-   **Mezon Mainnet**: [mmn](https://github.com/mezonai/mmn) - High-performance and zero free blockchain layer 1
-   **Real-time**: WebSocket with binary protocol
-   **Security**: E2E encryption, TLS 1.3
-   **Performance**: Sub-millisecond latency, horizontal scaling

#### Development Tools

-   **Testing**: Jest + Cypress
-   **Linting**: ESLint + Prettier
-   **CI/CD**: GitHub Actions
-   **Package Manager**: Yarn

### 📚 Getting Started

1. **Setup**: Follow the [Developer Guide](docs/developer/SETUP.md) for detailed setup instructions
2. **Architecture**: Review [Architecture docs](docs/developer/ARCHITECTURE.md) to understand the system
3. **Contribute**: Browse [open issues](https://github.com/mezonai/mezon/issues) for contribution opportunities
4. **Community**: Join our [developer community](https://mezon.ai/invite/1840696977034055680) for support and discussions

### 🔌 Extensibility

**Bot Development**

-   Build powerful bots using our official SDKs
-   Automate workflows and community management
-   Access comprehensive APIs for custom integrations

**Custom Themes**

-   Create custom themes and UI modifications
-   Brand customization for communities
-   Personalized user interfaces

**API Integration**

-   REST API and WebSocket support
-   Custom webhooks and third-party integrations
-   Extensive documentation and examples

> 🔗 **Resources**: [Bot Example](https://github.com/mezonai/mezon-bot-example) | [SDK Documentation](https://mezon.ai/docs/mezon-sdk-docs/)

## 📚 Resources & Documentation

### 🛠️ For Developers

-   [**Developer Guide**](docs/developer/SETUP.md) - Complete setup and development guide
-   [**API Documentation**](https://mezon.ai/docs/mezon-sdk-docs/) - REST API and WebSocket reference
-   [**Architecture Guide**](docs/developer/ARCHITECTURE.md) - System design and architecture
-   [**Bot Development**](https://github.com/mezonai/mezon-bot-example) - Bot creation tutorial

### 📦 SDKs & Libraries

-   [**JavaScript SDK**](https://github.com/mezonai/mezon-js) - Official JS/TS SDK
-   [**Go SDK**](https://github.com/mezonai/mezon-go-sdk) - Official Go SDK
-   [**Java SDK**](https://github.com/mezonai/mezon-java-sdk) - Official Java SDK
-   [**Python SDK**](https://github.com/phuvinh010701/mezon-sdk-python) - Official Python SDK
-   [**NestJS SDK**](https://github.com/n0xgg04/nezon) - Official NestJs SDK
-   [**Mezon WebJs SDK**](https://github.com/mezonai/mezon-web-js) - SDK for channel apps integration
-   [**MCP Integration**](https://github.com/mezonai/mezon-mcp) - AI-ready integration

---

## 🔧 Troubleshooting

### Common Issues

**Installation Problems**

-   Ensure Node.js 18+ and Yarn 1.22.4+ are installed
-   Clear node_modules and reinstall: `rm -rf node_modules && yarn install`
-   Check [system requirements](#-installation) for your platform

**Development Issues**

-   Port conflicts: Change port in project configuration
-   Build failures: Run `yarn lint` and `yarn format` to fix code issues
-   WebSocket connection issues: Check firewall and proxy settings

**Performance Issues**

-   Enable hardware acceleration in browser settings
-   Close unnecessary applications to free up system resources
-   Update to the latest version for performance improvements

> 🆘 **Need Help?** Visit our [troubleshooting guide](docs/TROUBLESHOOTING.md) or ask in our [community chat](https://mezon.ai/invite/1840696977034055680).

---

## 🙏 Acknowledgments

Mezon is built on top of amazing open-source technologies:

-   [webrtc](https://github.com/pion/webrtc) - Pion WebRTC A pure Go implementation of the WebRTC API
-   [livekit](https://livekit.io) - Livekit
-   [ScyllaDB](https://www.scylladb.com) - ScyllaDB
-   [Redis](https://redis.io) - Redis
-   [imgproxy](https://imgproxy.net) - imgproxy
-   [minio](https://min.io) - minio
-   [Ory Hydra](https://www.ory.sh/hydra) - OAuth 2.0 and OpenID Connect server
-   [Snowflake](https://github.com/bwmarrin/snowflake) - A very simple Twitter snowflake generator
-   [React](https://reactjs.org/) - UI framework
-   [Nx](https://nx.dev/) - Monorepo tooling
-   And many other fantastic open-source projects

[![MSeeP.ai Security Assessment Badge](https://mseep.net/pr/mezonai-mezon-badge.png)](https://mseep.ai/app/mezonai-mezon)
