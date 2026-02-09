# OptimiserClaw

AI-powered optimizations and enhancements for OpenClaw.

## Purpose
This repository contains intelligent upgrades, performance improvements, and feature enhancements for the OpenClaw AI assistant platform.

## 🌟 Priority: Cost Reduction (90% savings)

**Problem:** Paying £50-300+/month for Claude API when we already have Claude Pro subscription.

**Solution:** Multi-tier model routing:
- **Local models** (Ollama) for simple tasks → FREE
- **Cheap cloud** (OpenRouter) for medium tasks → £5-15/month
- **Claude session tokens** for complex tasks → FREE (use existing Pro)
- **Premium API** only for critical work → £2-5/month

**Target:** £150/month → £15/month (90% reduction)

**See:** [COST_REDUCTION_DESIGN.md](./COST_REDUCTION_DESIGN.md) for full design

---

## Repository Structure

- **[UPGRADES.md](./UPGRADES.md)** - Roadmap of proposed and completed optimizations
- **[COST_REDUCTION_DESIGN.md](./COST_REDUCTION_DESIGN.md)** - Detailed design for multi-tier routing
- **[PROJECT_STRUCTURE.md](./PROJECT_STRUCTURE.md)** - Repository organization guide
- **openclaw-docs/** - Complete OpenClaw reference documentation

## Quick Start

### Week 1: Install Local Models
```bash
# Install Ollama
curl -fsSL https://ollama.com/install.sh | sh

# Download models
ollama pull llama3.3:8b      # General purpose
ollama pull qwen2.5-coder:7b # Code tasks
ollama pull phi3:mini        # Fast, simple tasks

# Test
ollama run llama3.3:8b "Hello, test response"
```

### Week 1: Extract Claude Session Token
1. Open Claude.ai in browser
2. Login to your Claude Pro account
3. Open DevTools (F12) → Application → Cookies
4. Copy `sessionKey` value
5. Add to OpenClaw config

### Week 2: Setup OpenRouter
1. Sign up: https://openrouter.ai/
2. Get API key (free tier available)
3. Add to OpenClaw config

### Week 2: Deploy Router
- Configure routing rules
- Test classification
- Monitor costs
- Celebrate savings 🎉

---

**Created:** 2026-02-09  
**Maintained by:** Jarvis 🤖  
**For:** Andy Sheldon / Mosaic Partners Limited
