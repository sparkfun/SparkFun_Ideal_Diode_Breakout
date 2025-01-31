---
icon: material/cog
---

<!-- 

In this section, we will highlight the hardware and pins that are broken out on the SparkFun Qwiic Navigation Switch. For more information, check out our [Resources and Going Further](../resources/) on the components used on the breakout board.

<div style="text-align: center;">
  <table>
    <tr style="vertical-align:middle;">
     <td style="text-align: center; vertical-align: middle; border: solid 1px #cccccc;"><a href="../assets/img/PRT-27576_Qwiic_Navigation_Switch_Top_View.jpg"><img src="../assets/img/PRT-27576_Qwiic_Navigation_Switch_Top_View.jpg" width="600px" height="600px" alt="Top View"></a></td>
     <td style="text-align: center; vertical-align: middle; border: solid 1px #cccccc;"><a href="../assets/img/PRT-27576_Qwiic_Navigation_Switch_Bottom_View.jpg"><img src="../assets/img/PRT-27576_Qwiic_Navigation_Switch_Bottom_View.jpg" width="600px" height="600px" alt="Bottom View"></a></td>
    </tr>
    <tr style="vertical-align:middle;">
     <td style="text-align: center; vertical-align: middle; border: solid 1px #cccccc;"><i>Top View</i></td>
     <td style="text-align: center; vertical-align: middle; border: solid 1px #cccccc;"><i>Bottom View</i></td>
    </tr>
  </table>
</div>



### Power

To power the board, you will need **3.3V**. You can connect a Qwiic cable to the Qwiic connector on either side of the board or you can solder directly to the PTHs. Below are the power pins that are broken out on the edge of the board.

* **3V3** &mdash; This pin is the voltage input for the board. The recommended input voltage for this pin is 3.3V.
* **GND** &mdash; Of course, is the common, ground voltage (0V reference) for the system.

<div style="text-align: center;">
  <table>
    <tr style="vertical-align:middle;">
      <td style="text-align: center; vertical-align: middle; border: solid 1px #cccccc;"><a href="../assets/img/PRT-27576_Qwiic_Navigation_Switch_Top_Power_Ground.jpg"><img src="../assets/img/PRT-27576_Qwiic_Navigation_Switch_Top_Power_Ground.jpg" width="600px" height="600px" alt="Power and Ground Highlighted - Top View"></a></td>
     <td style="text-align: center; vertical-align: middle; border: solid 1px #cccccc;"><a href="../assets/img/PRT-27576_Qwiic_Navigation_Switch_Bottom_Power_Ground.jpg"><img src="../assets/img/PRT-27576_Qwiic_Navigation_Switch_Bottom_Power_Ground.jpg" width="600px" height="600px" alt="Power, Ground, and Qwiic Connector Highlighted - Bottom View"></a></td>
    </tr>
    <tr style="vertical-align:middle;">
      <td style="text-align: center; vertical-align: middle; border: solid 1px #cccccc;"><i>Power and Ground Highlighted - Top View</i></td>
     <td style="text-align: center; vertical-align: middle; border: solid 1px #cccccc;"><i>Power, Ground, and Qwiic Connector Highlighted - Bottom View</i></td>
    </tr>
  </table>
</div>



### 5-Way Tactile Switch

A small 5-way tactile switch is populated on the top side of the board and allows for a joystick-like interface in a very small package! Each direction includes a momentary switch that is read by the PCA9554 8-bit I<sup>2</sup>C I/O expander that is populated on the bottom of the board.

<div style="text-align: center;">
  <table>
    <tr style="vertical-align:middle;">
      <td style="text-align: center; vertical-align: middle; border: solid 1px #cccccc;"><a href="../assets/img/PRT-27576_Qwiic_Navigation_Switch_Top_5-way_Tactile_Switch.jpg"><img src="../assets/img/PRT-27576_Qwiic_Navigation_Switch_Top_5-way_Tactile_Switch.jpg" width="600px" height="600px" alt="5-Way Tactile Switch Highlighted - Top View"></a></td>
    </tr>
    <tr style="vertical-align:middle;">
      <td style="text-align: center; vertical-align: middle; border: solid 1px #cccccc;"><i>5-Way Tactile Switch Highlighted - Top View</i></td>
    </tr>
  </table>
