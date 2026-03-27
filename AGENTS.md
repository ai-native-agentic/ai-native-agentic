# AGENTS.md — ai-native-agentic

**Branch**: main  
**Commit**: 546b68b  
**Generated**: 2026-03-28 (Autonomous documentation check & update)

## OVERVIEW

Ecosystem documentation hub for the ai-native-agentic organization. Contains org-level planning docs, architecture overviews, integration roadmaps, and validation reports. This is a lightweight docs-only repo (smallest in the org). The README.md serves as the central inventory of all 12 repositories across 5 tiers (Personal AI Assistants, Research Labs, Frameworks, Development Tools, and this Documentation tier).

## STRUCTURE

```
ai-native-agentic/
├── README.md                        # Central ecosystem inventory (465 lines)
├── .github/
│   ├── workflows/
│   │   └── test-all.yml             # Unified test suite CI
│   └── badges/
│       └── README.md                # Project badge references
└── (other docs as needed)
```

## WHERE TO LOOK

| Task | Path | Notes |
|------|------|-------|
| Ecosystem overview | README.md lines 1-68 | Mission, CI status, founder, scale (12 repos, ~1.13M+ Python LOC) |
| 5-tier architecture | README.md lines 30-66 | Mermaid diagram + tier breakdown |
| Repository inventory | README.md lines 70-203 | Tier 1 (4 assistants), Tier 2 (5 labs), Tier 3 (2 frameworks), Tier 4 (1 tool) |
| Dependency graph | README.md lines 205-224 | Strong coupling (ClawWork → Nanobot), weak coupling, independent repos |
| Core technical patterns | README.md lines 226-253 | Multi-channel messaging, multi-LLM provider, container isolation, quality measurement, economic value tracking |
| Integration opportunities | README.md lines 255-299 | 7 integration projects (shared quality library, economic tracking SDK, channel abstraction, etc.) |
| Maturity assessment | README.md lines 301-323 | Production-ready (4), near-production (2), research stage (3), early development (3) |
| 2026 AI trends | README.md lines 325-353 | On-device first, self-driven exploration, production observability, dynamic memory, economic value metrics |
| Technology stack clusters | README.md lines 355-373 | TypeScript (2), Python (7), Elixir (1), Shell (2) |
| Quick start | README.md lines 375-414 | Clone all repos, try nanobot, configure NotebookLM MCP |
| Contributing | README.md lines 416-425 | Test coverage (70% min), logging (get_logger), 6-Gate compliance, no cross-imports |
| Strategic vision | README.md lines 443-459 | Short-term (3 months), mid-term (6 months), long-term (12 months) |

## CONVENTIONS

**Documentation style**:
- Markdown only (no code)
- Central inventory in README.md
- Mermaid diagrams for architecture
- Badge references in .github/badges/README.md
- CI status at top of README.md

**Cross-repo references**:
- Link to individual repo READMEs for detailed docs
- Link to AGENTS.md in each repo for contribution guidelines
- Link to VALIDATION_STATUS.md in each repo for deployment readiness

**Org-level patterns**:
- Test coverage: 70% minimum, 80% for new experiments
- Logging: `get_logger(__name__)`, never `print()`
- 6-Gate compliance: All PRs must pass harness-engineering gates
- No cross-imports: Except ClawWork → Nanobot, keep repos independent

## ANTI-PATTERNS

| Forbidden | Why |
|-----------|-----|
| Code in this repo | This is docs-only (smallest in org) |
| Duplicating repo-specific docs | Link to individual repo READMEs instead |
| Outdated inventory | README.md must reflect current state of all 12 repos |
| Missing CI status | Badge at top of README.md is required |
| Generic descriptions | Each repo entry must have specific tech stack and features |
| Ignoring maturity assessment | Production-ready vs research stage matters for users |

## COMMANDS

```bash
# Clone all repositories
cd ~/projects/ai-native-agentic
gh repo clone ai-native-agentic/openclaw
gh repo clone ai-native-agentic/nanoclaw
gh repo clone ai-native-agentic/nanobot
gh repo clone ai-native-agentic/seedbot
gh repo clone ai-native-agentic/ClawWork
gh repo clone ai-native-agentic/openmanus
gh repo clone ai-native-agentic/symphony
gh repo clone ai-native-agentic/harness-engineering
gh repo clone ai-native-agentic/lunark-chatbot-lab
gh repo clone ai-native-agentic/ai-native-self-learning-agents
gh repo clone ai-native-agentic/lunark-ondevice-ai-lab
gh repo clone ai-native-agentic/trpg-chatbot-lab

# Try nanobot (fastest path)
cd nanobot
pip install -e .
export ANTHROPIC_API_KEY="your-key-here"
nanobot agent -m "Hello from ai-native-agentic!"

# Configure NotebookLM MCP (optional)
uv tool install notebooklm-mcp-cli
export PATH="$HOME/.local/bin:$PATH"
nlm login
nanobot agent -m "내 NotebookLM 노트북 목록 보여줘"
```

## NOTES

- **Docs-only repo**: Smallest in the org (no code, just Markdown)
- **Central inventory**: README.md is the single source of truth for all 12 repos
- **5-tier architecture**: Personal AI Assistants (4), Research Labs (5), Frameworks (2), Development Tools (1), Documentation (this repo)
- **Scale**: 12 repositories, ~1,130,000+ Python LOC, 430K+ TypeScript LOC
- **Founded**: December 19, 2025 by JungSu Kim (@zzragida, NHN, South Korea)
- **CI status**: Unified test suite badge at top of README.md
- **Dependency graph**: Only 1 direct cross-repo import (ClawWork → Nanobot)
- **Maturity levels**: Production-ready (4), near-production (2), research stage (3), early development (3)
- **Integration opportunities**: 7 projects (shared quality library, economic tracking SDK, channel abstraction, cross-repo evaluation, harness for all agents, self-learning from economic feedback, multi-agent orchestra)
- **2026 AI trends**: On-device first (<20ms latency), self-driven exploration (intrinsic motivation), production observability (Lunary.ai pattern), dynamic memory (agents build knowledge graphs), economic value metrics (AI capability = economic output)
- **Technology clusters**: TypeScript (openclaw, nanoclaw), Python (nanobot, ClawWork, 5 labs, openmanus), Elixir (symphony), Shell (harness-engineering, seedbot)
- **Strategic vision**: Short-term (shared libraries, 6-Gate QA, production-grade nanoclaw/ClawWork SDK), mid-term (self-learning with economic feedback, multi-agent orchestra, production observability), long-term (on-device <20ms, unified assistant, open-source commercial platform)
- **Contributing**: 70% test coverage minimum, logging via get_logger, 6-Gate compliance, no cross-imports except ClawWork → Nanobot
- **Badge references**: .github/badges/README.md contains project badge references
- **Validation reports**: Link to documentation repo for VALIDATION_REPORT.md and INTEGRATION_ROADMAP.md
- **Quick start**: Clone all repos, try nanobot (fastest path), configure NotebookLM MCP (optional)
