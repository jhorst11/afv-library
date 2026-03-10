# Native Mobile Rental Tenant App

A sample Custom Agentic Mobile App (CAMA) for property managers and tenants. Use this as a starting point for building native mobile apps with Salesforce Mobile Publisher, MCF (Mobile Component Framework), and SharedUI.

## Overview

This sample demonstrates a rental tenant experience—browse properties, submit maintenance requests, pay rent, and communicate with property management—all from a native iOS or Android app.

## Prerequisites

- Node.js 20+
- Salesforce CLI (`sf`)
- Xcode (iOS) or Android Studio (Android)
- A Salesforce org with Mobile Publisher enabled

## Getting Started

1. **Authorize your org**
   ```bash
   sf org login web
   sf config set target-org <your-org-alias>
   ```

2. **Create a scratch org** (optional, for development)
   ```bash
   sf org create scratch -f config/project-scratch-def.json -a rental-tenant-dev
   sf config set target-org rental-tenant-dev
   ```

3. **Deploy metadata**
   ```bash
   sf project deploy start
   ```

4. **Open in Mobile Publisher** or your preferred mobile development environment to build the native app shell.

## Project Structure

```
force-app/
└── main/
    └── default/
        ├── aura/          # Aura components (if needed)
        └── lwc/           # Lightning Web Components for MCF
```

## Next Steps

- Add MCF components for property listings, maintenance requests, and payments
- Configure Mobile Publisher app settings
- Customize the SharedUI theme for your brand
- Deploy to App Store / Play Store via Mobile Publisher

## Resources

- [Custom Agentic Mobile Apps (CAMA)](https://developer.salesforce.com/docs/atlas.en-us.mobile_publisher.meta/mobile_publisher/)
- [Mobile Component Framework (MCF)](https://developer.salesforce.com/docs/atlas.en-us.mobile_publisher.meta/mobile_publisher/)
- [Agentforce Vibes](https://github.com/forcedotcom/afv-library)
