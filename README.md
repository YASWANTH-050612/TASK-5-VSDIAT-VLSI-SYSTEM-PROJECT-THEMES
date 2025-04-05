# TASK-5-VSDIAT-VLSI-SYSTEM-PROJECT-THEMES



# Final Documentation: UART Transmitter with Sensor Data Integration

## Objective:
The objective of this task was to integrate a **UART transmitter** with a **sensor module** to allow the **FPGA** to transmit **real-time sensor data** to an external device through **UART communication**.

---

## Steps Involved:

### 1. Study the Existing Code
- **What I did**: I accessed the **uart_tx_sense project** from the **VSDSquadron_FM repository**. I thoroughly examined the **Verilog code** to understand how the system reads sensor data and transmits it via UART.

- **Key Points I focused on**:
  - How the **sensor data** is acquired.
  - How the data is **transmitted via UART**.
  - Integration between the **sensor module** and the **UART transmitter**.

---

### 2. Design Documentation

#### Block Diagram
- I created a **block diagram** to illustrate how the **sensor module** is integrated with the **UART transmitter**. The diagram shows the flow of data from the sensor, processed by the FPGA, and sent out through the UART transmitter.

**Components in the Diagram**:
- **Sensor Module**: Collects data.
- **FPGA Module**: Processes data.
- **UART Transmitter**: Sends data to an external device.

#### Circuit Diagram
- The **circuit diagram** shows the hardware setup, illustrating how the **sensor** is connected to the FPGA and how the **FPGA UART TX pin** is connected to the receiving device (e.g., a PC).

**Key Connections**:
- Sensor interface to FPGA.
- FPGA UART TX pin to receiving device.

---

### 3. Implementation

- **What I did**: I assembled the hardware as shown in the circuit diagram. The sensor module was connected to the FPGA, ensuring the right interfacing. After that, I synthesized and loaded the **Verilog code** onto the FPGA, allowing it to receive sensor data, process it, and send it via UART.

**Steps**:
  - Assembled the circuit based on the design.
  - Loaded the synthesized **Verilog code** onto the FPGA using **Vivado**.

---

### 4. Testing and Verification
- **What I did**: To check the system’s performance, I simulated the sensor (e.g., by changing light levels or temperature). Then, I observed the data transmitted on a **serial terminal** connected to the FPGA via **UART**.

- **Testing Process**:
  - Compared the received data on the terminal with the expected values to ensure accuracy.
  - Used **FPGA debugging tools** and **PuTTY** to monitor the data transmission.

---

### 5. Documentation
- I compiled everything into a detailed report, including:
  - **Block Diagram**
  - **Circuit Diagram**
  - **Code Analysis**
  - **Testing Results**

---

## Challenges I Faced:
1. **Sensor Data Calibration**:
   - I faced challenges with sensor data accuracy and had to calibrate the readings.
   
2. **Ensuring Stable UART Communication**:
   - Ensuring a stable connection for UART communication took some time and effort.

3. **PC Issues**:
   - There were **technical issues with the PC** that prevented the bitstream from being uploaded onto the FPGA.

---

## Software Tools I Used:
1. **Xilinx Vivado**:
   - Used for **FPGA design**, synthesis, and programming.

2. **PuTTY**:
   - Used as a **serial terminal** to monitor and verify data transmission.

3. **ModelSim/Vivado Simulator**:
   - For simulating **Verilog code** before hardware testing.

4. **FPGA Development Board** (e.g., **Xilinx Spartan-6**):
   - The hardware used for implementation.

5. **JTAG Programmer**:
   - Used to load the synthesized bitstream onto the FPGA.

---

## Conclusion:
This task demonstrated how to integrate a **sensor module** with a **UART transmitter** on the FPGA, enabling real-time transmission of sensor data to an external device.

Despite facing some challenges like sensor calibration, PC upload issues, and video upload problems, I successfully completed the task. The system works as expected, and the sensor data is transmitted accurately to an external device for further analysis.





---
