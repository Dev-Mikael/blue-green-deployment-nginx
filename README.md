# blue-green-deployment-nginx
# Blue/Green Deployment with Nginx Auto-Failover

A Docker Compose setup demonstrating Blue/Green deployment patterns with automatic failover using Nginx upstreams.

## Features

- **Blue/Green Deployment**: Two identical Node.js services behind Nginx
- **Automatic Failover**: Nginx automatically switches to backup on primary failure
- **Zero Downtime**: Client requests are retried to backup within the same request
- **Health Monitoring**: Built-in health checks and fast failure detection
- **Header Preservation**: App headers (`X-App-Pool`, `X-Release-Id`) are forwarded to clients

## Quick Start

1. **Clone and setup**:
   ```bash
   cp .env.example .env
   # Edit .env if needed
