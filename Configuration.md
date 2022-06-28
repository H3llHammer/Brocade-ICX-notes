## Change between primary and secundary boot system flash

- `Switch# boot system flash [primary | secundary]`

## Inter-VLAN Routing

#### Create VLAN

- `Switch(config)# vlan <number> name <name>`

#### Add port to vlan

#### Trunk ports

- `Switch(config-vlan-<id>)# tagged ethernet <stackid>/<slot>/<port>`

#### Access ports

- `Switch(config-vlan-<id>)# untagged ethernet <stackid>/<slot>/<port>`

#### Assign router interface to vlan

- `Switch(config-vlan-<id>)# router-interface ve <vlan-id>`

#### Configure router interface

- `Switch(config)# int ve <vlan-id>`
- `Switch(config-vif-<vlan-id>)# ip address [x.x.x.x/x]`

## Change Hostname

- `Switch(config)# Hostname <hostname>`

## Configure dhcp server pool

- `Switch(config)# ip dhcp-server pool <name>`
- `Switch(config-dhcp-<name>)# dhcp-default-router x.x.x.x`
- `Switch(config-dhcp-<name>)# dns-server x.x.x.x`

#### One exclude ip for line

- `Switch(config-dhcp-<name>)# excluded-address x.x.x.x` 

#### Lease duration time

- `Switch(config-dhcp-<name>)# lease <days> <hour> <minutes>` 

#### Configures the subnet network and mask of the DHCP address pool.

- `Switch(config-dhcp-<name>)# network <network> <subnet-mask>` 
- `Switch(config-dhcp-<name>)# deploy` 