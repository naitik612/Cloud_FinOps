# Right-Sizing & Usage Optimization

## Overview
Eliminate waste by matching resource capacity to actual demand.

## Right-Sizing Process

### 1. Identify Candidates
- Underutilized instances (CPU < 40%, Memory < 60%)
- Oversized resources
- Idle resources (0% utilization)

### 2. Analyze Metrics
```
Key Metrics:
- CPU Utilization (average, peak)
- Memory Utilization
- Network I/O
- Disk I/O
- Instance runtime hours
```

### 3. Recommend Changes
- Downsize: Move to smaller instance types
- Upsize: Address performance bottlenecks
- Terminate: Remove unused resources
- Consolidate: Merge workloads

### 4. Implement & Validate
- Test in non-production first
- Gradual rollout to production
- Monitor performance post-change

## Common Optimization Patterns

### Auto-Scaling
```yaml
Scale-Up Triggers:
  - CPU > 70% for 5 minutes
  - Memory > 80% for 5 minutes

Scale-Down Triggers:
  - CPU < 30% for 15 minutes
  - Memory < 40% for 15 minutes
```

### Scheduled Scaling
- Dev/Test environments: Off during non-business hours
- Batch jobs: Scale up during processing windows
- Regional workloads: Follow timezone patterns

## Savings Potential
- Typical savings: 20-40% of compute costs
- Quick wins: Stopping dev/test environments saves 60-75%
