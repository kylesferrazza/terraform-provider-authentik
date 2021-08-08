---
# generated by https://github.com/hashicorp/terraform-plugin-docs
page_title: "authentik_property_mapping_ldap Resource - terraform-provider-authentik"
subcategory: ""
description: |-
  
---

# authentik_property_mapping_ldap (Resource)



## Example Usage

```terraform
# Create a custom LDAP property mapping

resource "authentik_property_mapping_ldap" "name" {
  name         = "custom-field"
  object_field = "username"
  expression   = "return ldap.get('sAMAccountName')"
}
```

<!-- schema generated by tfplugindocs -->
## Schema

### Required

- **expression** (String)
- **name** (String)
- **object_field** (String)

### Optional

- **id** (String) The ID of this resource.

