# M253BSP_FLASH_EMULATE_EEPROM
 M253BSP_FLASH_EMULATE_EEPROM


update @ 2023/05/16

1. Due to M253 have no data flash , use last 4 page (one page : 0x200 , 512 byes) for emulate EEPROM algorithm

2. startup.s Heap_Size , modify as 0x100

3. use terminal operation 

digit 1 : read all EEP index

digit 2 : increase 1 at each all EEP index

digit 3 : erase all EEP index to 0xFF

3. Below is log capture 

read data and erase , 

![image](https://github.com/released/M253BSP_FLASH_EMULATE_EEPROM/blob/main/read_erase_read.jpg)	


write data and read , 

![image](https://github.com/released/M253BSP_FLASH_EMULATE_EEPROM/blob/main/write_read_write_read.jpg)	

![image](https://github.com/released/M253BSP_FLASH_EMULATE_EEPROM/blob/main/write_read_write_read2.jpg)	


