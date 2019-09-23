# Forumla-students---Break-Over-Travel-Circuitry
In forumla students competetion, one of the main functions that needs to be implemented on the car is the Break Over Travel Circuitry. Essentially there's a safety button behind the brake which when pressed indicates that there's a problem has occured. In this case for the safety of the driver, the power supply needs to be disconnected from all the actuators immediately. This was done throughout relays as shown below. 

Circuit when the car is switched off
![](Circuit%20when%20the%20car%20is%20switched%20off.png)

Circuit when the car is switched on
![](Circuit%20when%20the%20car%20is%20switched%20on.png)

After the car starts the relay coil isn't activated yet so K1 is opened and K2 is closed (they are in their normal positions). Since K2 is closed, outputs and the LED are connected to the 12 V supply line via K2. This will make the LED lighting which indicates that we are in the run mode and the outputs are working correctly. This is what we should expect because when we switch on the car the brake pedal is working correctly and the outputs will be working correctly as well. 

After Push_for_fail_Mode1 Push button is pressed (the brake fails)
![](After%20Push_for_fail_Mode1%20Push%20button%20is%20pressed%20(the%20brake%20fails).png)

When the brake pedal travels more than it's meant to be the push_for_fail_mode1 (normally opened) push button will be pressed which will energize the relay coil. Making K1 pole closed and K2 pole opened. The wire connecting from point A to point B will then energize the relay coil even when the push button is released (bypassing current to the relay coil). When K2 pole is opened the connection between the supply voltage and the outputs will then be disconnected. Stopping the car from accelerating and switching off the LED (the indicator).

After Push_for_Run_mode1 push button (the reset button) is pressed
![](After%20Push_for_Run_mode1%20push%20button%20(the%20reset%20button)%20is%20pressed.png)

When the push_for _run_mode1 (normally closed push button) is pressed the connection between point A and Point B will be cut which will deactivate the relay coil. Because this is a non-latching relay, the poles will return to its original position when the coil was not activated (K1 will be opened because it's normally opened and K2 will be closed because it's normally closed). This will again connect the supply voltage to the outputs and the LED, which will make the car move again and the LED (indicator) will be switched on again.

## Components Used 
* 12V supply.
* Push_for_fail_mode1 normally opened push button (the button behind the brake pedal.
* Push_for_run_mode1 normally closed push button (the reset button).
* 220 ohms resistor.
* LED which lights when we are in run mode if it's not lighting then we are in fail mode.
* Double pole single throw non latching relay with the first pole is normally opened (K1) and the second pole is normally closed (K2).

Please note this was only used for the application process. It resulted in me being accepted in formula students soceity to be 1 out of 10 electrical team memebers in 2016.
