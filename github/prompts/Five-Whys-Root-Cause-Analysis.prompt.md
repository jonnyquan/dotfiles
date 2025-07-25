Your goal is to conduct a comprehensive Five Why's root cause analysis for a given problem.

Ask for the problem description if not provided.

## Analysis Approach

### Step 1: Problem Assessment

Evaluate the problem complexity to determine analysis approach:

- **Simple problems**: Single-system or straightforward issues → Use iterative questioning
- **Complex problems**: Multi-system or organizational issues → Use comprehensive analysis framework

### Step 2: Root Cause Investigation

#### For Simple Problems

Execute traditional iterative questioning:

1. **Why 1**: Ask "Why does [problem] occur?"

   - Identify the most likely immediate cause
   - Document reasoning and supporting evidence

2. **Why 2-5**: Continue the chain
   - Ask "Why does [previous answer] occur?"
   - Dig deeper into underlying causes
   - Stop early if root cause is clearly identified

#### For Complex Problems

Conduct comprehensive multi-dimensional analysis:

1. **Technical Analysis**

   - Java application failures, microservice infrastructure issues, database problems
   - Focus: Application logs, stack traces, JVM metrics, Gradle build failures, gRPC errors
   - Output: Technical root causes with evidence from monitoring and logging

2. **Process Analysis**

   - CI/CD workflow failures, deployment issues, development process gaps
   - Focus: Gradle build processes, deployment pipelines, team communication
   - Output: Process improvements and organizational causes

3. **Infrastructure Analysis**

   - MySQL database performance, Kafka cluster issues, service mesh problems
   - Focus: Database queries, message queue latency, network connectivity
   - Output: Infrastructure-centered causes and capacity requirements

4. **Integration Analysis**

   - gRPC service communication failures, Kafka event processing issues
   - Focus: Service contracts, event schemas, cross-service dependencies
   - Output: Integration patterns requiring architectural solutions

5. **Historical Pattern Analysis**
   - Past incidents, recurring patterns, trend analysis
   - Focus: Incident history, pattern recognition, prevention
   - Output: Systemic issues requiring long-term solutions

### Step 3: Synthesis and Recommendations

- Identify the primary root cause
- Document contributing factors
- Generate actionable solutions
- Define preventive measures

## Output Format

Provide a comprehensive analysis following this structure:

```markdown
# Five Why's Root Cause Analysis

## Problem Statement

[Clear description of the problem being analyzed]

## Analysis Approach

[Simple iterative vs. comprehensive multi-dimensional]

## Investigation Results

### Analysis Chain

[For simple problems: Traditional 5 why's chain] [For complex problems: Multi-dimensional findings summary]

### Root Cause

[Primary root cause with supporting evidence]

### Contributing Factors

[Additional factors that contributed to the problem]

## Recommendations

### Immediate Actions

- [Short-term fixes to address symptoms]

### Long-term Solutions

- [Systemic changes to address root cause]

### Preventive Measures

- [Steps to prevent recurrence]

## Next Steps

[Specific, actionable items with ownership and timelines]
```

## Requirements

- Focus on process and system failures, not individual blame
- Look for actionable root causes within reasonable control
- Validate assumptions with evidence when possible
- Consider multiple contributing factors
- Provide specific, measurable recommendations
- Include both immediate fixes and long-term prevention

## Analysis Guidelines

- **Be systematic**: Follow the structured approach consistently
- **Be evidence-based**: Support conclusions with observable facts
- **Be actionable**: Focus on causes that can be addressed
- **Be comprehensive**: Consider technical, process, human, and environmental factors
- **Be preventive**: Include measures to avoid future occurrences

#file:docs/configuration/troubleshooting.md #file:README.md #file:build.gradle #file:src/main/resources/application.yml
