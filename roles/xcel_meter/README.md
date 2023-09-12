Xcel Meter Data for Home Assistant
=========

Adds Xcel Meter data to home assistant.

Requirements
------------

- openssl

If certificates are not provided to the role, then OpenSSL is required on the target
host to generate the CSR and the certificate.

Role Variables
--------------

```YAML
hass_xcel_meter_cert:
  common_name: XceliTronMeter

# $/kWh price of energy during the summer
xcel_energy_price_summer: '0.103010'

xcel_energy_price_winter: '0.08803'

# $/kWh price of energy during the summer
hass_xcel_rate_input_entity: ""

# String containing private key content
hass_xcel_meter_key_data: ""

# String containing certificate content
hass_xcel_meter_cert_data: ""
```

Dependencies
------------

- Role: chriswgerber.home_assistant.configuration

Specified as dependency in `meta/main.yml`

Author Information
------------------

Author: Chris W. Gerber
