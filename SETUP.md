# 🛠️ Setup Guide - Enterprise AI Architects

Complete guide to setting up and configuring your Enterprise AI Architect team.

---

## Table of Contents

- [Prerequisites](#prerequisites)
- [Quick Setup (5 minutes)](#quick-setup-5-minutes)
- [Advanced Configuration](#advanced-configuration)
- [Agent-Specific Setup](#agent-specific-setup)
- [Verification](#verification)
- [Troubleshooting](#troubleshooting)

---

## Prerequisites

### Required
- ✅ **Nebula Account**: Sign up at [nebula.gg](https://nebula.gg) (free tier available)
- ✅ **Web Browser**: Modern browser (Chrome, Firefox, Safari, Edge)
- ✅ **Internet Connection**: Stable connection for AI consultations

### Optional (for advanced features)
- 🔧 **API Keys**: For specific integrations (GitHub, cloud providers)
- 🔧 **Connected Apps**: OAuth connections for research and data access
- 🔧 **Custom Agents**: For extending the team with your own agents

---

## Quick Setup (5 minutes)

### Step 1: Access Your Workspace

1. Log in to [nebula.gg](https://nebula.gg)
2. Navigate to your conversation interface
3. You're ready! No installation needed.

### Step 2: Verify Agent Access

Test that you can access the agents:

```
"Show me the available AI architect agents"
```

Expected response: List of 20 enterprise AI architect agents.

### Step 3: First Consultation

Try your first architecture consultation:

```
"I need help designing a RAG system for 10,000 PDFs"
```

✅ **Setup Complete!** If you received an architecture analysis, you're all set.

---

## Advanced Configuration

### Connecting External Services

Some agents can leverage connected services for enhanced capabilities:

#### GitHub Integration (Optional)
**Use Case**: Research code repositories, analyze architectures, review implementations

**Setup**:
1. In Nebula, go to Settings → Connected Apps
2. Click "Connect GitHub"
3. Authorize Nebula to access your repositories
4. Agents can now research GitHub repos when needed

**Agents That Use This**:
- AI Agent Orchestration Expert
- LangGraph StateGraph Expert
- Document Parsing Expert

#### Web Research (Enabled by Default)
**Use Case**: Latest benchmarks, pricing, best practices

All agents have web search capabilities for:
- Current technology pricing
- Latest AI model benchmarks
- Industry best practices
- Regulatory updates

**No setup required** - works out of the box.

---

### Custom Agent Configuration

#### Creating Custom Agents

You can extend this team with your own specialized agents:

```
"Create a custom agent for analyzing Kubernetes deployments"
```

The system will guide you through:
1. Defining the agent's expertise
2. Selecting tools and capabilities
3. Testing and validation

See [CONTRIBUTING.md](CONTRIBUTING.md) for details on creating custom agents.

---

## Agent-Specific Setup

### For RAG Pipeline Work

**Agent**: Advanced RAG Pipeline Architect

**Optional Enhancements**:
- Connect to your document storage (Google Drive, Dropbox)
- Provide sample documents for analysis
- Share existing architecture diagrams

**Usage**:
```
"Analyze this RAG architecture: [paste diagram or description]"
```

---

### For Security Assessments

**Agent**: Enterprise Security Architecture Specialist

**Recommended Preparation**:
- Have your compliance requirements ready (GDPR, HIPAA, SOC 2)
- List data types you'll process
- Identify regulatory jurisdictions

**Usage**:
```
"We need a HIPAA-compliant AI architecture for healthcare data"
```

---

### For Cost Optimization

**Agent**: Cost Optimization Analyst

**Helpful Information**:
- Current monthly AI spending
- Usage patterns (requests/day, avg tokens)
- Performance requirements (latency, throughput)

**Usage**:
```
"Our OpenAI costs are $30,000/month. We process 10M requests/day. 
Can you optimize this?"
```

---

### For Model Evaluation

**Agent**: AI Model Evaluation Advisor

**Preparation**:
- Define your use case clearly
- List your evaluation criteria (cost, latency, accuracy)
- Specify any constraints (data privacy, compliance)

**Usage**:
```
"Compare GPT-4, Claude Opus, and Gemini Ultra for:
- Customer service chatbot
- < 2s response time
- < $10,000/month budget
- Must support 100 languages"
```

---

## Verification

### Test Each Core Capability

Run these verification tests to ensure everything works:

#### 1. Architecture Design
```
"Design a simple RAG system architecture"
```
✅ Expected: Diagram, component descriptions, technology recommendations

#### 2. Technology Research
```
"What are the top 3 vector databases for production RAG systems?"
```
✅ Expected: Comparison table with pricing, features, pros/cons

#### 3. Cost Analysis
```
"Estimate costs for processing 1M documents with OpenAI embeddings"
```
✅ Expected: Detailed cost breakdown with calculations

#### 4. Risk Assessment
```
"What are the security risks in a multi-tenant AI system?"
```
✅ Expected: Risk matrix, severity ratings, mitigation strategies

#### 5. Implementation Planning
```
"Create a 90-day roadmap for building an enterprise RAG system"
```
✅ Expected: Phased plan with milestones, resources, dependencies

---

## Troubleshooting

### Common Issues

#### Issue: "Agent not found"
**Solution**: 
- Verify you're in the correct Nebula workspace
- Check that agents are listed in your agent directory
- Try: `"List all available agents"`

#### Issue: "Cannot access external research"
**Solution**:
- Check internet connection
- Verify web search is enabled (it should be by default)
- Some content may be behind paywalls - agents will note this

#### Issue: "Response is too generic"
**Solution**:
Provide more context:
- ❌ "Design an AI system"
- ✅ "Design an AI system for legal document analysis, handling 50,000 contracts/year, requiring < 3s response time, with SOC 2 compliance"

#### Issue: "Cost estimates seem wrong"
**Solution**:
- Agents use current public pricing - verify it's up to date
- Provide actual usage metrics for accurate estimates
- Consider that pricing changes frequently - always verify with vendors

#### Issue: "Recommendations don't match my constraints"
**Solution**:
Be explicit about constraints:
```
"Design a RAG system with these hard constraints:
- MUST use AWS only (no other clouds)
- MUST be < $10,000/month
- MUST support air-gapped deployment
- MUST comply with ITAR"
```

---

### Performance Optimization

#### For Faster Responses
1. **Be specific**: Narrow questions get faster, more precise answers
2. **Provide context upfront**: Don't make the agent ask for basic info
3. **Use focused agents**: Go directly to the specialist (see [Capability Matrix](docs/Agent_Capability_Matrix.md))

#### For Better Results
1. **Share examples**: "Like this: [example], but for my use case"
2. **Iterate**: Start broad, then drill down with follow-ups
3. **Validate**: Ask agent to verify assumptions and calculations

---

## Advanced Features

### Multi-Agent Workflows

Combine multiple agents for comprehensive analysis:

```
"I need a complete AI platform design:
1. Architecture (Enterprise AI Architect Director)
2. Security assessment (Security Architecture Specialist)  
3. Cost analysis (Cost Optimization Analyst)
4. Implementation plan (AI Agent Orchestration Expert)"
```

The system will coordinate multiple agents automatically.

---

### Delegation Patterns

For complex projects, agents can delegate to specialists:

```
"Design an enterprise AI platform with RAG, agent orchestration, 
and multi-tenant security. Provide complete architecture, 
implementation plan, and risk analysis."
```

The lead agent will:
1. Decompose the problem
2. Delegate to specialists
3. Synthesize results
4. Deliver unified plan

---

### Integration with FDE Super Team

For implementation and deployment:

1. **Design Phase**: Use AI Architects for architecture and planning
2. **Execution Phase**: Hand off to [FDE Super Team](https://github.com/glen200392/fde-super-team) for implementation
3. **Feedback Loop**: FDE insights improve AI Architects' recommendations

See [RELATED_PROJECTS.md](RELATED_PROJECTS.md) for integration patterns.

---

## Configuration Files

### Agent Preferences (Optional)

You can save preferences for repeated use:

**Example**: Cost-Conscious Mode
```
"For all future architecture recommendations:
- Prioritize cost over performance (unless specified)
- Prefer open-source solutions
- Include self-hosted options
- Target budget: < $5,000/month"
```

**Example**: Enterprise Mode
```
"For all future recommendations:
- Prioritize reliability and security
- Require SOC 2 / ISO 27001 compliance
- Enterprise SLA requirements
- Multi-region deployment"
```

---

## Next Steps

✅ **You're all set!** Here's what to do next:

1. **📖 Quick Start**: Try the [5-minute tutorial](QUICKSTART.md)
2. **📚 Examples**: See [real-world use cases](EXAMPLES.md)
3. **🔍 Explore Agents**: Browse the [Capability Matrix](docs/Agent_Capability_Matrix.md)
4. **🚀 Deploy**: Read the [Deployment Guide](DEPLOYMENT_GUIDE.md)

---

## Getting Help

- **📖 Documentation**: Check [docs/](docs/) for detailed guides
- **💬 Community**: Join [Discussions](../../discussions)
- **🐛 Issues**: Report problems in [Issues](../../issues)
- **🎓 Examples**: Learn from [EXAMPLES.md](EXAMPLES.md)

---

## Updates and Maintenance

### Staying Current

The AI Architect team is regularly updated with:
- New agents for emerging technologies
- Updated pricing and benchmarks
- Latest best practices
- New integration capabilities

**Check for updates**: Watch this repository for releases and announcements.

---

**Setup complete!** 🎉 Start your first consultation in [QUICKSTART.md](QUICKSTART.md)
