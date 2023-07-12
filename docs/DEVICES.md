### Networking

At the core of a smart house you need good networking equipment. I made the switch to the Prosumer Unifi and have been very happy with it. It has some pretty advanced features and allows me to setup VPN to the house relatively easily

| Device    | Quantity | Integration | Notes |
| --------- | :------: | ------- | ----- |
| <a href="https://store.ui.com/us/en/pro/category/all-switching/products/udm-pro"><img src="https://images.svc.ui.com/?u=https%3A%2F%2Fcdn.ecomm.ui.com%2Fproducts%2F9df27ed4-c4ae-471a-8982-f5b0650da76a%2Fd9511b02-b4bd-46ff-976f-e7bbccf99ae8.png&q=75&w=3840" width="px" height="150px"></a> [Dream Machine Pro]() | 1 | [Unifi Network](https://www.home-assistant.io/integrations/unifi/) | The Dream Machine Pro is a fantastic controller, switch and NVR system. My only down of this system is that it doesn't have any POE ports. |
| <a href="https://store.ui.com/us/en/products/usw-24"><img src="https://images.svc.ui.com/?u=https%3A%2F%2Fcdn.ecomm.ui.com%2Fproducts%2F467359c4-e5c3-487b-ae00-f6b7de29c6fc%2F94c1e7c7-1302-4484-a2cc-0e155b46f615.png&q=75&w=3840" width="px" height="150px"></a> [24 port Switch]() | 1 | [Unifi Network](https://www.home-assistant.io/integrations/unifi/) | 24 port switch with 16 POE+ ports. I use this to power APs and additional devices |
| <a href="https://store.ui.com/us/en/pro/category/all-wifi/products/u6-plus"><img src="https://images.svc.ui.com/?u=https%3A%2F%2Fcdn.ecomm.ui.com%2Fproducts%2F6d5c6141-e2e9-416a-b789-53e59416bb1a%2Ff13853b8-ddfe-4b56-b25d-dab3ffe81b0e.png&q=75&w=3840" width="px" height="150px"></a> [U6+](https://store.ui.com/us/en/pro/category/all-wifi/products/u6-plus) | 3 | [Unifi Network](https://www.home-assistant.io/integrations/unifi/) | At the time of purchase they were out of the U6 Lite so I had to step it up to these. But I am overall impressed with Unifi equipment and will be mounting them on the ceiling for the best coverage |
| <a href="https://store.ui.com/us/en/pro/category/all-wifi/products/u6-lite"><img src="https://images.svc.ui.com/?u=https%3A%2F%2Fcdn.ecomm.ui.com%2Fproducts%2F6d5c6141-e2e9-416a-b789-53e59416bb1a%2Ff13853b8-ddfe-4b56-b25d-dab3ffe81b0e.png&q=75&w=3840" width="px" height="150px"></a> [U6 Lite](https://store.ui.com/us/en/pro/category/all-wifi/products/u6-lite) | 1 | [Unifi Network](https://www.home-assistant.io/integrations/unifi/) | I have an old U6 Lite as they were out of stock I had to go with the three other plus models. If this doesn't fit it I will upgrade to the Plus |
| <a href="https://store.ui.com/us/en/pro/category/all-power-tech/products/usp-pdu-pro"><img src="https://images.svc.ui.com/?u=https%3A%2F%2Fcdn.ecomm.ui.com%2Fproducts%2Fb178b896-3499-4fa3-8c56-ce2822be933f%2F79ee9194-a423-479a-94e3-3189a71d4295.png&q=75&w=2048" width="px" height="150px"></a><br>[Power Distribution Professional](https://store.ui.com/us/en/pro/category/all-power-tech/products/usp-pdu-pro) | 1 | [Unifi Network](https://www.home-assistant.io/integrations/unifi/) | This is the first time I've used this unit. But I like that I can control the power of the cabinet if I need, I can even reset the modem without having to manually unplug it |

#### Additional Resources

[Unifi - Home Assistant Community Add-on](https://community.home-assistant.io/t/home-assistant-community-add-on-unifi-controller/56297)

### Computers, storage & more

| Device | Purpose |
| ------ | ------- |
| <a href="https://amzn.to/3XM2rc1"><img src="https://m.media-amazon.com/images/I/71FrPdp4wOL._AC_SX679_.jpg" width="200px" height="80px"></a> [NUC8 Intel i3](https://amzn.to/3XM2rc1) | I linked the newer version but it's the barebones system so you will have to put it together if you go this route. I really like that I can put the specs in I want and upgrade if I need to. This runs [Debian Linux](https://www.debian.org) and Docker to run the applications I need. |
| <a href="https://amzn.to/3Y4xq3n"><img src="https://th.bing.com/th/id/OIP.Xs5eAgeaX6hPIoJE8Z-oAQHaHa?pid=ImgDet&rs=1" width="200"></a> [PiKVM V4 - Mini](https://pikvm.org) | This is nice if I need to get a KVM (Keyboard / Video / Mouse) locally or remotely (through VPN) if there is an issue with the NUC8 |
| <a href="https://amzn.to/3Y4xq3n"><img src="https://m.media-amazon.com/images/I/51xjiZy7KtL._AC_SX679_.jpg" width="200"></a> [Synology 1621+](https://amzn.to/3Y4xq3n) | This is storage, not sure I need to go much more into what it does. But it's great and recommend Synology overall. I bought this a while ago but the newer ones are pretty much the same thing |
| <a href="https://amzn.to/3OdcxzE"><img src="https://m.media-amazon.com/images/I/51zGK54RWWL._AC_SX679_.jpg" width="75px"></a><br>[Eaton UPS 5S](https://amzn.to/3OdcxzE) | I chose this Eaton because it supports NUT (Network UPS Tools) and with this I can then integrate it into Home Assistant. This is a solid (1500VA / 900W) for a reasonable cost. I run this from the wall then to the Power Distribution Pro |
| <a href="https://amzn.to/3pxnWLq"><img src="https://images-na.ssl-images-amazon.com/images/I/61-zByP2fTL._SL1500_.jpg" width="190px" height="150px" /></a> [Aeotec Z-Stick Gen5](https://amzn.to/3pxnWLq) | Used as my primary Z-Wave hub for Home Assistant. Using secure Z-Wave that is configured in the configuration.yaml |
| <a href="https://amzn.to/3XQKhpn"><img src="https://m.media-amazon.com/images/I/61oHkgKDUoL._AC_SX679_.jpg" width="190px" height="150px" /></a> [Aqara Zigbee Hub](https://amzn.to/3XQKhpn) | Used as my primary ZigBee hub for Home Assistant. Using secure Z-Wave that is configured in the configuration.yaml |
| <a href="https://amzn.to/3POMC2k"><img src="https://m.media-amazon.com/images/I/51vU5wLPWUL._AC_SX679_.jpg" width="190px" height="150px" /></a> [Lutron Caseta Hub](https://amzn.to/3POMC2k) | Used as the Lutron Hub, Lutron uses a proprietry connection called Clear Connect, which stinks as I'm pretty setup for a good mesh network of Z-Wave and ZigBee but nothing I can do. |

## Lights

This time around I went with Smart switches vs Smart bulbs. I really do like Philips Hue but when internet is out or there is an issue with the Hub things fall apart quickly. I like the Lutron Caseta's and they are reliable
| Device  | Quantity | Connection | Component | Notes |
| ------------- | :---: | ------------- | ------------- | ------------- |
| <a href="https://amzn.to/3NJZbt4"><img src="https://m.media-amazon.com/images/I/51vU5wLPWUL._AC_SX679_.jpg" width="200px"></a><br> [Lutron Caseta](https://amzn.to/3NJZbt4) | {WIP} | Clear Connect | [Lutron Caseta](https://www.home-assistant.io/integrations/lutron_caseta/) | I'm new to these switches but I like the reliability over the Philips Hue. It also saves a lot per bulb rather than Philips Hue. They also have a pleasant dimming effect when turning off. |

### Indoor Climate

| Device  | Quantity | Connection | Component | Notes |
| ------------- | :---: | ------------- | ------------- | ------------- |
| <a href="https://amzn.to/3OaKosH"><img src="https://m.media-amazon.com/images/I/51vjw8de57L._AC_SX679_.jpg" width="150px" height="120px" /></a><br> [ecobee3 Lite](https://amzn.to/3OaKosH) | 2 | Wi-Fi | [ecobee](https://www.home-assistant.io/components/ecobee/) | Component works great, I use this for my entire HVAC system. I have multiple modes, AWAY, SLEEP, HOME. I also configured it to only be within 3 degrees rather than the typical 5 |
| <a href="https://amzn.to/3ry0S5e"><img src="https://images-na.ssl-images-amazon.com/images/I/61T5C%2B93PjL._AC_SL1500_.jpg" width="200px" height="60px" /></a><br> [Fanimation Fan - 72"](https://amzn.to/3ry0S5e) | 1 | {WIP} | {WIP} | I owned this fan in my previous condo. Although it's a touch more expensive than other fans it's solid build quality and is a statement piece of the room |
| <a href="https://www.homedepot.com/p/Home-Decorators-Collection-Bayshire-60-in-LED-Indoor-Outdoor-Matte-Black-Ceiling-Fan-with-Remote-Control-and-White-Color-Changing-Light-Kit-102L60MBKDB/314467714?MERCH=REC-_-rv_cartempty_rr-_-NA-_-314467714-_-N&"><img src="https://images.thdstatic.com/productImages/c563e5f6-c7a7-414b-9832-1a94a688ed90/svn/matte-black-home-decorators-collection-ceiling-fans-with-lights-102l60mbkdb-64_100.jpg" width="200px" height="95px" /></a><br> [Bayshire Fan - 60"](https://www.homedepot.com/p/Home-Decorators-Collection-Bayshire-60-in-LED-Indoor-Outdoor-Matte-Black-Ceiling-Fan-with-Remote-Control-and-White-Color-Changing-Light-Kit-102L60MBKDB/314467714?MERCH=REC-_-rv_cartempty_rr-_-NA-_-314467714-_-N&) | 1 | {WIP} | {WIP} | Bought this fan from Home Depot and although it had everything integrated I wanted a propeller theme for my office. So this means I will need to integrate WiFi -> RF |
| <a href="https://amzn.to/3XQE50O"><img src="https://m.media-amazon.com/images/I/612jnRAL4kL._AC_SX679_.jpg" width="160px" height="110px" /></a><br> [FIRST ALERT - Hardwired Z-Wave](https://amzn.to/3XQE50O) | 5 | Wi-Fi | [Z-Wave](https://www.home-assistant.io/components/nest/) | I had NEST before but the integration wasn't ideal, I've heard good things about these detectors and for half the cost I want to try them. |

### Media

| Device  | Quantity | Connection | Component | Notes |
| ------------- | :---: | ------------- | ------------- | ------------- |
| <a href="https://amzn.to/3pOhANy"><img src="https://m.media-amazon.com/images/I/81ufrbnPx-L._AC_SY879_.jpg"  height="130px"/></a><br> [Sonos Play:1](https://amzn.to/3pOhANy) | 4 | Wi-Fi | [SONOS](https://www.home-assistant.io/components/sonos/) | No longer manufacturered, but I really like the fact that no microphones were built in. I used these for several years with no issues. They are also still supported. [Latest Model Here](https://amzn.to/3hrVIi4) |
| <a href="https://amzn.to/3JXrPFU"><img src="https://m.media-amazon.com/images/I/71vr1oaCdlL._AC_SX679_.jpg" width="200px" /></a><br> [Sonos Arc](https://amzn.to/3JXrPFU) | 1 | Wi-Fi | [SONOS](https://www.home-assistant.io/components/sonos/) | Great soundbar with excellent quality. SONOS integrates well with Home Assistant and would recommend |
| <a href="https://amzn.to/3DhWqKx"><img src="https://m.media-amazon.com/images/I/71FbQ4nEZfL._AC_SX679_.jpg" width="200px"/></a><br> [Sonos Move](http://a.co/d/6aAYt6w) | 1 | Wi-Fi | [SONOS](https://www.home-assistant.io/components/sonos/) | Expensive at $399 but it is 'portable', the battery life is phenomenal I have gotten 9 hours at 75% volume the entire time. I'm very impressed with the SONOS Move |
| <a href="https://amzn.to/44tKYry"><img src="https://m.media-amazon.com/images/I/81jRyQeYI1S._AC_SX679_.jpg" width="210px" /></a><br> [83" Sony Bravia](https://amzn.to/44tKYry) | 1 | Wi-Fi | [Sony Bravia TV](https://www.home-assistant.io/integrations/braviatv/) | This is my main main TV. Highly recommend OLED and this is the 4K model, I had an LG OLED previously and although I liked it I wasn't a big fan of the operating system |

### Security

| Device  | Quantity | Connection | Component | Notes |
| ------------- | :---: | ------------- | ------------- | ------------- |
| <a href="https://amzn.to/3aQZsZd"><img src="https://m.media-amazon.com/images/I/71ad5XOAzTS._AC_SX679_.jpg" width="130px" height="105px" /></a><br> [August Smart Lock Pro - Gen 4](https://amzn.to/3aQZsZd) | 2 | Z-Wave / Wi-Fi | [August Lock](https://www.home-assistant.io/integrations/august/) | The new August Lock component in Home Assistant is fast and reliable. Z-Wave has been hit or miss for some devices. I like that the new Gen 4 no longer require the Wi-Fi hub and the size is much smaller |
| <a href="https://amzn.to/3DaWtrF"><img src="https://m.media-amazon.com/images/I/51z8ff2relL._AC_SX679_.jpg" width="200px" height="120px" /></a><br> [Aqara Z-Wave Plus Door Sensor](https://amzn.to/3DaWtrF) | 5 | Z-Wave | [Z-Wave](https://www.home-assistant.io/components/zwave/) | TheHookUp has a great video about these devices and was excited to use over the Monoprice ones. You do need a Z-Wave hub if you don't already have one. The small size of these really amaze me anytime I deal with them. |

TODO: Add doorbell
TODO: Add garage door / sensor

### Shower

| Device  | Quantity | Connection | Component | Notes |
| ------------- | :---: | ------------- | ------------- | ------------- |
| <a href="https://amzn.to/37VpOaX"><img src="https://images-na.ssl-images-amazon.com/images/I/61aNUTvrUhL._SL1500_.jpg" width="200px" height="100px" /></a><br> [U by Moen](https://amzn.to/37VpOaX) | 1 | Wi-Fi | N/A Yet (Hoping to use Wi-fi & API) | Amazing Shower Controller, but expensive and requires 2 different parts, (3 if you want the battery)  |

### Sprinkler
| Device | Connection | Component | Notes |
| ------------- | ------------- | ------------- | ------------- |
| <a href="https://amzn.to/3Oex72E"><img src="https://m.media-amazon.com/images/I/516Au-oBKiL._AC_SX679_.jpg" width="200px"></a><br>[Rachio 3 8-Zone](https://amzn.to/3Oex72E) | Rachio | [Rachio](https://www.home-assistant.io/integrations/rachio/) | This is my first time with a house and a sprinkler system. I've heard great things with the app. I'm excited to hook this into Home Assistant for additional functionality |

### Other

Add W/D

### Software Services / Integrations

*   Weather and Climate related
    *   [Windy](https://www.windy.com/)
    *   [Open Weather Map Api for Node-Red](https://openweathermap.org/api)
    *   [Pollen](https://www.home-assistant.io/components/sensor.pollen/) sensor for allergy related information
*   Presence:
    *   [Life360](https://github.com/pnbruckner/homeassistant-config/blob/master/docs/life360.md)
    *   [iOS app](https://itunes.apple.com/us/app/home-assistant-companion/id1099568401?mt=8)
    *   [Waze](https://www.home-assistant.io/components/sensor.waze_travel_time/) (for commute times)
*   [iOS for Notifications](https://home-assistant.io/docs/ecosystem/ios/notifications/basic/)
*   [Github](https://www.home-assistant.io/components/github/)