</div>



### PCA9554 8-bit I<sup>2</sup>C I/O Expander

The TI PCA9554 that is populated on the bottom side of the board is an 8-bit I<sup>2</sup>C I/O expander that enables users to read and write to the following GPIO pins through I<sup>2</sup>C. It is used to read the 5-way tactile switch or write to the non-addressable RGB LED. The I<sup>2</sup>C address of the PCA9554 is set to **0x20** by default. By adjusting the jumpers on the back of the board, the alternative address can be set to any value between _0x21_ to _0x27_.

* **GPIO0** &mdash; GPIO0 is connected to the 5-way Navigation Switch's UP switch. A 10k&ohm; pull-up resistor is connected.
* **GPIO1** &mdash; GPIO1 is connected to the 5-way Navigation Switch's DOWN switch. A 10k&ohm; pull-up resistor is connected.
* **GPIO2** &mdash; GPIO3 is connected to the 5-way Navigation Switch's RIGHT switch. A 10k&ohm; pull-up resistor is connected.
* **GPIO3** &mdash; GPIO4 is connected to the 5-way Navigation Switch's LEFT switch. A 10k&ohm; pull-up resistor is connected.
* **GPIO4** &mdash; GPIO4 is connected to the 5-way Navigation Switch's CENTER switch. A 10k&ohm; pull-up resistor is connected.
* **GPIO5** &mdash; GPIO5 is connected to the blue LED. The LED can be disconnected if users decide to use a different input to the GPIO5's PTH.
* **GPIO6** &mdash; GPIO6 is connected to the green LED. The LED can be disconnected if users decide to use a different input to the GPIO6's PTH.
* **GPIO7** &mdash; GPIO7 is connected to the red LED. The LED can be disconnected if users decide to use a different input to the GPIO7's PTH.

<div style="text-align: center;">
  <table>
    <tr style="vertical-align:middle;">
      <td style="text-align: center; vertical-align: middle; border: solid 1px #cccccc;"><a href="../assets/img/PRT-27576_Qwiic_Navigation_Switch_Top_PCA9554_IO_I2C_Expander.jpg"><img src="../assets/img/PRT-27576_Qwiic_Navigation_Switch_Top_PCA9554_IO_I2C_Expander.jpg" width="600px" height="600px" alt="PCA9554 Highlighted - Top View"></a></td>
      <td style="text-align: center; vertical-align: middle; border: solid 1px #cccccc;"><a href="../assets/img/PRT-27576_Qwiic_Navigation_Switch_Bottom_PCA9554_IO_I2C_Expander.jpg"><img src="../assets/img/PRT-27576_Qwiic_Navigation_Switch_Bottom_PCA9554_IO_I2C_Expander.jpg" width="600px" height="600px" alt="PCA9554 Highlighted - Bottom View"></a></td>
    </tr>
    <tr style="vertical-align:middle;">
     <td style="text-align: center; vertical-align: middle; border: solid 1px #cccccc;" colspan=2"><i>PCA9554 and Some GPIO Pins Highlighted<br />Top and Bottom View</i></td>
    </tr>
  </table>
</div>



### Qwiic and I<sup>2</sup>C

The board includes two horizontal Qwiic connectors to connect to other Qwiic-enabled I<sup>2</sup>C devices. However, the board still breaks out 0.1"-spaced pins for users who prefer a soldered connection.

* **SCL** &mdash; I<sup>2</sup>C clock on the PCA9554.
* **SDA** &mdash; I<sup>2</sup>C data on the PCA9554.

