---
icon: material/run-fast
hide: toc
---

<div class="grid cards desc" markdown>

-    <a href="https://www.sparkfun.com/products/27925">
    **SparkFun Ideal Diode Breakout**<br>
    **SKU:** COM-27925

    ---

    <figure markdown>
    ![Product Thumbnail](assets/img/27925-Ideal-Diode-Breakout-Feature.jpg)
    </figure></a>
    

-    Keep your project powered up during power supply hot-swaps with the SparkFun Ideal Diode Breakout. This compact (15.2mm x 12.7mm) breakout board features four channels and ground connections, providing reliable one-way voltage control. Ideal diodes minimize forward voltage drop, internal power dissipation, and reverse DC leakage current, making them perfect for dynamic power selection and switchover, over-voltage protection, and projects requiring stable power input.

    This breakout boasts impressive performance with a typical forward voltage drop as low as 8mV at 0.1A (20V input) and 62mV at 1A (20V input), ensuring efficient power delivery. For higher current applications, the forward voltage drop is typically 275mV at 4A (20V input). The typical on-resistance ranges from 69mΩ (20V, 4A) to 260mΩ (1.8V, 0.1A), depending on the input voltage and current. Reverse leakage current is minimal, ranging from -50µA to -560µA depending on reverse voltage and again on the input voltage.


    <center>
    [Purchase from SparkFun :fontawesome-solid-cart-plus:{ .heart }](https://www.sparkfun.com/products/27925){ .md-button .md-button--primary }
    </center>

</div>


## Hooking Up the Breakout

Hooking up the SparkFun Ideal Diode Breakout is fairly straightforward. Power inputs go through two separate input circuits but have a common ground. A quick example shows consistent current being supplied to the board from two separate power supplies. Note that as one power supply decreases, the other draw increases to provide consistent voltage: 



<figure markdown>
[![Hot Swapping Power Supply](../assets/img/Ideal-Diode-Breakout-Action-GIF.gif){ width="90%" }](../assets/img/Ideal-Diode-Breakout-Action-GIF.gif "Click to enlarge")
<figcaption markdown>Hot Swapping a Power Supply to a RedBoard</figcaption>
</figure>

Hookup looks something like the following: 


<figure markdown>
[![Hot Swapping Power Supply](../assets/img/hookup.png){ width="90%" }](../assets/img/hookup.png "Click to enlarge")
<figcaption markdown>Hot Swapping a Power Supply to a RedBoard</figcaption>
</figure>


