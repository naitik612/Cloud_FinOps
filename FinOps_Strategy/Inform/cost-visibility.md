# Cost Visibility & Allocation

## Objectives
- Achieve 100% cost allocation across all cloud resources
- Enable cost transparency for all stakeholders
- Implement tagging strategies for accurate tracking

## Key Practices

### Tagging Strategy
```yaml
Required Tags:
  - Environment: (dev/test/prod)
  - Team: (team-name)
  - CostCenter: (cost-center-id)
  - Application: (app-name)
  - Owner: (email)
```

### Cost Allocation Methods
1. **Direct Allocation**: Tag-based cost assignment
2. **Proportional Allocation**: Shared service distribution
3. **Fixed Allocation**: Predetermined percentages

### Tools & Dashboards
- Cloud Provider Native Tools (AWS Cost Explorer, Azure Cost Management, GCP Cost Management)
- Third-party FinOps platforms
- Custom dashboards and reports

## Metrics
- Percentage of allocated costs
- Untagged resource count
- Cost per service/team
