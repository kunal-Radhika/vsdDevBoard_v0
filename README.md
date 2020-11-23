# SOC Design For Testing Digital IP chips (RISC V and SRAM)
This Project explains the importance of components used in the PCB design and also how data flows within the design.

# Table of Contents
- [Brief Introduction to Testing flow]()
- [Introduction to FT2232H]()
- [Data flow from USB port to FT2232H]()
- [Data flow from FT2232H to SPI flash memory]()
- [Future work]()
- [Acknowledgements]()

# Brief Introduction to Testing flow
An IDE ( Integrated Development Environment) is used for programming the PCB design. For an IDE to recognize the hardware board, a Board Support Package(BSP) which includes hardware description and linker files for memory mapping are used and after programming, the hex files are generated. The resultant bitstream is passed to the following PCB design.

![pcb design](https://user-images.githubusercontent.com/74853558/99901876-d6eb3500-2cdf-11eb-98e2-f7399bf56f47.jpg)

# Introduction to FT2232H
The serial port of the computer usually meets RS-232 standard. It has signal voltage swing of around -13 to +13V. The PCB design uses TTL serial (Transistor-Transistor logic) which has signal voltage level between 0 and VDD ( 3.3V/1.8V). A common communication protocol is needed for data transfer, hence FT2232H is used for converting USB to serial converter.


![1](https://user-images.githubusercontent.com/74853558/99901951-50832300-2ce0-11eb-83eb-0b9878771b1e.jpg)

![2](https://user-images.githubusercontent.com/74853558/99904990-128ffa00-2cf4-11eb-8bde-f9693f8e3624.jpg)

![3](https://user-images.githubusercontent.com/74853558/99904992-13c12700-2cf4-11eb-96e3-813c6a7b75de.jpg) 

![4](https://user-images.githubusercontent.com/74853558/99904993-1459bd80-2cf4-11eb-8905-544269d66b9f.jpg)

![5](https://user-images.githubusercontent.com/74853558/99904994-14f25400-2cf4-11eb-9d85-3402415096fe.jpg)

![6](https://user-images.githubusercontent.com/74853558/99905235-a57d6400-2cf5-11eb-9f23-9140bd84b50f.jpg)

![7](https://user-images.githubusercontent.com/74853558/99905237-a7472780-2cf5-11eb-8387-13a4a12ac96b.jpg)

![8](https://user-images.githubusercontent.com/74853558/99904997-158aea80-2cf4-11eb-925a-c565d1dcbe6b.jpg)

![9](https://user-images.githubusercontent.com/74853558/99904999-16238100-2cf4-11eb-9220-c5b521bf7785.jpg)

![10](https://user-images.githubusercontent.com/74853558/99905000-16bc1780-2cf4-11eb-9f24-1c89a508696d.jpg)

![11](https://user-images.githubusercontent.com/74853558/99905001-16bc1780-2cf4-11eb-96d1-caabca6888cc.jpg)

![12](https://user-images.githubusercontent.com/74853558/99905002-1754ae00-2cf4-11eb-8c51-300a52c790a7.jpg)

![13](https://user-images.githubusercontent.com/74853558/99905003-1754ae00-2cf4-11eb-8f00-3c057b3d4974.jpg)