<div style="text-align: center;">
  <table>
    <tr style="vertical-align:middle;">
     <td style="text-align: center; vertical-align: middle; border: solid 1px #cccccc;"><a href="../assets/img/PRT-27576_Qwiic_Navigation_Switch_Top_I2C_PTH.jpg"><img src="../assets/img/PRT-27576_Qwiic_Navigation_Switch_Top_I2C_PTH.jpg" width="600px" height="600px" alt="Qwiic Connector, I2C, and PCA9554 Highlighted"></a></td>
     <td style="text-align: center; vertical-align: middle; border: solid 1px #cccccc;"><a href="../assets/img/PRT-27576_Qwiic_Navigation_Switch_Bottom_Qwiic_I2C_PTH.jpg"><img src="../assets/img/PRT-27576_Qwiic_Navigation_Switch_Bottom_Qwiic_I2C_PTH.jpg" width="600px" height="600px" alt="Qwiic Connector, I2C, and PCA9554 Highlighted"></a></td>
    </tr>
    <tr style="vertical-align:middle;">
     <td style="text-align: center; vertical-align: middle; border: solid 1px #cccccc;"><i>Qwiic Connector, I<sup>2</sup>C, and PCA9554 Highlighted - Bottom View</i></td>
      <td style="text-align: center; vertical-align: middle; border: solid 1px #cccccc;"><i>I<sup>2</sup>C Highlighted - Top View</i></td>
    </tr>
  </table>
</div>

As explained in the previous section, the I<sup>2</sup>C address of the PCA9554 is set to **0x20** by default. By adjusting the jumpers on the back of the board, the alternative address can be any value between _0x21_ to _0x27_. Make sure to check the Jumpers section below for more information.



### Interrupt

The interrupt pin labeled as INT is for users that want to notify a microcontroller that there is a switch being pushed on the 5-way tactile switch. This pin is active low.

<div style="text-align: center;">
  <table>
    <tr style="vertical-align:middle;">
      <td style="text-align: center; vertical-align: middle; border: solid 1px #cccccc;"><a href="../assets/img/PRT-27576_Qwiic_Navigation_Switch_Top_Interrupt.jpg"><img src="../assets/img/PRT-27576_Qwiic_Navigation_Switch_Top_Interrupt.jpg" width="600px" height="600px" alt="Interrupt Highlighted - Top View"></a></td>
      <td style="text-align: center; vertical-align: middle; border: solid 1px #cccccc;"><a href="../assets/img/PRT-27576_Qwiic_Navigation_Switch_Bottom_Interrupt.jpg"><img src="../assets/img/PRT-27576_Qwiic_Navigation_Switch_Bottom_Interrupt.jpg" width="600px" height="600px" alt="Interrupt Highlighted  - Bottom View"></a></td>
    </tr>
    <tr style="vertical-align:middle;">
     <td style="text-align: center; vertical-align: middle; border: solid 1px #cccccc;" colspan="2"><i>Interrupt Highlighted - Top and Bottom View</i></td>
    </tr>
  </table>
</div>



### LEDs

The board includes two LEDs on the top and bottom of the board. Both can be disabled with the jumpers on the back of the board.

