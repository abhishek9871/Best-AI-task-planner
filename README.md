# Best AI Task Planner - Free LLM Edition MCP Server

![License](https://img.shields.io/badge/license-MIT-blue.svg)
![Version](https://img.shields.io/badge/version-1.0.0-green.svg)
![Build](https://img.shields.io/badge/build-passing-success.svg)

## Introduction

**Problem:** Advanced AI task planning capabilities in code editors typically rely on expensive AI API calls, creating a cost barrier for many developers. Most MCP server implementations require paid models like Claude or GPT-4, leading to significant expenses during development.

**Solution:** This repository provides a **ready-to-use, verified, and pre-configured MCP server** for AI-powered task planning that leverages **free LLM tiers** via OpenRouter (e.g., `qwen/qwen3-30b-a3b:free`) or Google AI's free offerings. It enables AI Code Editors (like Cursor, Augment Code, etc.) to automate feature planning, task execution, and code review without the high API costs of alternatives.

**Key Benefits:**
- **Cost-Effective:** Utilizes free LLM tiers, eliminating expensive API costs
- **Production-Ready:** Includes verified working configuration and necessary build fixes
- **Editor Integration:** Compatible with major AI Code Editors supporting the MCP protocol
- **Complete Solution:** Includes both backend server and Svelte UI task viewer
- **Verified Working:** All dependencies updated and build process confirmed

## Key Features

### Core MCP Protocol Implementation
- **AI Feature Planning** (`plan_feature`): Break down complex features into clear, actionable tasks
- **Task Management Loop** (`get_next_task`, `mark_task_complete`): Automated sequential execution of planned tasks
- **Code Review Assistance** (`review_changes`): AI-powered code review capabilities
- **Svelte UI Task Viewer**: Visual interface for monitoring task progress and planning details

### LLM Integration
- **OpenRouter Free Tier Support**: Pre-configured for models like `qwen/qwen3-30b-a3b:free`
- **Google AI Free Tier Compatibility**: Alternative integration with Google's free AI offerings
- **Flexible Configuration**: Easy switching between providers and models

### Technical Improvements
- **Updated Dependencies**: Ensures compatibility with latest frameworks
- **Svelte 5 Compatible**: Frontend dependencies updated (including `bits-ui@latest`)
- **Cross-Platform Support**: Working build process (with documented Windows-specific steps)

## Technology Stack

- **Backend**: Node.js, TypeScript, Express, WebSocket
- **Frontend**: SvelteKit
- **LLM Integration**: OpenRouter API / Google AI API
- **Build Tools**: TypeScript compiler, Vite
- **Protocol**: MCP (Machine Coding Protocol)

## Status & Fixes

This repository represents a stable, working version with several critical improvements over common forks:

- ✅ **Updated Frontend Dependencies**: Resolved issues with `bits-ui` for Svelte 5 compatibility
- ✅ **Verified Build Process**: Tested and working build configuration
- ✅ **Cross-Platform Compatibility**: Documented necessary manual steps for Windows deployment
  - File copying requirements (`frontend/build/*` → `dist/frontend-ui/`)
  - Schema placement (`src/config/schema.sql` → `dist/config/`)
- ✅ **Pre-Configured for Free LLMs**: Ready to use with free tier models

These fixes ensure that you can deploy a fully functional MCP server without encountering common build errors or compatibility issues that exist in other versions.

## Getting Started (High-Level)

**Important:** This repository contains the working code. For the **complete, foolproof, step-by-step guide** covering prerequisites, installation, build fixes, MCP configuration for various editors (including direct JSON edits), API key setup, custom mode instructions, detailed usage, and troubleshooting, please refer to the **Best AI Task Planner Setup Guide** available here:

[Get the Full Setup Guide Here!](YOUR_GUMROAD_OR_LEMONSQUEEZY_LINK_HERE)

The comprehensive guide covers:

1. **Environment Setup**: Node.js, npm configuration, and prerequisites
2. **Repository Installation**: Cloning and dependency installation
3. **Building the Project**: Step-by-step build instructions with Windows-specific workarounds
4. **MCP Configuration**: Detailed editor integration for Cursor, Augment Code, and others
5. **API Setup**: Obtaining and configuring OpenRouter/Google AI API keys
6. **Custom Instructions**: Optimizing the planning capabilities for your specific needs
7. **Troubleshooting**: Solutions to common issues and edge cases
8. **Advanced Usage**: Leveraging the full potential of the AI task planner

## Disclaimer

This software is provided as-is. Usage is subject to the terms and conditions of the LLM providers (OpenRouter, Google AI, etc.). While this repository contains the working code, the comprehensive Setup Guide contains essential details for correct operation, configuration, and optimization of the MCP server. The repository maintainers are not responsible for any API costs incurred through misconfiguration or changes to provider terms.

---

© 2025 Best AI Task Planner. All Rights Reserved.
