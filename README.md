# Terraform GCR
A terraform module to ensure GCR bucket exists on GCP


## Usage

```hcl
#------------------------------
# Ensure GCR Bucket Exists
#------------------------------
module "gcr" {
  source   = "../modules/gcr"
  project  = var.project_id
  location = var.location
}
```

## Contributing

Report issues/questions/feature requests on in the issues section.

Full contributing guidelines are covered [here](CONTRIBUTING.md).

<!-- BEGINNING OF PRE-COMMIT-TERRAFORM DOCS HOOK -->
## Requirements

No requirements.

## Providers

| Name | Version |
|------|---------|
| google | n/a |

## Inputs

| Name | Description | Type | Default | Required |
|------|-------------|------|---------|:--------:|
| location | (Optional) The location of the registry. One of ASIA, EU, US or not specified. See the official documentation for more information on registry locations. | `any` | `null` | no |
| project | (Optional) The ID of the project in which the resource belongs. If it is not provided, the provider project is used. | `any` | `null` | no |

## Outputs

No output.

<!-- END OF PRE-COMMIT-TERRAFORM DOCS HOOK -->
