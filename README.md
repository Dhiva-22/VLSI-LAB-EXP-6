# VLSI-LAB-EXP-6
# SCHEMATIC ENTRY AND SIMULATION OF CMOS INVERTER, CMOS NAND and CMOS NOR USING CADENCE TOOL

## APPARATUS REQUIRED:

Laptop with MobaXterm
Cadence tool PROCEDURE SCHEMATIC ENTRY: Creating a new library:
In the library manager, execute File - New library. The new library form appears.
In the new library form, type ‘my design lib’ in the name section.
In the field of directory section, verify that the path to the library is set to ~/Database / Cadence- analog – lab –bl3 and click ok.
In the next ‘technology file for new library form select option attach to an existing tech file and click ok.
In the ‘attach design library to technology file’ form, select gpdk045 form the cyclic field and click ok.
After creating a new library you can verify it from the library manager.
If you right click on the ‘my design lib’ and select properties, you will find that gpdk045 library is attached as techlib to ‘my design lib’.
Creating a schematic cell view:

In the CIW or library manager, execute file – new – cell viw.
Setup the new file form as follows, Do not edit the library path file and the above might be different from the path shown in your form.
Click ok when done the above setting. A black schematic window for the inverter design appears.
## Adding components to schematic:

In the inverter schematic window, click the instance fixed menu icon to display the add instance form.
Click on the browse button. This opens up a library browser from which you can select components and the symbol view.
After you complete the add instance form move your cursor to the schematic window and click left to place a component. LIBRARY NAME CELL NAME gpdk045 PMOS gpdk045 NMOS
This is a table of components for building the inverter schematic.
After entering components, click cancel in the add instance form or press ESC with your cursor in the schematic window.
![image](https://github.com/Dhiva-22/VLSI-LAB-EXP-6/assets/161815121/963c9f2b-7e69-4ff3-94a4-3b9dc12db424)




## Adding pins to schematic:

Click the pin fixed menu icon in the schematic window. You can execute create pin or press ‘p’.
Add pin form appears. Type the following in the ADD pin form in the next order leaving space between the pin. PIN NAMES DIRECTION Vin,Vdd,Vss Input Vout Output
Select cancel and then the schematic window enter window file or press the f bind key. Adding wires to schematic:
Click the wire (narrow) icon in the schematic window.
In the schematic window click on a pin of one of your components as the first point for your wiring. A diamond shape appears over the starting point of this wire.
Follow the prompts at the bottom of design window and click left on the destination point for your wire. A wire is routed between the source and destination points.
Complete the wiring as shown in the figure and when done wiring press ECS key in the schematic window to cancel wiring.
Saving the design: Click the check and save icon in the schematic editor window observe CIW output for any errors.

## BUILDING THE INVERTER TEST DESIGN: Creating the inverter test cell view:

In the CIW or library manager, execute file – new – cell view.
Setup the newfile as shown below.
Click ok when done. A blank schematic window for the inverter test design appears.
Using the components list and properties/ comments in this table build the inverter test schematic. LIBRARY NAME CELL VIEW NAME PROPERTIES/COMMENTS My design lib Inverter Symbol Analog lib Vpulse Voltage1 = 0, Voltage2 = 1.8, delay Time = 0, Rise time=Fall time=1ns Period=20ns Analog lib Vdc, gnd Vdc = 1.8v
Add the above components using create – instance or by pressing I.
Click the wire (narrow) icon and wire your schematic.
Click create wire name or press c to name the i/p (vsin) and output wires as in below schematic.
Click on the check and save icon to save the design.

![image](https://github.com/Dhiva-22/VLSI-LAB-EXP-6/assets/161815121/98c0bbff-0647-4cb5-9c01-40f724accf50)


## ANALOG SIMULATION WITH SPECTRA: Starting the simulation environment:

In the Inverter-test schematic window execute launch – ADEL. The variable virtuoso analog design environment (ADE) simulation window appears. Choosing a simulator:
In the simulation window (ADE) execute setup – simulator / directory / host.
In the choosing simulator form, set the simulator field to specra and click ok.
In the simulation window (ADE) execute the setup model libraries. To complete, move the cursor and click ok. Choosing Analysis:
Click the choose- Analysis icon in the simulation window (ADE).
The choosing analysis form appears.
To Setup the transient analysis. a. In the analysis section select tron. b. Set the stop time as 100ns c. Click at the moderate or enabled button and the bottom and then click apply.
To set for DC analysis a. In the analysis section select DC. b. Turn on save DC operating point. c. Turn on the component parameters. d. Double click the select Vpulse source or Type V0 (capital V zero). e. Select the DC voltage in the select window parameter and click in the form start and stop voltages are 0 to 1.8. f. Select the enable button and click apply and then click ok.
Selecting output for plotting:

Execute the o/p’s to be plotted -select on sschematic in the simulation window.
Follow the prompt at the bottom. Click on the o/p net vout input vin of the inverter. Press esc with the cursor after selecting.
Running the simulation:

Execute the simulation Netlist and run in the simulation window to start the simulation on the icon. This will create the netlist as well as run the simulation.
When the simulation finishes the transient and DC plots automatically will be popped up along with netlist.
![image](https://github.com/Dhiva-22/VLSI-LAB-EXP-6/assets/161815121/369ec686-e52b-4037-b512-5be998ca650c)

![image](https://github.com/Dhiva-22/VLSI-LAB-EXP-6/assets/161815121/313c479d-a9f4-42d0-87d4-226826928de9)




# CMOS NAND GATE

## NAND SCHEMATIC

![image](https://github.com/Dhiva-22/VLSI-LAB-EXP-6/assets/161815121/b1155804-8f6d-499f-bbdf-6cd929e31288)


## NAND TEST CELL VIEW

![image](https://github.com/Dhiva-22/VLSI-LAB-EXP-6/assets/161815121/30602559-f737-4877-8228-b9140454a67f)


## NAND SIMULATION WITH SPECTRA

![image](https://github.com/Dhiva-22/VLSI-LAB-EXP-6/assets/161815121/76c5e518-e4db-485e-ad58-afb9f8282e24)


# CMOS NOR GATE

## NOR SCHEMATIC
![image](https://github.com/Dhiva-22/VLSI-LAB-EXP-6/assets/161815121/f45b17ab-83b1-4400-9e1d-27990dd068b5)




## NOR TEST CELL VIEW

![image](https://github.com/Dhiva-22/VLSI-LAB-EXP-6/assets/161815121/2333ef87-9c84-4f43-b939-d6bbe497fe08)


## NOR SIMULATION WITH SPECTRA
![image](https://github.com/Dhiva-22/VLSI-LAB-EXP-6/assets/161815121/d64f32cd-a54e-4f39-9915-7057ee06b90d)



## RESULT:
THe design and simulation of the CMOS inverter and the DC and transient responses using cadence tool is successfully observed and verified.