* **PWR** &mdash; On the bottom side of the board, the power LED indicates when power is available on 3.3V.
* **STAT** &mdash; The status LED is a non-addressable RGB LED that is used to indicate which switch is being pushed on the 5-way tactile switch. While this is populated on the bottom of the board, it will light up through the hole toward the top side of the board. Each channel can be disabled with the jumper on the back for users that want to connect them to some other input. Note that two colors were not used since there were only 5 switches available on the tactile switch.
<div style="text-align: center;">
    <table>
        <tr>
            <th style="text-align: center; border: solid 1px #cccccc;">Switch Direction
            </th>
            <th style="text-align: center; border: solid 1px #cccccc;">Color
            </th>
            <th style="text-align: center; border: solid 1px #cccccc;">Red<br />(GPIO7)
            </th>
            <th style="text-align: center; border: solid 1px #cccccc;">Green<br />(GPIO6)
            </th>
            <th style="text-align: center; border: solid 1px #cccccc;">Blue<br />(GPIO5)
            </th>
        </tr>
        <tr>        
            <td style="text-align: center; border: solid 1px #cccccc;">Up
            </td>
            <td style="text-align: center; border: solid 1px #cccccc;">Red
            </td>
            <td style="text-align: center; border: solid 1px #cccccc;">1
            </td>
            <td style="text-align: center; border: solid 1px #cccccc;">0
            </td>
            <td style="text-align: center; border: solid 1px #cccccc;">0
            </td>
        </tr>
        <tr>            
            <td style="text-align: center; border: solid 1px #cccccc;">Down
            </td>   
            <td style="text-align: center; border: solid 1px #cccccc;">Green
            </td>
            <td style="text-align: center; border: solid 1px #cccccc;">0
            </td>
            <td style="text-align: center; border: solid 1px #cccccc;">1
            </td>
            <td style="text-align: center; border: solid 1px #cccccc;">0
            </td>
        </tr>
        <tr>            
            <td style="text-align: center; border: solid 1px #cccccc;">Left
            </td>   
            <td style="text-align: center; border: solid 1px #cccccc;">Magenta
            </td>
            <td style="text-align: center; border: solid 1px #cccccc;">1
            </td>
            <td style="text-align: center; border: solid 1px #cccccc;">0
            </td>
            <td style="text-align: center; border: solid 1px #cccccc;">1
            </td>
        </tr>
        <tr>       
            <td style="text-align: center; border: solid 1px #cccccc;">Right
            </td>        
            <td style="text-align: center; border: solid 1px #cccccc;">Cyan
            </td>
            <td style="text-align: center; border: solid 1px #cccccc;">0
            </td>
            <td style="text-align: center; border: solid 1px #cccccc;">1
            </td>
            <td style="text-align: center; border: solid 1px #cccccc;">1
            </td>
        </tr>
        <tr>       
            <td style="text-align: center; border: solid 1px #cccccc;">Center
            </td>        
            <td style="text-align: center; border: solid 1px #cccccc;">White
            </td>
            <td style="text-align: center; border: solid 1px #cccccc;">1
            </td>
            <td style="text-align: center; border: solid 1px #cccccc;">1
            </td>
            <td style="text-align: center; border: solid 1px #cccccc;">1
            </td>
        </tr>
            <tr><td style="text-align: center; border: solid 1px #cccccc;"><i>No Switch Push</i>
            </td>          
            <td style="text-align: center; border: solid 1px #cccccc;">OFF
            </td>
            <td style="text-align: center; border: solid 1px #cccccc;">0
            </td>
            <td style="text-align: center; border: solid 1px #cccccc;">0
            </td>
            <td style="text-align: center; border: solid 1px #cccccc;">0
            </td>
        </tr>
        <tr>
            <tr><td style="text-align: center; border: solid 1px #cccccc;"><i>Not Assigned</i>
            </td>        
            <td style="text-align: center; border: solid 1px #cccccc;">Blue
            </td>
            <td style="text-align: center; border: solid 1px #cccccc;">0
            </td>
            <td style="text-align: center; border: solid 1px #cccccc;">0
            </td>
            <td style="text-align: center; border: solid 1px #cccccc;">1
            </td>
        </tr>
        <tr>
            <tr><td style="text-align: center; border: solid 1px #cccccc;"><i>Not Assigned</i>
            </td>        
            <td style="text-align: center; border: solid 1px #cccccc;">Yellow
            </td>
            <td style="text-align: center; border: solid 1px #cccccc;">1
            </td>
            <td style="text-align: center; border: solid 1px #cccccc;">1
            </td>
            <td style="text-align: center; border: solid 1px #cccccc;">0
            </td>
        </tr>
    </table>
</div>


<div style="text-align: center;">
  <table>
    <tr style="vertical-align:middle;">
      <td style="text-align: center; vertical-align: middle; border: solid 1px #cccccc;"><a href="../assets/img/PRT-27576_Qwiic_Navigation_Switch_Top_LEDs.jpg"><img src="../assets/img/PRT-27576_Qwiic_Navigation_Switch_Top_LEDs.jpg" width="600px" height="600px" alt="LEDs Highlighted"></a></td>
      <td style="text-align: center; vertical-align: middle; border: solid 1px #cccccc;"><a href="../assets/img/PRT-27576_Qwiic_Navigation_Switch_Bottom_LEDs.jpg"><img src="../assets/img/PRT-27576_Qwiic_Navigation_Switch_Bottom_LEDs.jpg" width="600px" height="600px" alt="LEDs Highlighted"></a></td>
    </tr>
    <tr style="vertical-align:middle;">
     <td style="text-align: center; vertical-align: middle; border: solid 1px #cccccc;" colspan="2"><i>LEDs Highlighted Top and Bottom View</i></td>
    </tr>
  </table>
