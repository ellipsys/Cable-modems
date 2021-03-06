# Cisco EPC3925 UPC modem/router default passphrase vulnerabilities #

Platforms / Firmware confirmed affected:
- Cisco EPC3925, ESIP-12-v302r125573-131230c_upc

## Vulnerabilities ##
Default SSID and passphrase can be calculated
The default SSID and passphrase are derived from the MAC address and the DOCSIS serial number. Since the MAC address of the device is broadcasted via WiFi and the typical serial number is within the range 200.000.000 and 260.000.000, the default password can be brute-forced within minutes.

## Timeline ##
- 2015.07.30: We sent some new issues affecting the Ubee router and other findings in Technicolor TC7200 and Cisco EPC3925 devices to UPC
- Between 2015.07.31 and 08.12 there were several e-mail and phone communications between technical persons from Liberty Global to clarify the findings
- 2015.08.19: UPC sent out advisory emails to its end users to change the default WiFi passphrase
- 2016.01.27: UPC Magyarorszag send out a repeated warning to its end users about the importance of the change of the default passphrases.
- 2016.02.16: Face to face meeting with Liberty Global security personnel in Amsterdam headquarters 
- 2016.02.18: A proposal was sent to Liberty Global suggesting a wardriving experiment in Budapest, Hungary to measure the rate of end users who are still using the default passphrases.

## POC ##
POC script is available to demonstrate the default SSID and passphrase generation.

## Recommendations ##
Since only the ISP can update the firmware, we can recommend for users to change the WiFi passphrase.

## Links ##
[Search-lab advisory](http://www.search-lab.hu/advisories/secadv-20150720)
