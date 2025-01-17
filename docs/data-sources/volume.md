---
# generated by https://github.com/hashicorp/terraform-plugin-docs
page_title: "civo_volume Data Source - terraform-provider-civo"
subcategory: ""
description: |-
  Get information on a volume for use in other resources. This data source provides all of the volumes properties as configured on your Civo account.
  An error will be raised if the provided volume name does not exist in your Civo account.
---

# civo_volume (Data Source)

Get information on a volume for use in other resources. This data source provides all of the volumes properties as configured on your Civo account.

An error will be raised if the provided volume name does not exist in your Civo account.

## Example Usage

```terraform
data "civo_volume" "mysql" {
    name = "database-mysql"
}
```

<!-- schema generated by tfplugindocs -->
## Schema

### Optional

- `name` (String) The name of the volume
- `region` (String) The region where volume is running

### Read-Only

- `created_at` (String) The date of the creation of the volume
- `id` (String) The ID of this resource.
- `mount_point` (String) The mount point of the volume
- `size_gb` (Number) The size of the volume (in GB)