</div>



### Jumpers

!!!note
    If this is your first time working with jumpers, check out the [How to Work with Jumper Pads and PCB Traces](https://learn.sparkfun.com/tutorials/how-to-work-with-jumper-pads-and-pcb-traces/all) tutorial for more information.

The back of the board includes jumpers to configure the board.

* **PWR** &mdash; By default, the power jumper connects the LED to the output's 3.3V pin. Cutting this trace disables the LED.
* **7** &mdash; By default, this jumper is closed. Cutting this jumper will disconnect GPIO7 and the red channel from the RGB LED. Once disabled, GPIO7 is available for users that want to connect them to some other input.
* **6** &mdash; By default, this jumper is closed. Cutting this jumper will disconnect GPIO6 and the green channel from the RGB LED. Once disabled, GPIO6 is available for users that want to connect them to some other input.
* **5** &mdash; By default, this jumper is closed. Cutting this jumper will disconnect GPIO5 and the blue channel from the RGB LED. Once disabled, GPIO5 is available for users that want to connect them to some other input.
* **I<sup>2</sup>C** &mdash; By default, this three-pad jumper is closed. The three way jumper labeled I<sup>2</sup>C connects 3.3V to two 2.2k&ohm; pull-up resistors and to the I<sup>2</sup>C data and clock lines. If multiple devices are connected to the bus with the pull-up resistors enabled, the parallel equivalent resistance will create too strong of a pull-up for the bus to operate correctly. As a general rule of thumb, [disable all but one pair of pull-up resistors](https://learn.sparkfun.com/tutorials/i2c/all#i2c-at-the-hardware-level) if multiple devices are connected to the bus.
* **ADR**  &mdash; By default, the three jumpers **0**, **1**, and **2** are open. These set the I<sup>2</sup>C address of the Qwiic Navigation Switch. Adding a solder blob will close the jumper and set the jumper as a `1`. Below shows the table needed to configure the three jumpers to achieve the desired I<sup>2</sup>C address.
<div style="text-align: center;">
    <table>
        <tr>
            <th style="text-align: center; border: solid 1px #cccccc;">I<sup>2</sup>C Address
            </th>
            <th style="text-align: center; border: solid 1px #cccccc;">ADR2<br/> (Jumper <b>2</b>)
            </th>
            <th style="text-align: center; border: solid 1px #cccccc;">ADR1<br/> (Jumper <b>1</b>)
            </th>
            <th style="text-align: center; border: solid 1px #cccccc;">ADR0<br/>(Jumper <b>0</b>)
            </th>
        </tr>
        <tr>        
            <td style="text-align: center; border: solid 1px #cccccc;">0x20
            </td>
            <td style="text-align: center; border: solid 1px #cccccc;">0
            </td>
            <td style="text-align: center; border: solid 1px #cccccc;">0
            </td>
            <td style="text-align: center; border: solid 1px #cccccc;">0
            </td>
        </tr>
        <tr>        
            <td style="text-align: center; border: solid 1px #cccccc;">0x21
            </td>
            <td style="text-align: center; border: solid 1px #cccccc;">0
            </td>
            <td style="text-align: center; border: solid 1px #cccccc;">0
            </td>
            <td style="text-align: center; border: solid 1px #cccccc;">1
            </td>
        </tr>
        <tr>        
            <td style="text-align: center; border: solid 1px #cccccc;">0x22
            </td>
            <td style="text-align: center; border: solid 1px #cccccc;">0
            </td>
            <td style="text-align: center; border: solid 1px #cccccc;">1
            </td>
            <td style="text-align: center; border: solid 1px #cccccc;">0
            </td>
        </tr>
        <tr>        
            <td style="text-align: center; border: solid 1px #cccccc;">0x23
            </td>
            <td style="text-align: center; border: solid 1px #cccccc;">0
            </td>
            <td style="text-align: center; border: solid 1px #cccccc;">1
            </td>
            <td style="text-align: center; border: solid 1px #cccccc;">1
            </td>
        </tr>
        <tr>        
            <td style="text-align: center; border: solid 1px #cccccc;">0x24
            </td>
            <td style="text-align: center; border: solid 1px #cccccc;">1
            </td>
            <td style="text-align: center; border: solid 1px #cccccc;">0
            </td>
            <td style="text-align: center; border: solid 1px #cccccc;">0
            </td>
        </tr>
        <tr>        
            <td style="text-align: center; border: solid 1px #cccccc;">0x25
            </td>
            <td style="text-align: center; border: solid 1px #cccccc;">1
            </td>
            <td style="text-align: center; border: solid 1px #cccccc;">0
            </td>
            <td style="text-align: center; border: solid 1px #cccccc;">1
            </td>
        </tr>
        <tr>        
            <td style="text-align: center; border: solid 1px #cccccc;">0x26
            </td>
            <td style="text-align: center; border: solid 1px #cccccc;">1
            </td>
            <td style="text-align: center; border: solid 1px #cccccc;">1
            </td>
            <td style="text-align: center; border: solid 1px #cccccc;">0
            </td>
        </tr>
        <tr>        
            <td style="text-align: center; border: solid 1px #cccccc;">0x27
            </td>
            <td style="text-align: center; border: solid 1px #cccccc;">1
            </td>
            <td style="text-align: center; border: solid 1px #cccccc;">1
            </td>
            <td style="text-align: center; border: solid 1px #cccccc;">1
            </td>
        </tr>
    </table>
</div>

<div style="text-align: center;">
  <table>
    <tr style="vertical-align:middle;">
     <td style="text-align: center; vertical-align: middle; border: solid 1px #cccccc;"><a href="../assets/img/PRT-27576_Qwiic_Navigation_Switch_Bottom_Jumpers.jpg"><img src="../assets/img/PRT-27576_Qwiic_Navigation_Switch_Bottom_Jumpers.jpg" width="600px" height="600px" alt="Jumpers Highlighted - Bottom View"></a></td>
    </tr>
    <tr style="vertical-align:middle;">
     <td style="text-align: center; vertical-align: middle; border: solid 1px #cccccc;"><i>Jumpers Highlighted<br />Bottom View</i></td>
    </tr>
  </table>
</div>

-->

### 3D Model

A 3D model of the board and components was exported to a STEP file using KiCad.

<script type="module" src="https://ajax.googleapis.com/ajax/libs/model-viewer/3.5.0/model-viewer.min.js"></script>

<center>
    <model-viewer src="../assets/3d_model/SparkFun_Ideal_Diode_Breakout_3d_model.glb" camera-controls poster="../assets/3d_model/SparkFun_Ideal_Diode_Breakout_3d_model.png" environment-image="legacy" shadow-intensity="1.58" exposure="0.64" shadow-softness="0.24" tone-mapping="neutral" camera-orbit="-46.67deg 57.14deg 153.3m" field-of-view="30deg" style="width: 750px; height: 500px;">
    </model-viewer>
</center>
<br />
<div style="text-align: center">
    <a href="../assets/3d_model/SparkFun_Ideal_Diode_Breakout_3d_model.step" target="stp_file" class="md-button">Click Here for the STEP File</a>
</div>



### Board Dimensions

The board measures 15.2mm x 12.7mm. 

<figure markdown>
[![Board Dimensions are 15.2mm by 12.7mm](../assets/board_files/SparkFun_Ideal_Diode_Breakout_Dimensions.png){ width="50%" }](../assets/board_files/SparkFun_Ideal_Diode_Breakout_Dimensions.png "Click to enlarge")
<figcaption markdown>Board Dimensions</figcaption>
</figure>

