Notas del dia 4 05/07/2026

Host forwarding decision: La computadora manda mensajes a diferentes destinos como a si mismo o a otro device and el mismo network, tambien a otro device in a different network a travez del default gateway

<!-- !Itself: Manda un mensaje a si mismo para confirmar que pueda recibir mensajes -->

<!-- ?Local host: Manda un mensaje a un device en el mismo network (LAN)  -->

<!-- *Remote host: Es como se envia un mensaje a un different network esta comunicacion se hace a traves de un router -->

*Cuando los mensajes no salen de la red local, lo primero que debemos revisar es el default getway settings en los devices.*

'IP publicas son reutilizables.'

<!-- *NAT (Network address translation): * -->: 
Es lo mismo pero en un diferente idioma. 
No existen suficientes IP, para que no haya repeticiones. Para eso se usa el <NAT.> IP privadas no salen de la red privada. EL NAT permite que diferentes devices compartan un mismo IP publico. 

El problema con 2 routers es cambiar los settings del extra router para que sea un swtich "Wireles Media <Bridge>" y no asigne IP address usando el DHCP ni use NAT

NAT replaces the private IP address for a public one. So multiple private address can be the same but in the internet it will be different.

Usable and importants ports for <SONOS>
53 (udp) DNS 
445,3445 (TCP)
More are in the anki tool.

Lab 1
TS: Check that both devices are under the same default gateway
Both devices have a different IP address
mywifi_2 was the correct network name and router have the correct settings
We found that one of the devices was connected to 5G instead of 2.4

Lab 2
TS: Check if the ports for sonos are blocked 
Confirm that ip address is not blocked
Confirmed that the IP address is ok for the router gui settings
WPA2 Enterprise Sonos cannot work with it only with personal and router was set up for WPA2 Enterprise

Found that Sonos device was connecting to WPA instead of WPA2 psk


lab 4
Sonos device1 is connected to wifi5 y usando wpa instead of WPA psk

Found a MAC address listed in the Wireless MAC address Filter 00:30:A3:1A:9B:29 it belongs to SONOS device 2 

Beamforming 

Check the double name que puede dar problema con el NAT

Lab 3
TS: 2.4 is disabled
The 2 devices are connected to to a 5G network. Even the WPA2 is set up correctly as WPA2 personal SONOS devices can only connect to 2.4 networks

# Activity Router simulators 


### router GUI simuladors
- https://www.tp-link.com/us/support/emulator/ 
- https://demoui.asus.com/
- http://routeremulator.com/
- https://www.snbforums.com/threads/router-ui-emulators.30552/
- https://ui.linksys.com/
- aries, getwgear  

* choose a router from the list above and research how to change the following settings:

- 2.4 GHz enable or disable x
- bridge mode x
- Beamforming 
- Hidden SSID / Network Cloaking  x
- MAC Address Filtering
- guest network 
- UPNP enable and disable 

take SS showing where to find it


Calificacion de los puertos


TCP reliable, mas segura y asegurarme de esta manera de que va a llegar. Nos aseguramos de que llega completa.

UDP, es mas rapido pero no tan reliable o consistente. No va a repetir o buscar information que ya se perdio 
Este es mas rapido pero no tan seguro 

Tipos de atacks
<!-- ?DOS -->
Denegar servicios a traves de requests falsos "Denial of service.

<!-- ?Rouge AP (Unauthorized ap) -->
Devices can connect to a similar AP trying to connect to the correct authorized one.

<!-- *MITM man in the middle* -->
An interception of the information that review that information 

Ways to protect but are not supported by sonos

-1 hidden SSID
-2 Mac address filtering
-3 VPN
-4 Guest Network 

Other things to observe (Allowed or not supportted)

UPnP Universal Plug and Play
QoS quality of service must be off
IGMP proxy must be OFF 
IGMP Snooping ON
Smart connect bandsteering smart steering/ in all of it presentations should be turned off.
Airetime Fairness de prioridad dependiendo del orden en que se conectaron a la red 

Futuros labs
Look at the supported hardware devices 
DHCP issues with the IP


