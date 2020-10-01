# terraform-azure-subnets-associations

Associates a Network Security Group with a Subnet.
It is based on the official [```azurerm_subnet_network_security_group_association``` resource](https://www.terraform.io/docs/providers/azurerm/r/subnet_network_security_group_association.html) from ```azurerm``` provider.

## Example usage

```hcl
inputs = {
    network_security_group_id = "/subscriptions/c2691f6c-0980-428a-b31e-xx/resourceGroups/mycustomrg/providers/Microsoft.Network/networkSecurityGroups/front-nsg"
    subnet_id = "/subscriptions/c2691f6c-0980-428a-b31e-xx/resourceGroups/mycustomrg/providers/Microsoft.Network/virtualNetworks/mysubnet/subnets/front"
}
```
