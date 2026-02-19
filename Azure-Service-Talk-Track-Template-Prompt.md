# Azure Service Talk Track Development Prompt Template

**This is the prompt to submit to your AI assistant.** For usage guidance and customization examples, see [README.md](README.md).

---

## The Prompt Template

```
I need help developing a comprehensive customer talk track and demonstration script 
for [AZURE_SERVICE_NAME].

**CORE INPUTS** (all you need to provide):
- **Service**: [AZURE_SERVICE_NAME] (e.g., "Azure API Management", "Azure Cosmos DB")
- **Demo Repository**: [GITHUB_REPO_URL] (e.g., https://github.com/user/azure-service-demo)
- **Audience**: [AUDIENCE_DESCRIPTION] (e.g., "enterprise architects evaluating platform strategy")
- **Duration**: [PRESENTATION_LENGTH] (e.g., "60 minutes")
- **Additional Context** (optional): [ANY SPECIFIC CUSTOMER CONCERNS, INDUSTRY FOCUS, OR ARCHITECTURAL CONTEXT]

**IMPORTANT**: Use the Azure Learn MCP server to:
1. Fetch official Azure service documentation for [AZURE_SERVICE_NAME]
2. Retrieve README from the GitHub repository: [GITHUB_REPO_URL]
3. Discover best practices, architectural patterns, and integration guidance
4. Gather current pricing and SKU information
5. Find competitive positioning and use case examples

You should NOT require me to provide documentation links — discover them via MCP server.

---

## AUTO-DISCOVERY: WHAT THE AI WILL DO

Before generating the talk track, the AI will:

✅ **Repository Analysis**: Read the README to understand the demo topology and architecture
✅ **Service Documentation**: Query Azure Learn for complete service information
✅ **Capabilities Mapping**: Identify service features, tiers, and SKUs
✅ **Integration Discovery**: Find complementary Azure services that integrate
✅ **Best Practices Gathering**: Retrieve official best practices and guidance
✅ **Pricing Research**: Gather current pricing models and cost considerations
✅ **Competitive Analysis**: Research competitive positioning

---

## TALK TRACK STRUCTURE

Please develop a comprehensive talk track with the following sections:

### 1. Introduction (5 minutes)
- Hook: Why [SERVICE] matters for [AUDIENCE]
- Problem statement: What business challenge does it solve?
- Brief overview of what will be covered

### 2. Strategic Context (5 minutes)
- How [SERVICE] fits into [ARCHITECTURE_CONTEXT]
- Why it's important for enterprise organizations
- Alignment with [ENTERPRISE_FRAMEWORK] principles

### 3. Core Capabilities Deep Dive (12-15 minutes)
- 3-5 major capabilities/features (expand each in detail):
  - For each capability: What it does, why it matters, real-world scenarios
  - Include any SKU/tier differentiation (if applicable)
  - Explain integration with complementary Azure services
  - Competitive differentiation for each capability

### 4. Live Demo Walkthrough (15-20 minutes)
- Step-by-step guidance for demonstrating the service
- Using [DEMO_ENVIRONMENT] or [REFERENCE_ARCHITECTURE]
- Include specific actions in Azure Portal
- PowerShell/CLI commands where applicable
- Key talking points at each stage
- Success criteria (what to show to prove value)

### 5. Advanced Features & Considerations (5 minutes)
- Premium/advanced tiers or configuration options
- Security and compliance features
- Operational excellence capabilities
- Scalability and performance characteristics

### 6. Cost Optimization & ROI (3-5 minutes)
- Pricing model explanation
- Cost optimization strategies
- Comparison to alternative approaches
- Break-even analysis if applicable

### 7. Best Practices & Implementation Strategy (5 minutes)
- Design best practices
- Security best practices
- Operational best practices
- Phased deployment/adoption approach

### 8. Integration with Broader Azure Ecosystem (3-5 minutes)
- Key services that work with [SERVICE]
- How it fits into customer's existing architecture
- Governance and policy integration

### 9. Customer Success Stories / Use Cases (2-3 minutes)
- 2-3 realistic scenarios where [SERVICE] solved a problem
- Measurable outcomes
- Applicable to [AUDIENCE] vertical

### 10. Objection Handling & Q&A (3-5 minutes)
- 5-10 common objections and responses
- Frequently asked questions
- Links to resources for deeper learning

### 11. Closing & Next Steps (3-5 minutes)
- Summary of key value propositions
- Recommended next actions (immediate, short-term, long-term)
- Resources (documentation, support, FastTrack)
- Contact information for follow-up

---

## CONTENT GUIDELINES

### For Each Capability Section:
- **Explain the "What"**: What does this capability do?
- **Explain the "Why"**: Why does your customer need it?
- **Explain the "How"**: How do you configure/use it?
- **Demonstrate the Value**: What's the business outcome?
- **Provide Talking Points**: Include several 1-2 sentence statements that emphasize value

### For Demo Sections:
- Include specific Azure Portal navigation paths
- Provide actual PowerShell/CLI commands (not pseudocode)
- Mention what to look for (success indicators)
- Include troubleshooting tips if demo might fail
- Provide backup screenshots/documentation

### For Each Section:
- Include estimated timing
- Provide "talking point" statements (quotable, concise)
- Note where to pause for questions
- Suggest transitions between sections

---

## ADDITIONAL DELIVERABLES

Please also include:

1. **Competitive Comparison Table** (if applicable):
   - [SERVICE] vs. [COMPETITOR_A] vs. [COMPETITOR_B]
   - Feature comparison matrix
   - When to choose each option

2. **Cost Calculator**:
   - Typical monthly cost for different scenarios
   - ROI calculation for moving from alternative approaches

3. **Objection Handling Guide** (Appendix):
   - 5-10 common objections with prepared responses

4. **Demo Preparation Checklist**:
   - Pre-demo setup steps
   - Verification/testing before presenting
   - Common failure points and workarounds

5. **Quick Reference Cards** (Optional):
   - One-page summary of key capabilities
   - Common PowerShell/CLI commands
   - Pricing summary

---

## TONE & STYLE

- **Approach**: Consultative, not sales-y
- **Audience Level**: Technical decision-makers (understand cloud concepts)
- **Emphasis**: Business outcomes + technical depth
- **Language**: Clear jargon (assume customer knows Azure basics, explain domain-specific concepts)
- **Format**: Markdown with clear section breaks, code blocks, and talking points
- **Length**: Comprehensive (allow 2,000+ words) but scannable (use headers, bullets, tables)

---

## FINAL REQUEST

After generating the talk track, please:

1. Format as comprehensive Markdown document
2. Include timing estimates for each section
3. Add [TALKING POINTS] in quotes for me to use verbatim
4. Suggest where to pause for audience questions
5. Provide a demo preparation checklist
6. Include common Q&A with prepared answers

---

## REQUIRED INSTRUCTIONS FOR THE AI

⚠️ **These instructions are for the AI assistant—user should NOT manually provide documentation**

**Step 1: Fetch GitHub Repository**
- Retrieve the README.md from [GITHUB_REPO_URL]
- Analyze the architecture, components, and demo topology
- Extract any sample code, deployment scripts, or configuration details
- Identify the key resource types being deployed

**Step 2: Query Azure Learn MCP Server**
- Use mcp_azure_mcp_documentation to search for:
  - Overview and capabilities of [AZURE_SERVICE_NAME]
  - Best practices and architectural patterns
  - Integration with complementary Azure services
  - Security, compliance, and governance guidance
  - Pricing and cost optimization strategies
  - Common deployment patterns and use cases
  
- Use mcp_azure_mcp_get_bestpractices to retrieve:
  - Official best practices for [SERVICE]
  - Code generation guidelines
  - Security recommendations
  - Operational excellence patterns

**Step 3: Current Azure Information**
- Fetch latest pricing, SKU information, and regional availability
- Identify newest features and recent announcements
- Gather integration points with other Azure services
- Find official support and documentation references

**Step 4: Cross-Reference**
- Align GitHub demo architecture with official Azure guidance
- Identify any advanced features or optimizations not yet in the demo
- Map demo components to Well-Architected Framework principles
- Highlight industry-specific compliance and security considerations

**Output Note**: Do NOT ask the user to provide documentation links. Everything needed should come from:
- Azure Learn MCP Server (authoritative source)
- GitHub repository README (demo specifics)
- Your knowledge of Azure services and best practices

```

---

## How to Use This Prompt

1. Fill in the bracketed placeholders `[LIKE_THIS]` with your specific Azure service, repository, audience, and duration
2. Copy the entire **The Prompt Template** section (between the triple backticks)
3. Submit it to your AI assistant
4. The AI will automatically query the MCP server and generate your talk track
5. Request specific customizations and iterations based on your needs

For detailed guidance on customization, audience-specific variations, context-specific adjustments, and examples for different Azure services, see [README.md](README.md).
