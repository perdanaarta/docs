- [Azure Resources Naming Convention](#azure-resources-naming-convention)
  - [Medium, multi region services](#medium-multi-region-services)
- [Resource Short Code](#resource-short-code)
- [Region Short Code](#region-short-code)
- [Environments](#environments)

# Azure Resources Naming Convention

## Medium, multi region services
**Example without instance number**

    master-pip-prod-sea
      |     |   |    |
      |     |   |    resource region
      |     |   environment
      |     resource type
      app/stack name

Usually we want to conserve public IP as long as possible, so we only inclued region and environment as its naming scheme. We want to avoid re-creating a public ip as it could disturb our workflow

**Example with instance number**

    master-vm-prod-sea-1-disk-1
      |    |   |    |  |  |   v
      |    |   |    |  |  v   attached resource instance number
      |    |   |    |  v  atttached resource type
      |    |   |    v  instance number
      |    |   v    region (shortened)
      |    v   environment
      v    resource type
      app/stack name

A vm with its attachment usually deployed as a set with load balancer to distribute load to multiple instance with cost saving in mind

# Resource Short Code

# Region Short Code

# Environments