# Fujitsu IR AR-JE5
## Fujitsu  AR-JE5 Remote IR codes. (AEHA)

<img src="https://github.com/migabit/Fujitsu_IR_AR-JE5/assets/81569439/0abcc83a-343b-4deb-9439-838390345557" width="30%" height="30%">

Codes of the infrared remote to control the basic functions of Fujitsu air conditioners. <br>
(Checked the operability for the ASY9USCCW model.) 

These codes may also be suitable for other models and models of air conditioners from other manufacturers such as:

Fujitsu :
ASY20F11, ASY25F11, ASY35F11, ASY20FM3, ASY25FM3, ASY35FM3, ASY9RSECW, ASY9RSEC-W, ASY12RSECW, ASY12RSEC-W,
ASY25F2, ASY35F2, ASY9LSACW, AOY9LSAC, ASY12LSACW, AOY12LSAC, ASY12RSJCW, AOY12RSJC, ASY12RSJTW, AOY12RSJT, ASY9USCCW, AOY9USCC, ASY12USCCW, AOY12USCC, ASY7USBCW, ASY9USBCW, ASY12USBCW

General :
ASH7USBCW, AOH7UGBC, ASH7USCCW, AOH7USCC, ASH9FSBCW, AOH9FSBC, ASH9LSACW, AOH9LSAC, ASH9RSJCW,
OH9RSJC, ASH9USBCW, AOH9UGBC, ASH9USCCW, AOH9UFCC, ASH12FSBCW, AOH12FSBC, ASH12LSACW, AOH12LSAC, ASH12RSJCW, AOH12RSJC, ASH12USBCW, AOH12UGBC, ASH12USCCW, AOH12USCC, ASG9F2 , ASG12F2, ASG12F11, ASG9F11, ASY20F11, ASY25F11, ASY35F11

Fuji Electric :
RSM-7FA, RSM-9FA, RSM-12FA, RS-7FC, RS-7UC, RS-9FA, RS-9UA, RS-12FC, RS-12UC, RS-9UB, RS-12UD, RS-9LA, RS-12LA, RO-9LA, RO-12LA, RSW-9RC, RSW-12RC

Hiyasu :
HSM-12U, HSM-9U, HSM-7U

### Use with ESPHome:
````
  - platform: template
    name: "SWING"
    turn_on_action:
      remote_transmitter.transmit_aeha:
         address: 0x28C6
         data: [0x00,0x08,0x08,0xB6]
````			 

