PoE support for UCI
===================

This package provides PoE support for the UCI configuration system in OpenWrt.

PoE support in this package is based on GPIOs, as implemented in Ubiquiti's EdgeSwitch product line.


# Examples

The following show an example `/etc/config/poe` config for the EdgeSwitch 5 XP, where 24V pPOE is enabled on port 5:

```
config port
	option port '1'
	list supported_mode '24v'
	option gpio_24v 'ubnt:24v-poe:port1'
	option mode 'off'

config port
	option port '2'
	list supported_mode '24v'
	option gpio_24v 'ubnt:24v-poe:port2'
	option mode 'off'

config port
	option port '3'
	list supported_mode '24v'
	option gpio_24v 'ubnt:24v-poe:port3'
	option mode 'off'

config port
	option port '4'
	list supported_mode '24v'
	option gpio_24v 'ubnt:24v-poe:port4'
	option mode 'off'

config port
	option port '5'
	list supported_mode '24v'
	option gpio_24v 'ubnt:24v-poe:port5'
	option mode '24v'
```




This next config shows an example `/etc/config/poe` config for the EdgeSwitch 8 XP, where multiple PoE modes are available:

```
config port
	option port '1'
	list supported_mode '24v'
	list supported_mode '48v'
	option gpio_24v 'ubnt:24v-poe:port1'
	option gpio_48v 'ubnt:48v-poe:port1'
	option mode 'off'

config port
	option port '2'
	list supported_mode '24v'
	list supported_mode '48v'
	option gpio_24v 'ubnt:24v-poe:port2'
	option gpio_48v 'ubnt:48v-poe:port2'
	option mode 'off'

config port
	option port '3'
	list supported_mode '24v'
	list supported_mode '48v'
	option gpio_24v 'ubnt:24v-poe:port3'
	option gpio_48v 'ubnt:48v-poe:port3'
	option mode 'off'

config port
	option port '4'
	list supported_mode '24v'
	list supported_mode '48v'
	option gpio_24v 'ubnt:24v-poe:port4'
	option gpio_48v 'ubnt:48v-poe:port4'
	option mode 'off'

config port
	option port '5'
	list supported_mode '24v'
	list supported_mode '48v'
	option gpio_24v 'ubnt:24v-poe:port5'
	option gpio_48v 'ubnt:48v-poe:port5'
	option mode 'off'

config port
	option port '6'
	list supported_mode '24v'
	list supported_mode '48v'
	option gpio_24v 'ubnt:24v-poe:port6'
	option gpio_48v 'ubnt:48v-poe:port6'
	option mode '24v'

config port
	option port '7'
	list supported_mode '24v'
	list supported_mode '48v'
	option gpio_24v 'ubnt:24v-poe:port7'
	option gpio_48v 'ubnt:48v-poe:port7'
	option mode '24v'

config port
	option port '8'
	list supported_mode '24v'
	list supported_mode '48v'
	option gpio_24v 'ubnt:24v-poe:port8'
	option gpio_48v 'ubnt:48v-poe:port8'
	option mode '24v'
```
